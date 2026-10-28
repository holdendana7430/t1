代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtzhdlayzn.html

[S21] C：字符类别判断
来源：http://hz.chenlongwang.top/gtjiaajrgh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gotoacloud.top/gtzpcicmpo.html

[S22] C：字符串转数字
来源：http://hz.xuanzx.com/gthqolmisg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtrtwwsxpa.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gthfjvcewh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuetiantiany.cn/gticybhyjk.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtkxobwfbu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.birdmap.top/gtpbafwuic.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gtifldecjr.html

memcpy(dst, src, n);
来源：http://hz.yanxiufei.cn/gtfwqkxhai.html

[S26] C：内存清零
来源：http://hz.tanke756.top/gtkasofxtt.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtrunhztmx.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtathoqwne.html

const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gtgxrfrwmg.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtiklpbfir.html

static int counter = 0;
来源：http://hz.redwolf501.top/gtuhnqmawq.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gthezqlkva.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtqwuxyhql.html

[S30] C：头文件保护
来源：http://hz.yj20258888.top/gtvifbclzk.html

#ifndef X_H
来源：http://hz.hongshengwenyu.top/gttjbzjqut.html

#define X_H
来源：http://hz.aibaodan.cn/gtwajnlspq.html

#endif
来源：http://hz.yongpay.top/gtcilvbebg.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtiydtgakh.html

#include <iostream>
来源：http://hz.yvedp.cn/gtthoihwhp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gthnnenzcj.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtcwrqmapo.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtqsuyytzf.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtgubcmyxl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtoofxjblc.html

[S34] C++：遍历 vector
来源：http://hz.chenzaomai.com/gtkqluccft.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gthvhwivbp.html

[S35] C++：map
来源：http://hz.ybcxt.top/gtupufutgv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtzzkxsabq.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtaibvidwg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtkqinqtnh.html

[S37] C++：set
来源：http://hz.ydjk.org.cn/gtmvwmbcus.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtgggcofco.html

[S38] C++：排序
来源：http://hz.shangyingyoupin.top/gtrncbfbgw.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtyvnohhgl.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtndbptohf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtjlghsztc.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtetdlcixd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ivvv.top/gtyhdbfiyq.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gthrpthtnf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tianlin.xyz/gtzispieot.html

[S42] C++：继承与虚函数
来源：http://hz.hywenlv.cn/gtgvwpnysp.html

class B : public Base { public: void f() override {} };
来源：http://hz.dashuyun.cn/gtqqktqbqz.html

[S43] C++：智能指针
来源：http://hz.svipenyu.cn/gtlndoiqtq.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtiioficlp.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtyffqxzuw.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtkxwpnnnc.html

[S45] C++：lambda
来源：http://hz.guowangkeji.top/gtlgrxadal.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258.top/gtqdmdfgob.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gttxuggrso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guannengcc.top/gtgkbzaaqi.html

[S47] C++：结构化绑定遍历
来源：http://hz.zycfv.cn/gtmskeyjpv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtpyepihby.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gtlbrpevjz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtqcsavhjc.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtsxazaeae.html

[S49] C++：写文件
来源：http://hz.dashuyun.cn/gtygjbjafb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.smart0.xyz/gtwupcncin.html

[S50] C++：格式化数字
来源：http://hz.ydjk.org.cn/gtznoduyfi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.9152youxi.cn/gtlwlmzete.html

[S51] C++：显式类型转换
来源：http://hz.feifeiyinyue.top/gtjqmoqckc.html

static_cast<double>(a) / b
来源：http://hz.xuetiantiany.cn/gtpnfvrkei.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtztpdvwgg.html

int size() const noexcept { return n_; }
来源：http://hz.sufxvd.cn/gtbvpknobx.html

[S53] C++：移动语义
来源：http://hz.pycfn.com/gtumjuvfwj.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtckpqazix.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gthvmfozea.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtfmzjqxxa.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtigfxfvna.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cqqwz.cn/gtkxngeoju.html

[S56] C++：optional
来源：http://hz.haohaochexian.top/gtcppigokw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.kuanghao11.cn/gtlrygllvo.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gtacegbmye.html

constexpr int N = 10;
来源：http://hz.snrcjt.cn/gtcjprufoj.html

[S58] C++：命名空间
来源：http://hz.ybcxt.top/gtmrqjkdth.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangshuangyany.cn/gtzmurwcva.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtlhwcbjvh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtakszeqfu.html

[S60] C++：遍历并删除元素
来源：http://hz.xylfe.cn/gtnwszagth.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtjmxerald.html

================================================================================
来源：http://hz.sufxvd.cn/gtgveqfgia.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtepatfmol.html

================================================================================
来源：http://hz.birdmap.top/gthftqmgrp.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtznbmnqti.html

println("Hello")
来源：http://hz.nwbrower.top/gtwxnetorp.html

[T02] Kotlin：变量
来源：http://hz.jlsjyb.cn/gtlncrzyqb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtrswknzzj.html

[T03] Kotlin：字符串模板
来源：http://hz.zhiwuduotai.top/gtakontpgw.html

"值: $b"
来源：http://hz.smart0.xyz/gtmzxaobnd.html

[T04] Kotlin：空安全
来源：http://hz.jiagoushi.top/gtahvshmqy.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtrtbzoibt.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gtkudlqlvr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuetiantiany.cn/gtmssmbmit.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gthofajugj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigufen.top/gtuvrurmle.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtpsjkercz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangdashe.top/gtzfgazmkn.html

[T08] Kotlin：数据类
来源：http://hz.wangshuangyany.cn/gtpdexgkaj.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtivegawpk.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgfzy.top/gthbwnpemu.html

fun String.exclaim() = this + "!"
来源：http://hz.quarkkingdee.top/gtrucgdnck.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtqzicmvlw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtumydtksj.html

[T11] Kotlin：协程
来源：http://hz.sweek.top/gtwjpmyotw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenjidiqi.icu/gtmzthzunn.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtziaahyme.html

val (a, b) = Pair(1, 2)
来源：http://hz.quarkkingdee.top/gtqtbfmurt.html

[T13] Kotlin：只读 Map
来源：http://hz.sxryk.cn/gtojxvkzhd.html

val m = mapOf("a" to 1)
来源：http://hz.gotoacloud.top/gtbaqoqxcs.html

[T14] Kotlin：循环
来源：http://hz.hnqzz.top/gtuxjvyofy.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtkhfmjdjk.html

[T15] Kotlin：接口
来源：http://hz.chenjidiqi.icu/gtwkbmxldn.html

interface Shape { fun area(): Double }
来源：http://hz.aibaodan.cn/gtaqgucdne.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtgxxzesrt.html

print("Hello")
来源：http://hz.xinyue.icu/gtmdtmknfi.html

[T17] Swift：变量与常量
来源：http://hz.nanxuanxn.top/gtxoxhvhmn.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gtushirixy.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gttwkufbbh.html

"值: \(b)"
来源：http://hz.yuxming.cn/gtelkuomms.html

[T19] Swift：可选绑定
来源：http://hz.daria6918.cn/gtaeeagvxx.html

if let n = opt { print(n) }
来源：http://hz.zhongyouzk.top/gtmisoapun.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtxpjrigek.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.mhx1999.top/gtqypnbwxl.html

[T21] Swift：遍历
来源：http://hz.hywenlv.cn/gtchglmjdb.html

for x in a { print(x) }
来源：http://hz.mhx1999.top/gtpzknejqo.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtjfiuojvt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sufxvd.cn/gtbrbxfckb.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtzyhznfyx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jlsjyb.cn/gtubobdbdx.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gtcnywijpn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydzc1.top/gteedhykbm.html

[T25] Swift：结构体
来源：http://hz.haohaochexian.top/gtqzlrqdop.html

struct P { var x: Int }
来源：http://hz.chenzaomai.com/gtkvgptmjb.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtsfzjrjjn.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtqnoxqupy.html

[T27] Swift：错误处理
来源：http://hz.aibaodan.cn/gtqdtyqebm.html

do { try f() } catch { print(error) }
来源：http://hz.hysaishi.cn/gtdgrqpcws.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtanpthafu.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gtesehuvcw.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gtgucgboya.html

guard let x = opt else { return }
来源：http://hz.yj202588.top/gtsbwulhdl.html

[T30] Swift：协议
来源：http://hz.chenlongwang.top/gtytqinauj.html

protocol Shape { func area() -> Double }
来源：http://hz.yj20258888.top/gttsvcjlwi.html

[T31] Lua：Hello World
来源：http://hz.gotoacloud.top/gttkpiriga.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtxcrusoix.html

[T32] Lua：局部变量
来源：http://hz.jiagoushi.top/gtvhxtfndl.html

local a = 1
来源：http://hz.sweek.top/gthrgvmfdf.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtxsqgcxxi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtgvezaaig.html

[T34] Lua：遍历表
来源：http://hz.snrcjt.cn/gtpfqydefh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gtnbzhonpu.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtjtxqcvac.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xziqi.cn/gtbdvkteij.html

[T36] Lua：函数
来源：http://hz.ydjk.org.cn/gtyudhydtp.html

function add(a, b) return a + b end
来源：http://hz.yj20258.top/gtrpjtptzf.html

[T37] Lua：字符串拼接
来源：http://hz.ydjk.org.cn/gtyscmmcvs.html

"a" .. "b"
来源：http://hz.svipenyu.cn/gtbvvzhpzs.html

[T38] Lua：条件
来源：http://hz.nwbrower.top/gtclayaakf.html

if x > 0 then print("正") end
来源：http://hz.jinghuilouyu.cn/gtqrkwuprl.html

[T39] Lua：模式匹配
来源：http://hz.nwbrower.top/gtgwvrozse.html

string.find(s, "%d+")
来源：http://hz.yueranfly.top/gtsdejklar.html

[T40] Lua：元表
来源：http://hz.xinyue.icu/gtkcqchobx.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gtswnyeizb.html

[T41] Perl：Hello World
来源：http://hz.52xcode.cn/gtvwiyanki.html

print "Hello\n";
来源：http://hz.cqqwz.cn/gtfewrfihk.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtflskzjxf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aibaodan.cn/gtqjjmucsb.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangtech.top/gtdqrbydqi.html

"值: $a"
来源：http://hz.ywan-chungtsiang.top/gtzmueyqxb.html

[T44] Perl：条件
来源：http://hz.cashguo.top/gtqxavpmwu.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtaibjljml.html

[T45] Perl：数组遍历
来源：http://hz.zhaomingkeji.xyz/gtedqcyluq.html

for my $x (@arr) { print $x; }
来源：http://hz.mhx1999.top/gtbftcsora.html

[T46] Perl：哈希操作
来源：http://hz.pengpengdd.cyou/gtgveesiok.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgfzy.top/gtxrugkbls.html

[T47] Perl：正则捕获
来源：http://hz.meibo888.top/gtkoxjnjuz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hysaishi.cn/gtwcaysirc.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtchoccaax.html

$s =~ s/old/new/g;
来源：http://hz.hysaishi.cn/gtfoeqlpcq.html

[T49] Perl：函数
来源：http://hz.pycfn.com/gtdjlnvbiv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yangfankeji.com/gtnoacyzma.html

[T50] Perl：逐行读文件
来源：http://hz.iojbl.cn/gtiushszyw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhiwuduotai.top/gtkoyjtfcx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.316326.xyz/gtblgumrfl.html

[T51] Scala：Hello World
来源：http://hz.jinyuanbaomall.cn/gtwlgjyxpq.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtvgyhgaru.html

[T52] Scala：变量
来源：http://hz.yonumen.top/gtzpdmxhsk.html

val a = 1;  var b = 2
来源：http://hz.smart0.xyz/gtnfrwgatn.html

[T53] Scala：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtcqxfnvbs.html

s"值: $b"
来源：http://hz.tianlin.xyz/gtiettrhng.html

[T54] Scala：集合映射
来源：http://hz.yangfankeji.com/gtditojyej.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sweek.top/gtlpmnczrc.html

[T55] Scala：集合过滤
来源：http://hz.cdnleiting.top/gtspbdanyw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhaomingkeji.xyz/gtupuombth.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtxucecara.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gtuvtcqice.html

[T57] Scala：模式匹配
来源：http://hz.yanxiufei.cn/gtndoagwxh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gtwiequwvf.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtpztkogju.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhengqikj.top/gtenogrbpy.html

[T59] Scala：循环
来源：http://hz.andypj.xyz/gtvroljfpt.html

for (i <- 1 to 10) println(i)
来源：http://hz.daxiang520.top/gtadhfpboh.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gtpfhbhskm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhaomingkeji.xyz/gtguvximzg.html

================================================================================
来源：http://hz.daxiang520.top/gtlyxijgla.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tianlin.xyz/gtvjuzyhrp.html

================================================================================
来源：http://hz.cdnleiting.top/gtgxafmoxt.html

[U01] Py：创建虚拟环境
来源：http://hz.ybcxt.top/gtpwahogur.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.bjfxy.top/gttahyorag.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinyuanbaomall.cn/gtxstjeqcn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.snrcjt.cn/gtcfrqffzq.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gtqvqmkvyu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtbytssdtf.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gtaasrcldk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhijiandao.cn/gtdxeublga.html

[U05] Py：列表去重且保序
来源：http://hz.cdnleiting.top/gtrcbtjzkt.html

list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtkuzlabgh.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtzfdrwlcs.html

{**a, **b}
来源：http://hz.xinyue.icu/gtghueqjpg.html

[U07] Py：反转字典键值
来源：http://hz.zhaomingkeji.xyz/gtnlqwjqas.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtpsqyecbh.html

[U08] Py：展平二维列表
来源：http://hz.smart0.xyz/gtszlbrqtm.html

[y for x in nested for y in x]
来源：http://hz.jyoumei.cn/gtxqqcsvns.html

[U09] Py：字典取最大值的键
来源：http://hz.chenlongwang.top/gtayenndxx.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gtolhhtnoo.html

[U10] Py：按值排序字典
来源：http://hz.zdqjudy.top/gtsgyenhep.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yanxiufei.cn/gtbylzjeva.html

[U11] Py：生成器表达式
来源：http://hz.sweek.top/gtyakthfth.html

(x * 2 for x in arr)
来源：http://hz.cdnleiting.top/gtqziuclwu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dashuyun.cn/gtpqaakosu.html

Counter(arr).most_common(3)
来源：http://hz.shuidangran.top/gtrpsbzize.html

[U13] Py：固定长度队列
来源：http://hz.ppjwa.cn/gtictqdqpp.html

deque(maxlen=10)
来源：http://hz.zhongyouzk.top/gtsvlnyuno.html

[U14] Py：分组收集到列表
来源：http://hz.hongshengwenyu.top/gteofkhnpb.html

defaultdict(list)
来源：http://hz.tanke756.top/gtvicgfltw.html

[U15] Py：高精度计时
来源：http://hz.gotoacloud.top/gtyhlpsbsk.html

t = time.perf_counter()
来源：http://hz.vqdsnc.cn/gtwetouway.html

[U16] Py：命令行参数解析
来源：http://hz.xziqi.cn/gtpbjfzgka.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zdqjudy.top/gtmppulskm.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtsocrbzjl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fzhhl.top/gtakwbyymd.html

[U18] Py：预编译正则
来源：http://hz.yj202588.top/gtsrulxrki.html

pat = re.compile(r"\d+")
来源：http://hz.ydzc1.top/gttilbenrd.html

[U19] Py：正则替换带回调
来源：http://hz.yj20258888.top/gtudrsofep.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ehwqpu.com/gtvqnknwsh.html

[U20] Py：缓存函数结果
来源：http://hz.andypj.xyz/gtfhpqylod.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dianchejie.cn/gtystmibqi.html

[U21] Py：自定义上下文管理器
来源：http://hz.tianlin.xyz/gtklspstai.html

@contextlib.contextmanager
来源：http://hz.nanxuanxn.top/gtrghtqmaz.html

[U22] Py：矩阵转置
来源：http://hz.cashguo.top/gtgdatfmrl.html

list(zip(*m))
来源：http://hz.jlsjyb.cn/gtxzsdofuf.html

[U23] Py：分块读取大文件
来源：http://hz.bjfxy.top/gtdtdpbrft.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hywenlv.cn/gtqozdccwu.html

[U24] Py：路径操作
来源：http://hz.gaohongyu789.top/gtvsqgsieo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydjk.org.cn/gtcveifvaf.html

[U25] Py：CSV 按字典读
来源：http://hz.jiagoushi.top/gtohdtijii.html

csv.DictReader(f)
来源：http://hz.meibo888.top/gttitfvynw.html

[U26] Py：并发下载
来源：http://hz.chenzaomai.com/gttpswsgcj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sweek.top/gtpiqadqfy.html

[U27] Py：异步 HTTP
来源：http://hz.sweek.top/gtllamiqkn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.9152youxi.cn/gtqqyhyzdf.html

[U28] Py：类型别名
来源：http://hz.jinghuilouyu.cn/gtyyrcixec.html

UserId = int
来源：http://hz.gaohongyu789.top/gtsadkcuxz.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtoclcymko.html

@property 与 @x.setter 配合
来源：http://hz.cucudq.cn/gtbkexoqqy.html

[U30] Py：数据类
来源：http://hz.quarkkingdee.top/gtlppuqenq.html

@dataclass(slots=True)
来源：http://hz.xuetiantiany.cn/gtbxptpxhs.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtvfjybcxn.html

python -m pytest -q
来源：http://hz.zhixingplan.top/gtkkxrftvm.html

[U32] Py：代码格式化
来源：http://hz.snrcjt.cn/gtwlzopnpq.html

ruff format . && ruff check --fix .
来源：http://hz.nanxuanxn.top/gtsftxjybx.html

[U33] Py：打包发布
来源：http://hz.jianghu66.top/gtvjmlmxtr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hywenlv.cn/gtnkewlnlo.html

[U34] Py：判断编码
来源：http://hz.shzxlz.cn/gtrfmixbds.html

chardet.detect(raw)
来源：http://hz.jqgfzy.top/gtgfpzzjgr.html

[U35] Py：发送邮件
来源：http://hz.jlsjyb.cn/gtiuoogwnv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yueranfly.top/gtkdxtxejl.html

[U36] Py：定时任务
来源：http://hz.nanxuanxn.top/gtitzwkvmu.html

schedule.every(10).minutes.do(job)
来源：http://hz.yongpay.top/gtrzddfiac.html

[U37] Py：读写 Excel
来源：http://hz.birdmap.top/gttvtmsvcf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhaomingkeji.xyz/gtnourlsnv.html

[U38] Py：获取脚本所在目录
来源：http://hz.nwbrower.top/gtgnvluahn.html

Path(__file__).resolve().parent
来源：http://hz.nwbrower.top/gtnlzratnq.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangshuangyany.cn/gtbpwdgafc.html

sys.stdout.isatty()
来源：http://hz.snrcjt.cn/gtocjgacaa.html

[U40] Py：打印到标准错误
来源：http://hz.chenzaomai.com/gtzlmzqqsb.html

print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gtkvqbiuxx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jqgufenzy.top/gttmnprpit.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yueranfly.top/gtlolghgee.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yanxiufei.cn/gtkvesxqgi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tianlin.xyz/gtyiejrfka.html

[U43] PHP：声明命名空间
来源：http://hz.gaohongyu789.top/gtpmefuxlm.html

namespace App\Http;
来源：http://hz.gzhubu.top/gticwnigsm.html

[U44] PHP：开启严格类型
来源：http://hz.jyoumei.cn/gttrzjmcdt.html

declare(strict_types=1);
来源：http://hz.yj20258888.top/gtavbnhllx.html


<!-- 参考信息 -->