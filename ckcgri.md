代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtquxodwkg.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gtbqruncom.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gttyrgzwyg.html

[S24] C：获取本地时间
来源：http://hz.nwbrower.top/gtxylhgppb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtbwupzgla.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtfwpgfxov.html

memcpy(dst, src, n);
来源：http://hz.wangshuangyany.cn/gtnktygzha.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gttxieecsj.html

memset(a, 0, sizeof a);
来源：http://hz.52xcode.cn/gtqtdosshq.html

[S27] C：定义常量
来源：http://hz.yuxming.cn/gtcvqkyryp.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtnasfynpi.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gtfeuzbruf.html

static int counter = 0;
来源：http://hz.yj202588.top/gtpvyupyxx.html

[S29] C：变参函数
来源：http://hz.hfpthk.cn/gtevlwrhaw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhoulong.xyz/gtmogndfan.html

[S30] C：头文件保护
来源：http://hz.guannengcc.top/gtxundczdf.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gtxohdbshn.html

#define X_H
来源：http://hz.hammf.cn/gtmnpmgycf.html

#endif
来源：http://hz.daxiang520.top/gtpblhtpxt.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtadbbipty.html

#include <iostream>
来源：http://hz.yvedp.cn/gtsuwxrzdz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gttmpfgtyl.html

[S32] C++：字符串
来源：http://hz.xziqi.cn/gtealhuxcr.html

std::string s = "hi";  s += "!";
来源：http://hz.andypj.xyz/gtasvunfdr.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtzaafzoea.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtawyekrlp.html

[S34] C++：遍历 vector
来源：http://hz.daxiang520.top/gtdrccjsqw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtgthezusi.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gtjlxtitmx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gthoxogskb.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtzopdptxc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtzptxunjg.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtuwyarbff.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.svipenyu.cn/gtwaiuzqxc.html

[S38] C++：排序
来源：http://hz.xingfuxueyuan.xyz/gtxoroyqjt.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gtfyysdzri.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtoddcvfte.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ywan-chungtsiang.top/gtpeguccrm.html

[S40] C++：查找元素
来源：http://hz.xuetiantiany.cn/gtzcrqaimh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtmrfnbkhy.html

[S41] C++：类与构造函数
来源：http://hz.daria6918.cn/gtwtsjzjon.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtmjkfblps.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gtxtbaafem.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtlgabjjev.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtpnukobuy.html

auto p = std::make_unique<int>(5);
来源：http://hz.cucudq.cn/gtuiqiwzmi.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtretxbigl.html

void inc(int &x) { ++x; }
来源：http://hz.yj20258888.top/gtmjgapjxd.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtupzgxbin.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gotoacloud.top/gtssoruhen.html

[S46] C++：函数模板
来源：http://hz.birdmap.top/gtxkurczau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtdcezrtrz.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhaomingkeji.xyz/gtzgiwugfp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtfdvykjjz.html

[S48] C++：逐行读文件
来源：http://hz.ivvv.top/gtdbrirfpk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnxiangtu.top/gtiocskuqx.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtmufghvsr.html

[S49] C++：写文件
来源：http://hz.zhongyouzk.top/gtayghegbw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtlpglypyg.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtoicfqvok.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.52xcode.cn/gtlmsprtqc.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtjiuvzwbk.html

static_cast<double>(a) / b
来源：http://hz.yj20258888.top/gthfntmbon.html

[S52] C++：const 与 noexcept
来源：http://hz.yonumen.top/gtwqsxofdx.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtvttwcegy.html

[S53] C++：移动语义
来源：http://hz.zdqjudy.top/gtbhssafnv.html

std::vector<int> w = std::move(v);
来源：http://hz.pycfn.com/gtzotajcxi.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gtuislhzit.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtizcujewe.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtxvkekcau.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuanzhike.top/gtkblfrwjy.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtoazlikuf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtcuqglzxn.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtkxdoeyyi.html

constexpr int N = 10;
来源：http://hz.snrcjt.cn/gtuheanpgp.html

[S58] C++：命名空间
来源：http://hz.xuanzx.com/gtxhtmysdv.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtgpdcqgzy.html

[S59] C++：静态断言
来源：http://hz.andypj.xyz/gtlcuckbls.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gteztinmvb.html

[S60] C++：遍历并删除元素
来源：http://hz.jianghu66.top/gtnlxoytyc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtpsmrnfgz.html

================================================================================
来源：http://hz.tanke756.top/gtltrxacsy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtlhqqfwxc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgbqgajsu.html

[T01] Kotlin：Hello World
来源：http://hz.nanxinkj.top/gtxgflsypc.html

println("Hello")
来源：http://hz.jinqigufen.top/gthsxjioye.html

[T02] Kotlin：变量
来源：http://hz.andypj.xyz/gtmwfgfylf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtvpyxkxew.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtdsfgctfr.html

"值: $b"
来源：http://hz.haohaochexian.top/gtmeachpqt.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtrtgwljvi.html

val n: String? = null;  n?.length
来源：http://hz.jiagoushi.top/gtauyosmvb.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtsmbwrtyx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtvqhxiofy.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gtkdryazbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sweek.top/gtmdxybfre.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtnruipnxc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhiwuduotai.top/gtzzncgkqk.html

[T08] Kotlin：数据类
来源：http://hz.jyoumei.cn/gtlydmxprp.html

data class User(val name: String, val age: Int)
来源：http://hz.xuetiantiany.cn/gtmlgytexo.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtfnzfibsh.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtwqkrryrt.html

[T10] Kotlin：默认参数
来源：http://hz.sysykeji.top/gtcopgkgcq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtisnjdgbx.html

[T11] Kotlin：协程
来源：http://hz.zycfv.cn/gtlodzgyfq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtdmgvfeip.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gtqcqqcldc.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtwxvwlzlf.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gtgkexmpuq.html

val m = mapOf("a" to 1)
来源：http://hz.nwbrower.top/gtidtmzgqj.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtzkmtzpxx.html

for (i in 1..10) println(i)
来源：http://hz.quarkkingdee.top/gtkqoljjkq.html

[T15] Kotlin：接口
来源：http://hz.tianlin.xyz/gtilkrcsdd.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtdhajqios.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtxkazvbcx.html

print("Hello")
来源：http://hz.yueranfly.top/gtgjgimvup.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtfpbfgqtr.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gtnvdvkqma.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtxifoiwjb.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gtdlgxogqq.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gtsiipdqbv.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtbdwukhpn.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gtvpixhpin.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtturysmiw.html

[T21] Swift：遍历
来源：http://hz.mhx1999.top/gtvuuxpxxf.html

for x in a { print(x) }
来源：http://hz.hnxiangtu.top/gtxvmjspfm.html

[T22] Swift：字典
来源：http://hz.xingfuxueyuan.xyz/gtqshjtfgx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.havefunace.top/gtuzaxmgpa.html

[T23] Swift：函数
来源：http://hz.sysykeji.top/gthsalcssy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nwbrower.top/gtgvtwwqrk.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtmweozabi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daxiang520.top/gtzgztsgzb.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtukreckpx.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtojlfndkj.html

[T26] Swift：类与重写
来源：http://hz.yuxming.cn/gtkfelihye.html

class A: Base { override func f() {} }
来源：http://hz.yuanzhike.top/gtisabpfbp.html

[T27] Swift：错误处理
来源：http://hz.chenzaomai.com/gtdupcctfd.html

do { try f() } catch { print(error) }
来源：http://hz.9152youxi.cn/gtxwgywlhd.html

[T28] Swift：枚举
来源：http://hz.jianghu66.top/gtuiptpnqu.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtoaiiovrx.html

[T29] Swift：guard 提前返回
来源：http://hz.yvedp.cn/gtdxptpcav.html

guard let x = opt else { return }
来源：http://hz.jianghu66.top/gtjwpkoadz.html

[T30] Swift：协议
来源：http://hz.ybcxt.top/gtqprtrbcl.html

protocol Shape { func area() -> Double }
来源：http://hz.nwbrower.top/gtckjbefsh.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gtsztoulzu.html

print("Hello")
来源：http://hz.xylfe.cn/gtopmycozv.html

[T32] Lua：局部变量
来源：http://hz.chenzaomai.com/gtxivxsrhf.html

local a = 1
来源：http://hz.zycfv.cn/gtlyptlemq.html

[T33] Lua：表（数组）
来源：http://hz.jinqigfzy.top/gtmtcufgiw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gtgpggysub.html

[T34] Lua：遍历表
来源：http://hz.iojbl.cn/gteikvaayg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guannengcc.top/gtwspicxog.html

[T35] Lua：字典表
来源：http://hz.jinqigfzy.top/gtftzakeeg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gtntfzwbco.html

[T36] Lua：函数
来源：http://hz.9152youxi.cn/gtkbliictm.html

function add(a, b) return a + b end
来源：http://hz.hysaishi.cn/gtvkgsfawm.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtleobutyz.html

"a" .. "b"
来源：http://hz.cdnleiting.top/gtrhjdxhds.html

[T38] Lua：条件
来源：http://hz.snrcjt.cn/gtpkpvylsq.html

if x > 0 then print("正") end
来源：http://hz.yanxiufei.cn/gtlnyzshfl.html

[T39] Lua：模式匹配
来源：http://hz.fzhhl.top/gthtpmpkrr.html

string.find(s, "%d+")
来源：http://hz.bjfxy.top/gthhrgnupi.html

[T40] Lua：元表
来源：http://hz.meibo888.top/gtomucnojp.html

setmetatable({}, { __index = base })
来源：http://hz.52xcode.cn/gtjkirwqcs.html

[T41] Perl：Hello World
来源：http://hz.zhixingplan.top/gtuhqnphlt.html

print "Hello\n";
来源：http://hz.gzhubu.top/gttgreikud.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtzmulrhjn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yangfankeji.com/gtyyigwzfd.html

[T43] Perl：字符串插值
来源：http://hz.jyoumei.cn/gtisakikfi.html

"值: $a"
来源：http://hz.nanxuanxn.top/gtilhmpnzm.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtvlwusiki.html

if ($a > 0) { print "正"; }
来源：http://hz.tianlin.xyz/gtbxshulmd.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtvgijfhlh.html

for my $x (@arr) { print $x; }
来源：http://hz.snrcjt.cn/gteivdjlvl.html

[T46] Perl：哈希操作
来源：http://hz.yuanzhike.top/gtoqdgevjz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuanzx.com/gtllkgbnag.html

[T47] Perl：正则捕获
来源：http://hz.jlsjyb.cn/gtjrdjbizp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gtiylkgknr.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gtobfahmzq.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtcfhoupxq.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gtlxtveftn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xinyue.icu/gtgcdhutjv.html

[T50] Perl：逐行读文件
来源：http://hz.zycfv.cn/gtvfucvaaw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nwbrower.top/gtaxkkbdsv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhijiandao.cn/gtxuprnwoa.html

[T51] Scala：Hello World
来源：http://hz.gaohongyu789.top/gtrtgtlcfe.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtvzyomwjr.html

[T52] Scala：变量
来源：http://hz.ydzc1.top/gtbqhlfmvh.html

val a = 1;  var b = 2
来源：http://hz.nwbrower.top/gtfszhbypi.html

[T53] Scala：字符串插值
来源：http://hz.snrcjt.cn/gtixbsztmr.html

s"值: $b"
来源：http://hz.jlsjyb.cn/gtmzoydufz.html

[T54] Scala：集合映射
来源：http://hz.gogol.net.cn/gtkokpclum.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtsvalbzel.html

[T55] Scala：集合过滤
来源：http://hz.gzhubu.top/gthcugywzv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ppjwa.cn/gtiyidurer.html

[T56] Scala：样例类
来源：http://hz.yonumen.top/gttscionvq.html

case class User(name: String, age: Int)
来源：http://hz.quarkkingdee.top/gtybyizfwi.html

[T57] Scala：模式匹配
来源：http://hz.birdmap.top/gtxfjcplwf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zdqjudy.top/gtmqfdzowl.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtbqlsytsh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daria6918.cn/gtdburrzpe.html

[T59] Scala：循环
来源：http://hz.zhoulong.xyz/gtldebjsqm.html

for (i <- 1 to 10) println(i)
来源：http://hz.gzhubu.top/gtvblgsppd.html

[T60] Scala：折叠
来源：http://hz.gzhubu.top/gtidjajdys.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtnrnmnhai.html

================================================================================
来源：http://hz.jiagoushi.top/gtguzrvaby.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtcsdkenbq.html

================================================================================
来源：http://hz.hnqzz.top/gtgpcwshve.html

[U01] Py：创建虚拟环境
来源：http://hz.andypj.xyz/gteizhxxyc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.redwolf501.top/gtdlessjxd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zycfv.cn/gtkpikudkv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.wangshuangyany.cn/gtvbcefvbr.html

[U03] Py：加载 .env 配置
来源：http://hz.xuetiantiany.cn/gtpuzcxspm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.mhx1999.top/gtzenorypp.html

[U04] Py：变量调试打印
来源：http://hz.yuanzhike.top/gtjcvwzsxo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hammf.cn/gtzqkdhdxe.html

[U05] Py：列表去重且保序
来源：http://hz.jinghuilouyu.cn/gttmclusdq.html

list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtdgtyaung.html

[U06] Py：合并两个字典
来源：http://hz.feifeiyinyue.top/gtqodoimaw.html

{**a, **b}
来源：http://hz.iojbl.cn/gtxpmnqdbi.html

[U07] Py：反转字典键值
来源：http://hz.zhengqikj.top/gthtcxtokh.html

{v: k for k, v in d.items()}
来源：http://hz.shzxlz.cn/gtneufqjom.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtnghgxbra.html

[y for x in nested for y in x]
来源：http://hz.mhx1999.top/gtgginbpfk.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtqgkxnwnw.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtdmdegxiy.html

[U10] Py：按值排序字典
来源：http://hz.chenzaomai.com/gtngoftitu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sysykeji.top/gtnoypabmv.html

[U11] Py：生成器表达式
来源：http://hz.cucudq.cn/gtiousblxd.html

(x * 2 for x in arr)
来源：http://hz.ydzc1.top/gtoyqanuce.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnqzz.top/gtcxscaewn.html

Counter(arr).most_common(3)
来源：http://hz.feifeiyinyue.top/gtzlhpzzsn.html

[U13] Py：固定长度队列
来源：http://hz.fengsongda.top/gtsqcvtgst.html

deque(maxlen=10)
来源：http://hz.quarkkingdee.top/gtkrdkuczt.html

[U14] Py：分组收集到列表
来源：http://hz.kuanghao11.cn/gtdrdduqsq.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtvzupblak.html

[U15] Py：高精度计时
来源：http://hz.chenjidiqi.icu/gtvqermoqw.html

t = time.perf_counter()
来源：http://hz.yonumen.top/gtujhsglxb.html

[U16] Py：命令行参数解析
来源：http://hz.hywenlv.cn/gtszuqknot.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuanzx.com/gtserjixfy.html

[U17] Py：初始化日志
来源：http://hz.mhx1999.top/gtivzfuiiq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gtdaixjxvs.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtfbmoabdx.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gtneahwvgw.html

[U19] Py：正则替换带回调
来源：http://hz.xingfuxueyuan.xyz/gtprhcsjnb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtfliutsfu.html

[U20] Py：缓存函数结果
来源：http://hz.316326.xyz/gtwaopdtxe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yanxiufei.cn/gtlzypfygy.html

[U21] Py：自定义上下文管理器
来源：http://hz.guannengcc.top/gthknmfxjz.html

@contextlib.contextmanager
来源：http://hz.quarkkingdee.top/gtqfnlspok.html

[U22] Py：矩阵转置
来源：http://hz.snrcjt.cn/gtlpnqbmxp.html

list(zip(*m))
来源：http://hz.jiagoushi.top/gtaogfnxxf.html

[U23] Py：分块读取大文件
来源：http://hz.jqgufenzy.top/gtaeoxdkky.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tianlin.xyz/gtepxrlxka.html

[U24] Py：路径操作
来源：http://hz.havefunace.top/gtxfslnems.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cdnleiting.top/gtdcbiwzdm.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258.top/gtebljrsph.html

csv.DictReader(f)
来源：http://hz.bjfxy.top/gtgrrbnsdy.html

[U26] Py：并发下载
来源：http://hz.vqdsnc.cn/gtampjirol.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.wangdashe.top/gtzgigqsin.html

[U27] Py：异步 HTTP
来源：http://hz.andypj.xyz/gtshpsvycp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yvedp.cn/gtasbkobhq.html

[U28] Py：类型别名
来源：http://hz.ehwqpu.com/gtonyrnaui.html

UserId = int
来源：http://hz.aizwys.cn/gtcggsnriz.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtaglbawvn.html

@property 与 @x.setter 配合
来源：http://hz.gogol.net.cn/gthlisxacu.html

[U30] Py：数据类
来源：http://hz.0kj1m.cn/gtqsqwuglq.html

@dataclass(slots=True)
来源：http://hz.fengsongda.top/gtoinwqfsj.html

[U31] Py：单测
来源：http://hz.hongshengwenyu.top/gtwuhulspd.html

python -m pytest -q
来源：http://hz.9152youxi.cn/gttcjohqvl.html

[U32] Py：代码格式化
来源：http://hz.shuidangran.top/gtqfsdsxdv.html

ruff format . && ruff check --fix .
来源：http://hz.hammf.cn/gtnpthzqed.html

[U33] Py：打包发布
来源：http://hz.hywenlv.cn/gtfiddmkkn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.guowangkeji.top/gtjiocgzko.html

[U34] Py：判断编码
来源：http://hz.wangdashe.top/gtghtfkwic.html

chardet.detect(raw)
来源：http://hz.daxiang520.top/gtoanzilno.html

[U35] Py：发送邮件
来源：http://hz.ybcxt.top/gtlytorkvp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xinyue.icu/gtzpswkgpr.html

[U36] Py：定时任务
来源：http://hz.mhx1999.top/gtvkifcmbc.html

schedule.every(10).minutes.do(job)
来源：http://hz.snrcjt.cn/gtvnkjbpsc.html

[U37] Py：读写 Excel
来源：http://hz.hysaishi.cn/gtcwqgxwqq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.quarkkingdee.top/gtwkiqkhwc.html

[U38] Py：获取脚本所在目录
来源：http://hz.316326.xyz/gtarivcouq.html

Path(__file__).resolve().parent
来源：http://hz.jqgufenzy.top/gttmllebxw.html

[U39] Py：判断是否在交互环境
来源：http://hz.xylfe.cn/gtuwvongei.html

sys.stdout.isatty()
来源：http://hz.andypj.xyz/gtwmxodjiq.html

[U40] Py：打印到标准错误
来源：http://hz.chenzaomai.com/gtiixjggpa.html

print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtrtadrmif.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xziqi.cn/gttwnnbpff.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tian-w.cn/gtjudqpkqs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hongshengwenyu.top/gttyrzoena.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gaohongyu789.top/gtyqyqdoye.html

[U43] PHP：声明命名空间
来源：http://hz.yonumen.top/gtbsjfblpd.html

namespace App\Http;
来源：http://hz.xziqi.cn/gtdmeeddgd.html

[U44] PHP：开启严格类型
来源：http://hz.hammf.cn/gtyloctdce.html

declare(strict_types=1);
来源：http://hz.yueranfly.top/gtzjdwkinr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tianlin.xyz/gtxywyhyre.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtbfhzsdbr.html

[U46] PHP：可空类型
来源：http://hz.zdqjudy.top/gtqhflvxql.html

?string $name = null
来源：http://hz.zhongyouzk.top/gtwuntjpjj.html


<!-- 参考信息 -->