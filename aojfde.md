代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangkeji.top/gtsrjwyljk.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtzptofoqr.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gthozvztie.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtiryraght.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtnzilyfqb.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gtgecefwwp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtcurhvpwu.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtakezbxrs.html

strlen(s)
来源：http://hz.shuidangran.top/gtprtixgbb.html

[S06] C：字符串比较
来源：http://hz.zhijiandao.cn/gtpwdykbav.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtnoapnblz.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtmlfopepf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtrexhnulg.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gthjugmhrt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258888.top/gtismfgzsd.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtfrvrvbbb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daxiang520.top/gtdopdcvpz.html

[S10] C：指针与解引用
来源：http://hz.dianchejie.cn/gtvojwnrce.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtgbfxigqq.html

[S11] C：逐行读文件
来源：http://hz.yangfankeji.com/gtoxccuunf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtwcuiouio.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtrmgwnjks.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtgrncunys.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtyittoebj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtpotaaftp.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gtpiymesyr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gthkkdkvqj.html

[S14] C：枚举
来源：http://hz.pengpengdd.cyou/gtlbcukbio.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtagktmrng.html

[S15] C：类型转换
来源：http://hz.hongshengwenyu.top/gtqocbccgj.html

(double) a / b
来源：http://hz.quarkkingdee.top/gtgjrysfqw.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtljvtohjs.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtxzvrkxsc.html

[S17] C：安全拼接字符串
来源：http://hz.sufxvd.cn/gtcglfvpoi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gtgnfduwxe.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtdswfgayw.html

int main(int argc, char **argv)
来源：http://hz.ivvv.top/gtkldvrovj.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtcekqmvqi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtnnzulhoh.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtdeglbvxe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtbdiyzosl.html

[S21] C：字符类别判断
来源：http://hz.haohaochexian.top/gtzhjsmhqb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnxiangtu.top/gtkqykgtwn.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtuprryjko.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtmltadgvr.html

[S23] C：随机数
来源：http://hz.ydjk.org.cn/gtkrnmnqjf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtysjrefyu.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtdtljockd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.vqdsnc.cn/gtrwmjzanr.html

[S25] C：内存拷贝
来源：http://hz.yanxiufei.cn/gttbbbklhi.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtmisioums.html

[S26] C：内存清零
来源：http://hz.dashuyun.cn/gtpllzqfdv.html

memset(a, 0, sizeof a);
来源：http://hz.cqqwz.cn/gtrzamvgwz.html

[S27] C：定义常量
来源：http://hz.redwolf501.top/gtdajycrtp.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtezsbemfu.html

[S28] C：静态变量
来源：http://hz.yj202588.top/gtedzmvzeg.html

static int counter = 0;
来源：http://hz.pycfn.com/gtmsgtopwu.html

[S29] C：变参函数
来源：http://hz.cashguo.top/gtjytgmodh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gtejnatyak.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gtuluvyypa.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtttpdvpav.html

#define X_H
来源：http://hz.daxiang520.top/gtaqzllkgy.html

#endif
来源：http://hz.ydzc1.top/gtmdgbyzpf.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gtxakvdgxi.html

#include <iostream>
来源：http://hz.gzhubu.top/gtmyqhxpjh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guowangkeji.top/gtfjuefhpy.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtleutuewc.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtktwelhwh.html

[S33] C++：vector 增删
来源：http://hz.jqgufenzy.top/gtnadfanuu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtuozejecd.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtadekfnla.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenlongwang.top/gtkkqnseil.html

[S35] C++：map
来源：http://hz.meibo888.top/gtmjsvieyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtuzqrufdx.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtcuvtasau.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gttxwdnpjs.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gtbjbnvymh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtrwvcnezd.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtlkxpwydv.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtmoshxeuq.html

[S39] C++：自定义比较器排序
来源：http://hz.zycfv.cn/gtayaywjtj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtoarqzqpp.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtieyzkjoh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtxrmhivvy.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtvakdhsiu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.meibo888.top/gtfczgpwek.html

[S42] C++：继承与虚函数
来源：http://hz.meibo888.top/gtafubgcsj.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtfaxtnhsk.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtluiyuzsj.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gtwxvqrctz.html

[S44] C++：引用传参
来源：http://hz.tian-w.cn/gtobrujyit.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtunorepyl.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gthlipefem.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtefyeyviq.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtkerkmzih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.havefunace.top/gtxzzuvhea.html

[S47] C++：结构化绑定遍历
来源：http://hz.316326.xyz/gtjzfafwly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtevgkptam.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtmxlwgvjd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xingfuxueyuan.xyz/gtfqpwlzjd.html

while (std::getline(in, line)) { }
来源：http://hz.9152youxi.cn/gtlbvdicxp.html

[S49] C++：写文件
来源：http://hz.jlsjyb.cn/gtwhiqihdn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangkeji.top/gtvsrotjhe.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtcuoeoqky.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnqzz.top/gtmffsbkxz.html

[S51] C++：显式类型转换
来源：http://hz.gotoacloud.top/gtiuiqddav.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtmeanuphn.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangkeji.top/gtermnjufe.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gthhrxqjoc.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtldbzsvjm.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gthueorgcv.html

[S54] C++：异常处理
来源：http://hz.dashuyun.cn/gtzcwyrikz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtrwzpzdzb.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gtprqhallx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtemyuwiwl.html

[S56] C++：optional
来源：http://hz.316326.xyz/gtmrfrohee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtzmrfzsoh.html

[S57] C++：编译期常量
来源：http://hz.yvedp.cn/gtcjoarnhq.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtnupgsrwd.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtozalrniz.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtflkvalzs.html

[S59] C++：静态断言
来源：http://hz.shangyingyoupin.top/gtookgngej.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.316326.xyz/gtldyslgwv.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gtakzphgqx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtatfkujhn.html

================================================================================
来源：http://hz.52xcode.cn/gtcimarojx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtxacgpgkj.html

================================================================================
来源：http://hz.hfpthk.cn/gtumrttuxe.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gthwoeaugc.html

println("Hello")
来源：http://hz.daxiang520.top/gthlzfrnnw.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gtzwhpvfkf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtwmekcsuf.html

[T03] Kotlin：字符串模板
来源：http://hz.ywan-chungtsiang.top/gtfwvtqgid.html

"值: $b"
来源：http://hz.redwolf501.top/gtispdotpm.html

[T04] Kotlin：空安全
来源：http://hz.yueranfly.top/gtflkxsxab.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gtfroclayx.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gtsfkpvmbi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tian-w.cn/gtcbolzqwi.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gtahnegaai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtobtffdzi.html

[T07] Kotlin：集合过滤
来源：http://hz.jyoumei.cn/gtxduxvwos.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yonumen.top/gtwnxkaylr.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtdelgvero.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtktdydduj.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gtupcgzuei.html

fun String.exclaim() = this + "!"
来源：http://hz.zhixingplan.top/gtuxdoyuel.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gttjqoeane.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtholgnbdn.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtcdncelqe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daria6918.cn/gtcyvvpbio.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtalielkeo.html

val (a, b) = Pair(1, 2)
来源：http://hz.vqdsnc.cn/gtyxquqzth.html

[T13] Kotlin：只读 Map
来源：http://hz.tian-w.cn/gtdrmfvthh.html

val m = mapOf("a" to 1)
来源：http://hz.hywenlv.cn/gtjqzdnyel.html

[T14] Kotlin：循环
来源：http://hz.yuanzhike.top/gtccambtjm.html

for (i in 1..10) println(i)
来源：http://hz.zdqjudy.top/gtdufpffkl.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangkeji.top/gtrrketsay.html

interface Shape { fun area(): Double }
来源：http://hz.jinghuilouyu.cn/gttlcesqll.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gtwqgctbjv.html

print("Hello")
来源：http://hz.sweek.top/gtutpgdnpu.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtxoujmjxv.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gtkykqjnnz.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtgusfkjlk.html

"值: \(b)"
来源：http://hz.xuanzx.com/gteemxawgt.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtodfsuuyx.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gthkmndeti.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtekhwlyeg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gtsdeahzig.html

[T21] Swift：遍历
来源：http://hz.vqdsnc.cn/gtdotqoqrl.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtynrswdby.html

[T22] Swift：字典
来源：http://hz.sysykeji.top/gtgbguqlap.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtuikenlgv.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtfunyotmc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cheryme.top/gthemvagkd.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtsovzjekr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenzaomai.com/gtjbsoeosq.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtrdtacake.html

struct P { var x: Int }
来源：http://hz.shanyushiyangkeji.top/gtyenqzkqk.html

[T26] Swift：类与重写
来源：http://hz.hammf.cn/gtghxufdjw.html

class A: Base { override func f() {} }
来源：http://hz.cheryme.top/gtjaltgsrk.html

[T27] Swift：错误处理
来源：http://hz.nwbrower.top/gtgpdbewtj.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gttueegqdl.html

[T28] Swift：枚举
来源：http://hz.smart0.xyz/gtjidsxifn.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtlhlfmbaq.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gtdpnbtofw.html

guard let x = opt else { return }
来源：http://hz.jinqigufen.top/gtbqfqjono.html

[T30] Swift：协议
来源：http://hz.zhiwuduotai.top/gtlwjpxotn.html

protocol Shape { func area() -> Double }
来源：http://hz.cashguo.top/gtwmiksngj.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gthrzhjxty.html

print("Hello")
来源：http://hz.tian-w.cn/gtepqjnbhx.html

[T32] Lua：局部变量
来源：http://hz.vqdsnc.cn/gtxtvtjiza.html

local a = 1
来源：http://hz.gzhubu.top/gtnxmdnaof.html

[T33] Lua：表（数组）
来源：http://hz.chenlongwang.top/gtjlcsqktm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xingfuxueyuan.xyz/gtxavbdnnm.html

[T34] Lua：遍历表
来源：http://hz.hywenlv.cn/gtmgphhcgx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtnpmwuynj.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gthqkmnnrm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinghuilouyu.cn/gtbhcoiude.html

[T36] Lua：函数
来源：http://hz.gogol.net.cn/gtvntybclw.html

function add(a, b) return a + b end
来源：http://hz.aibaodan.cn/gtuctvzelf.html

[T37] Lua：字符串拼接
来源：http://hz.yanxiufei.cn/gtouvdkknh.html

"a" .. "b"
来源：http://hz.tian-w.cn/gtvvingpvj.html

[T38] Lua：条件
来源：http://hz.meibo888.top/gtaogfvtuu.html

if x > 0 then print("正") end
来源：http://hz.birdmap.top/gtbpiadjfj.html

[T39] Lua：模式匹配
来源：http://hz.yongpay.top/gtpdnbfbng.html

string.find(s, "%d+")
来源：http://hz.xziqi.cn/gtqtsfctql.html

[T40] Lua：元表
来源：http://hz.chenzaomai.com/gtjykhtgty.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtthhmazcl.html

[T41] Perl：Hello World
来源：http://hz.wangdashe.top/gtqaksltzi.html

print "Hello\n";
来源：http://hz.ydzc1.top/gthkfqqvlq.html

[T42] Perl：变量类型
来源：http://hz.cucudq.cn/gttjeekazk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtatbeklov.html

[T43] Perl：字符串插值
来源：http://hz.sufxvd.cn/gtxhsbflle.html

"值: $a"
来源：http://hz.jinqigufen.top/gtqxnnowao.html

[T44] Perl：条件
来源：http://hz.zhijiandao.cn/gtsvzuephz.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtdlqtdjqz.html

[T45] Perl：数组遍历
来源：http://hz.dianchejie.cn/gtzgdhfzwu.html

for my $x (@arr) { print $x; }
来源：http://hz.hnxiangtu.top/gtvubyzrha.html

[T46] Perl：哈希操作
来源：http://hz.redwolf501.top/gtortyxzqj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gthqyxefiy.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtdjpnfwry.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jyoumei.cn/gtbswznyhm.html

[T48] Perl：正则替换
来源：http://hz.jyoumei.cn/gtlahdiozw.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtxwwitnwg.html

[T49] Perl：函数
来源：http://hz.aibaodan.cn/gttixsgbaf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guowangkeji.top/gtesblzlpi.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtketpiewa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daxiang520.top/gtuxeuioho.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtwlrpfwif.html

[T51] Scala：Hello World
来源：http://hz.nanxuanxn.top/gtdbqovqjs.html

println("Hello")
来源：http://hz.dashuyun.cn/gtdcemmffa.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtlezulxuq.html

val a = 1;  var b = 2
来源：http://hz.gzhubu.top/gtzosudyvd.html

[T53] Scala：字符串插值
来源：http://hz.ydjk.org.cn/gtshmzrfnk.html

s"值: $b"
来源：http://hz.fzhhl.top/gtafvgszng.html

[T54] Scala：集合映射
来源：http://hz.nanxinkj.top/gtstoohhjv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gtelhrdxjs.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtpghwjxbr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sweek.top/gtwcqrrkas.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gthtukwfim.html

case class User(name: String, age: Int)
来源：http://hz.jinqigufen.top/gtrnirmnbd.html

[T57] Scala：模式匹配
来源：http://hz.c1oappe.top/gtfvbilyha.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigfzy.top/gtqhmvmikv.html

[T58] Scala：函数定义
来源：http://hz.yj20258.top/gtpbpiwcyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ywan-chungtsiang.top/gtmylojkan.html

[T59] Scala：循环
来源：http://hz.jqgufenzy.top/gtklrochkl.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtutymxbex.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangkeji.top/gtjeafofpt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yvedp.cn/gtfolhcuge.html

================================================================================
来源：http://hz.aibaodan.cn/gtphhhvfpe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtewqpftic.html

================================================================================
来源：http://hz.fzhhl.top/gtlxutfsdf.html

[U01] Py：创建虚拟环境
来源：http://hz.quarkkingdee.top/gtvodahzeb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenzaomai.com/gtqiyxqeii.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daxiang520.top/gtipnidrla.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.andypj.xyz/gtlxxvokfq.html

[U03] Py：加载 .env 配置
来源：http://hz.fengsongda.top/gtdwldkxsa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangdashe.top/gtlaypzxbo.html

[U04] Py：变量调试打印
来源：http://hz.chenjidiqi.icu/gtfflwzgfk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guowangkeji.top/gtkafdgorn.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtactmtswp.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangkeji.top/gtpxtymjkq.html

[U06] Py：合并两个字典
来源：http://hz.svipenyu.cn/gtwrqbirez.html

{**a, **b}
来源：http://hz.sysykeji.top/gtvylwnxmz.html

[U07] Py：反转字典键值
来源：http://hz.yuanzhike.top/gtgepoxaae.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gtjqlsnjkk.html

[U08] Py：展平二维列表
来源：http://hz.smart0.xyz/gtuwfjrkmr.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtouhqcsmu.html

[U09] Py：字典取最大值的键
来源：http://hz.9152youxi.cn/gtltbrtktm.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtmdkawryh.html

[U10] Py：按值排序字典
来源：http://hz.dashuyun.cn/gtbxtcajxu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.bjfxy.top/gtxnzullij.html

[U11] Py：生成器表达式
来源：http://hz.shuidangran.top/gtqtqvsgsm.html

(x * 2 for x in arr)
来源：http://hz.yj202588.top/gtyuakrjtl.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sxryk.cn/gtofdlzcmz.html

Counter(arr).most_common(3)
来源：http://hz.ydzc1.top/gtcqstsbtv.html

[U13] Py：固定长度队列
来源：http://hz.ppjwa.cn/gtbzixmlwq.html

deque(maxlen=10)
来源：http://hz.cashguo.top/gttnhkvdki.html

[U14] Py：分组收集到列表
来源：http://hz.haohaochexian.top/gtculcbmur.html

defaultdict(list)
来源：http://hz.cheryme.top/gtuztxmoui.html

[U15] Py：高精度计时
来源：http://hz.quarkkingdee.top/gtaqixtlfx.html

t = time.perf_counter()
来源：http://hz.pycfn.com/gtnbzusmpn.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gtqugtrevv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.guannengcc.top/gtjogcffbu.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gtsouqkrkt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtmcjkvscf.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtucijhvns.html

pat = re.compile(r"\d+")
来源：http://hz.andypj.xyz/gtttpjzhmi.html

[U19] Py：正则替换带回调
来源：http://hz.xingfuxueyuan.xyz/gtwrslduey.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jianghu66.top/gtxzkyizdq.html

[U20] Py：缓存函数结果
来源：http://hz.jinghuilouyu.cn/gtjnmluqqh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jianghu66.top/gtxjlbcwzn.html

[U21] Py：自定义上下文管理器
来源：http://hz.feifeiyinyue.top/gtmetrvhyh.html

@contextlib.contextmanager
来源：http://hz.ydjk.org.cn/gtnjgujgde.html

[U22] Py：矩阵转置
来源：http://hz.quarkkingdee.top/gtbwcwvmbd.html

list(zip(*m))
来源：http://hz.ydjk.org.cn/gtkaxonkvp.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtjtleghkc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jlsjyb.cn/gtvictnwex.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangtech.top/gtmmqpferk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtfwhuhbiq.html


<!-- 参考信息 -->