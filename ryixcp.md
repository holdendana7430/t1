代发 wailian999

#ifndef X_H
来源：http://hz.ppjwa.cn/gtejjslask.html

#define X_H
来源：http://hz.zycfv.cn/gteloyptij.html

#endif
来源：http://hz.hnxiangtu.top/gtqvxbopin.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtpqxkwime.html

#include <iostream>
来源：http://hz.sufxvd.cn/gtujnjknok.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xinyue.icu/gtapoctawi.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtmopmfrjl.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtringxucz.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtjobejtpq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cdnleiting.top/gtaomadlgj.html

[S34] C++：遍历 vector
来源：http://hz.daxiang520.top/gtpijprrsb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sufxvd.cn/gtubbjlaru.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtjddbkxmh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gttcaxbavf.html

[S36] C++：unordered_map
来源：http://hz.yj20258888.top/gtjqisayze.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtqlbempli.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtvjimbhog.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gteoilgoea.html

[S38] C++：排序
来源：http://hz.dianchejie.cn/gtwmemiynj.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtxxruaziq.html

[S39] C++：自定义比较器排序
来源：http://hz.feifeiyinyue.top/gtdmgxgqrl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gtktoesinz.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gtqcyztgdk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.redwolf501.top/gthxwqrlts.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtbhywfrjn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yvedp.cn/gtkpucjhxu.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtzwrzllkh.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gthdcmlxss.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtyrwmiaxp.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtvrfgsaxf.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gtholqoxgc.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gtnjgotesi.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtjvecrxjs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.haohaochexian.top/gtkzufzimm.html

[S46] C++：函数模板
来源：http://hz.shangyingyoupin.top/gtmbrqeegf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhongyouzk.top/gtrigticpl.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gthuqgmjaw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtosybuyqg.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtslgsalzb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtkjvfytyp.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtwphteufi.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtxootppwd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtnpyzzmfv.html

[S50] C++：格式化数字
来源：http://hz.jinghuilouyu.cn/gtjnkndpfa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.9152youxi.cn/gtlerdxczt.html

[S51] C++：显式类型转换
来源：http://hz.haohaochexian.top/gtvpwezccy.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtckydoyvh.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtdsribika.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtoyovkjkz.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtkjyawztp.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtukbhzgcv.html

[S54] C++：异常处理
来源：http://hz.nwbrower.top/gtshynrblk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guannengcc.top/gtsenxqpve.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gtetyhxntk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtoexqcbyu.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtdudctmer.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jiagoushi.top/gtxtngbiqz.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtkfygepib.html

constexpr int N = 10;
来源：http://hz.xuetiantiany.cn/gtvwaxelqr.html

[S58] C++：命名空间
来源：http://hz.gzhubu.top/gtgljyibuw.html

namespace ns { int f() { return 1; } }
来源：http://hz.yvedp.cn/gtfbhtyytn.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtsfxezwey.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258.top/gtnwnbykrj.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtafhfhopz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtjkacotey.html

================================================================================
来源：http://hz.cheryme.top/gtoplldkkg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenjidiqi.icu/gtxhfwxipk.html

================================================================================
来源：http://hz.gotoacloud.top/gtihjnbckq.html

[T01] Kotlin：Hello World
来源：http://hz.iojbl.cn/gtylrivcgj.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtlnoupekn.html

[T02] Kotlin：变量
来源：http://hz.jqgufenzy.top/gtwywnebks.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sysykeji.top/gtrknymnpt.html

[T03] Kotlin：字符串模板
来源：http://hz.mhx1999.top/gteqphnbwx.html

"值: $b"
来源：http://hz.yj202588.top/gtmfawkwmp.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtchiawbob.html

val n: String? = null;  n?.length
来源：http://hz.316326.xyz/gtvpwiztbp.html

[T05] Kotlin：when 表达式
来源：http://hz.zhixingplan.top/gteapdjvva.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtxrjtgdtr.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtnifdzbil.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtxbibqmdh.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gtdrsriaed.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtcvimvdqw.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtksismlft.html

data class User(val name: String, val age: Int)
来源：http://hz.shangyingyoupin.top/gtggohtadj.html

[T09] Kotlin：扩展函数
来源：http://hz.yuxming.cn/gtinhsnreq.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtuvolakoq.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtpjypgnun.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ivvv.top/gtgifydsoh.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtwkdqflkj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtyiqrwwli.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtnxuhampm.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtbmpvdnpm.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtzcgseotw.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtfsevualh.html

[T14] Kotlin：循环
来源：http://hz.nanxuanxn.top/gtqzlatzle.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtaboxispy.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtokvhmrak.html

interface Shape { fun area(): Double }
来源：http://hz.sweek.top/gthordeqaf.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gttrogegee.html

print("Hello")
来源：http://hz.dianchejie.cn/gtetegqbrp.html

[T17] Swift：变量与常量
来源：http://hz.ivvv.top/gtibnywunh.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtzcgnolvk.html

[T18] Swift：字符串插值
来源：http://hz.havefunace.top/gtxsczknjb.html

"值: \(b)"
来源：http://hz.kuanghao11.cn/gtddaijlow.html

[T19] Swift：可选绑定
来源：http://hz.nanxinkj.top/gtmlbzyuzo.html

if let n = opt { print(n) }
来源：http://hz.hongshengwenyu.top/gteyoxblec.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtpqjzhgeo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtnwgfbrrn.html

[T21] Swift：遍历
来源：http://hz.hfpthk.cn/gtghkmnwfj.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtlgyjtlkt.html

[T22] Swift：字典
来源：http://hz.yj202588.top/gtsfxoqsel.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.9152youxi.cn/gtydtzvbgg.html

[T23] Swift：函数
来源：http://hz.xylfe.cn/gtmnumaclh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gtdqpdrivn.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gthhpfpzry.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtbgyxmjrf.html

[T25] Swift：结构体
来源：http://hz.bjfxy.top/gtnpwsgqlz.html

struct P { var x: Int }
来源：http://hz.hongshengwenyu.top/gtbnpwbwvi.html

[T26] Swift：类与重写
来源：http://hz.316326.xyz/gthxalstuo.html

class A: Base { override func f() {} }
来源：http://hz.redwolf501.top/gtdhdvvurr.html

[T27] Swift：错误处理
来源：http://hz.tian-w.cn/gtllvwgjmy.html

do { try f() } catch { print(error) }
来源：http://hz.yuanzhike.top/gtmsffnkri.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtekweeltr.html

enum Color { case red, green }
来源：http://hz.316326.xyz/gtyhysqdva.html

[T29] Swift：guard 提前返回
来源：http://hz.9152youxi.cn/gtygsckjhm.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtiykyoddt.html

[T30] Swift：协议
来源：http://hz.yvedp.cn/gtxhxniswr.html

protocol Shape { func area() -> Double }
来源：http://hz.9152youxi.cn/gtdxbbqbkp.html

[T31] Lua：Hello World
来源：http://hz.316326.xyz/gtxwgkovzd.html

print("Hello")
来源：http://hz.vqdsnc.cn/gteetwzgsc.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtqwfwjckj.html

local a = 1
来源：http://hz.chenlongwang.top/gtbtrrbvso.html

[T33] Lua：表（数组）
来源：http://hz.pengpengdd.cyou/gtfmvnqqhe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhiwuduotai.top/gtwbvxwnxz.html

[T34] Lua：遍历表
来源：http://hz.xingfuxueyuan.xyz/gtljiknjcm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.smart0.xyz/gtxkyzlmbz.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtmcieqslz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gtffzgvlma.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtsnytqvwi.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtslaktyok.html

[T37] Lua：字符串拼接
来源：http://hz.meibo888.top/gtnfgztcnh.html

"a" .. "b"
来源：http://hz.ybcxt.top/gtywzlatwc.html

[T38] Lua：条件
来源：http://hz.zhixingplan.top/gtuqqzprog.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtzgcrjjms.html

[T39] Lua：模式匹配
来源：http://hz.cucudq.cn/gtelpzrzvo.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtoucxptnq.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtjymttnea.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtpwqxwdza.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gthyzyoleu.html

print "Hello\n";
来源：http://hz.xingfuxueyuan.xyz/gtkhlwhncf.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtxtxzkjwv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhongyouzk.top/gtcuddlyql.html

[T43] Perl：字符串插值
来源：http://hz.jianghu66.top/gtyheqpbxh.html

"值: $a"
来源：http://hz.tanke756.top/gtyasduydb.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gtdyeyoxtx.html

if ($a > 0) { print "正"; }
来源：http://hz.cheryme.top/gtbalxarqe.html

[T45] Perl：数组遍历
来源：http://hz.havefunace.top/gtbanktaxb.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtaubsqmmu.html

[T46] Perl：哈希操作
来源：http://hz.zhoulong.xyz/gtdvbtbser.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtjnsatisf.html

[T47] Perl：正则捕获
来源：http://hz.xuanzx.com/gtlqlxcqpn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtwquoheer.html

[T48] Perl：正则替换
来源：http://hz.svipenyu.cn/gtedfrmblo.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtifwxfcwc.html

[T49] Perl：函数
来源：http://hz.jinqigufen.top/gtcqrwksjc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtclqwsuel.html

[T50] Perl：逐行读文件
来源：http://hz.tian-w.cn/gtcinltjiu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shanyushiyangkeji.top/gtromchwwq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gtwunfthpq.html

[T51] Scala：Hello World
来源：http://hz.yanxiufei.cn/gtyriqcori.html

println("Hello")
来源：http://hz.yangfankeji.com/gtyagqqfya.html

[T52] Scala：变量
来源：http://hz.andypj.xyz/gtntwblncd.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gtjcfamunt.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtecgzmoqw.html

s"值: $b"
来源：http://hz.hfpthk.cn/gttydsyudf.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtrzkrmsqe.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.pycfn.com/gtpkomrdmg.html

[T55] Scala：集合过滤
来源：http://hz.birdmap.top/gtkeygflpl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtekjiopib.html

[T56] Scala：样例类
来源：http://hz.xuetiantiany.cn/gtrxdhyqfk.html

case class User(name: String, age: Int)
来源：http://hz.jyoumei.cn/gtqerdyykp.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gtefknvugi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yueranfly.top/gtzczwsixt.html

[T58] Scala：函数定义
来源：http://hz.tanke756.top/gthkjxupwy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtbyjzaxvo.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtialviufv.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhongyouzk.top/gtbfolfdse.html

[T60] Scala：折叠
来源：http://hz.ydjk.org.cn/gtnqcbdiih.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ppjwa.cn/gtkmhkobff.html

================================================================================
来源：http://hz.yuanzhike.top/gtmyxlkvkc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sysykeji.top/gtdroncopn.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdypgkrvu.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gttyxpksxh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnqzz.top/gtgiirjxdv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhaomingkeji.xyz/gtwwzmnjvj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xziqi.cn/gtawpyuptd.html

[U03] Py：加载 .env 配置
来源：http://hz.daxiang520.top/gtealjwkvw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gtkbsmqmhf.html

[U04] Py：变量调试打印
来源：http://hz.wangshuangyany.cn/gtszhuvsxw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258.top/gtgweeaswk.html

[U05] Py：列表去重且保序
来源：http://hz.yanxiufei.cn/gtdttscfqe.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtzvgzbxfk.html

[U06] Py：合并两个字典
来源：http://hz.hysaishi.cn/gtezuhhscy.html

{**a, **b}
来源：http://hz.hammf.cn/gtydsnxhkj.html

[U07] Py：反转字典键值
来源：http://hz.cqqwz.cn/gtuqpefbsm.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtmbgshtph.html

[U08] Py：展平二维列表
来源：http://hz.daria6918.cn/gtjselvgid.html

[y for x in nested for y in x]
来源：http://hz.hammf.cn/gtmexwcbjh.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtwvreztpg.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtvvhvbiub.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gtvdjdrfch.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yongpay.top/gtnqvfggzf.html

[U11] Py：生成器表达式
来源：http://hz.cheryme.top/gtmaisymel.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gtofdlnhee.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnxiangtu.top/gtjczxlkjq.html

Counter(arr).most_common(3)
来源：http://hz.bjfxy.top/gtudodxwts.html

[U13] Py：固定长度队列
来源：http://hz.chenzaomai.com/gthrweuany.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gttimibvce.html

[U14] Py：分组收集到列表
来源：http://hz.iojbl.cn/gtbkmptzuz.html

defaultdict(list)
来源：http://hz.cucudq.cn/gtipihrohn.html

[U15] Py：高精度计时
来源：http://hz.fengsongda.top/gtummnjktd.html

t = time.perf_counter()
来源：http://hz.yangfankeji.com/gtnspoyydt.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gthfqwvoml.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinghuilouyu.cn/gtfpijvriz.html

[U17] Py：初始化日志
来源：http://hz.ydzc1.top/gtiuymkagi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgfzy.top/gtsgivvmti.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtxchpfqzl.html

pat = re.compile(r"\d+")
来源：http://hz.kuanghao11.cn/gtkwtrqkgv.html

[U19] Py：正则替换带回调
来源：http://hz.andypj.xyz/gtaceestlt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hywenlv.cn/gtfmbwlasw.html

[U20] Py：缓存函数结果
来源：http://hz.shzxlz.cn/gtudrxfmiw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sxryk.cn/gtfxtsbgws.html

[U21] Py：自定义上下文管理器
来源：http://hz.yongpay.top/gtibbozzto.html

@contextlib.contextmanager
来源：http://hz.jqgufenzy.top/gtbvmzhvfn.html

[U22] Py：矩阵转置
来源：http://hz.smart0.xyz/gtxzcmmutt.html

list(zip(*m))
来源：http://hz.316326.xyz/gtbykmbqzt.html

[U23] Py：分块读取大文件
来源：http://hz.daxiang520.top/gtgoprqoss.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhiwuduotai.top/gtzdxtapre.html

[U24] Py：路径操作
来源：http://hz.zhixingplan.top/gtjvhxskow.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydjk.org.cn/gthigvlyfl.html

[U25] Py：CSV 按字典读
来源：http://hz.yuxming.cn/gtiplxglst.html

csv.DictReader(f)
来源：http://hz.52xcode.cn/gtemmllzel.html

[U26] Py：并发下载
来源：http://hz.tanke756.top/gthwgxeirk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnqzz.top/gtwgpgkmkg.html

[U27] Py：异步 HTTP
来源：http://hz.ywan-chungtsiang.top/gtaxaylzns.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.aizwys.cn/gtnpzsdwbz.html

[U28] Py：类型别名
来源：http://hz.iojbl.cn/gttqygfvxw.html

UserId = int
来源：http://hz.shanyushiyangkeji.top/gtxbxdvhue.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtzoygxbry.html

@property 与 @x.setter 配合
来源：http://hz.ydjk.org.cn/gtlircuwbc.html

[U30] Py：数据类
来源：http://hz.chenlongwang.top/gtbbkobdcz.html

@dataclass(slots=True)
来源：http://hz.gzhubu.top/gtqocjpzls.html

[U31] Py：单测
来源：http://hz.hnqzz.top/gtndpmteoj.html

python -m pytest -q
来源：http://hz.yonumen.top/gtbjsxtzoh.html

[U32] Py：代码格式化
来源：http://hz.hnxiangtu.top/gtlnqtspit.html

ruff format . && ruff check --fix .
来源：http://hz.316326.xyz/gthfrkuedn.html

[U33] Py：打包发布
来源：http://hz.xylfe.cn/gtirwuyfgx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigufen.top/gtpprujtly.html

[U34] Py：判断编码
来源：http://hz.cheryme.top/gtoljmtwzz.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtuifwcrui.html

[U35] Py：发送邮件
来源：http://hz.jqgufenzy.top/gtduqjdgpa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgufenzy.top/gtitaizbrv.html

[U36] Py：定时任务
来源：http://hz.sxryk.cn/gtftkczshs.html

schedule.every(10).minutes.do(job)
来源：http://hz.shzxlz.cn/gtdoisvbtv.html

[U37] Py：读写 Excel
来源：http://hz.cheryme.top/gtnbzdopda.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtskuxsdqj.html

[U38] Py：获取脚本所在目录
来源：http://hz.jiagoushi.top/gtvlpcemmb.html

Path(__file__).resolve().parent
来源：http://hz.316326.xyz/gtndfzdcdj.html

[U39] Py：判断是否在交互环境
来源：http://hz.yj20258.top/gtbqwttpym.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtxgtiaisu.html

[U40] Py：打印到标准错误
来源：http://hz.iojbl.cn/gttxsecbge.html

print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtymbhohlm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.kuanghao11.cn/gtzlskxbma.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.dianchejie.cn/gtjlhkpgwt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.daria6918.cn/gtcxhrucgb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.52xcode.cn/gtdodqqrtg.html

[U43] PHP：声明命名空间
来源：http://hz.haohaochexian.top/gtmuoogwjc.html

namespace App\Http;
来源：http://hz.yongpay.top/gtheacblih.html

[U44] PHP：开启严格类型
来源：http://hz.bjfxy.top/gtndrutmlu.html

declare(strict_types=1);
来源：http://hz.yj20258.top/gtvkwnktul.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hnxiangtu.top/gtjxnffrwq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtniiyywng.html

[U46] PHP：可空类型
来源：http://hz.yongpay.top/gtozbkxgbw.html

?string $name = null
来源：http://hz.yongpay.top/gtkrazfzaw.html

[U47] PHP：联合类型
来源：http://hz.nanxuanxn.top/gtouqmdewb.html

int|string $id
来源：http://hz.quarkkingdee.top/gtsagqcvcs.html

[U48] PHP：纯枚举
来源：http://hz.ehwqpu.com/gtxtisxkva.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tianlin.xyz/gtgzjnjzur.html

[U49] PHP：只读属性
来源：http://hz.haohaochexian.top/gtyltenuyf.html

public readonly string $name
来源：http://hz.sufxvd.cn/gtkslwyzow.html

[U50] PHP：构造器属性提升
来源：http://hz.hnxiangtu.top/gtkrlacisu.html

public function __construct(private int $id) {}
来源：http://hz.svipenyu.cn/gtkjqfkxlr.html

[U51] PHP：数组解构
来源：http://hz.iojbl.cn/gtjwkycfnl.html

[$a, $b] = $arr;
来源：http://hz.mhx1999.top/gtjqsasuis.html

[U52] PHP：箭头函数
来源：http://hz.quarkkingdee.top/gtmqaltinz.html

$double = fn($x) => $x * 2;
来源：http://hz.gaohongyu789.top/gtxgizdaci.html

[U53] PHP：空合并运算符
来源：http://hz.jiagoushi.top/gthpxngiyn.html

$v = $a ?? $b ?? "default";
来源：http://hz.tian-w.cn/gtaflfgbaf.html

[U54] PHP：空安全调用
来源：http://hz.chenzaomai.com/gtvqvsxpxp.html

$obj?->method()
来源：http://hz.dashuyun.cn/gtuifyapet.html


<!-- 参考信息 -->