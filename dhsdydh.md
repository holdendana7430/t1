代发 wailian999

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/goviozhoi.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gigzcyszj.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/grkghzmpf.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gmyxuqadb.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/glrypjmwg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfcljtxb.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gsuqbipxu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/ghbaskdxq.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gvawokuqo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gqkbcvkjs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gpvuxhsdg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/geyxkkmct.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gxgdxciwv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqvtexrqa.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gdlqfjswo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gyqwzolfg.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gruwkayyl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gkeccwefy.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/grsfhwjok.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gapoicgoa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gfrmbqgmc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gilpdobgt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gliyxkhac.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gwajzsdjt.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gooiuiyjw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gpzzqjtbm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gnjodduvd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gwrauvaui.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gfasjplkg.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gxsvdvpji.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/goxpiudqs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gpgasevat.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/ggeijbtfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gmsvvmfax.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gepudlwef.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gxegqjfjo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gqarihura.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gywjscvtf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gykurucot.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/glgcyvvaj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gunsmezfy.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gmkpquomf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gkakjbzts.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gofasvxjf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/garixizrr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gxkotuwzi.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gxutxzcew.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/guygcmmfw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gomepfbbf.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gqzlztyjs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gduaqixso.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gquakrzej.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/guywvciih.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gyjbbkwcr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkavmawcb.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gutcgiphz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/giiwasaxb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gxznwxqsx.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gcsusqscq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gmwqgtzrk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/guqzktpbb.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gulynmasg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gnnvobhhd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdgtzzmmx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gxarfdwkm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gapcxehbz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gbgspujmw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gffltpesi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gorythyrc.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gcyqoeynz.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gacaqgurj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gqgwmfqqs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gofswyzsm.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gxuiaqntz.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gudqnovhm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gxrxmwumd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gkijhgxgx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gshuqyhni.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gtoumjicu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjtvzshkj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gsqhnnqtb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gfkxcaobd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ginnwscuq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/grpcfuegx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gemumpnhh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwhmbrs.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/ghxesrewz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gxzfgjujg.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/ghacjcuee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gvstkdaum.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gtukbosnd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gjixqvwef.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gyzeljhsr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gbpkouwew.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gvovrqbdx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gaehowdxn.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gwineseuz.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gxolwzyoj.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmstdwaxo.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqzbgcirj.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gdcygwolb.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gfrcwjnxg.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gmszcauvr.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gkzubkvgb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gafkbswfb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gljppoczv.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gnsvsqohh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gfqzttrid.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gybanxnxd.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gpqrnzxmv.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gqfjafott.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gnkhmlris.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/genanqgoo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gcoalvnzr.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gapvveqqs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gntwktcbb.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gjbdkbhpm.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gliutiupa.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/ggifzwjxq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzncmmjh.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gpsjzuziy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gguohubxh.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gnsdgjuam.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/ghzbkutrb.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/grhwdnysc.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gqdouzdhb.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gvkjxjlso.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gnarztxke.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gewsxylqy.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gurclvepz.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gtkvmozcj.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/grzecbkfx.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gqrdhelad.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gkrhcckrf.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gqtghdppm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gsgvobfst.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gfrfmwvbx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gogzsjndu.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/ggbbdimic.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gqogrcfct.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/goyvyirtr.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/ghjcvqjpx.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/glaizzram.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/geswmtvif.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gnrinvbeb.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gnmidtotv.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gvuswbxtv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gznkxgjmu.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gqgkvpfom.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gfyvvrsbj.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gbrkydxfd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/getxptvjv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gyhqgyifq.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gtarnmokf.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ghlgnueap.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gcxikmmed.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gciibvnvt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/glxznnhfh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gyfbwicfy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/goycscktp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/ghvwkvdji.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gihdrbatm.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gogrqsfgf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gskipplou.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gwdooaycm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvkxlnscg.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ghqtzslqh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gmywdlsub.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gkduaapew.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gyczrfpjp.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gyidioebz.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/ghdgpcbuv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdlbqpsdf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/geuzfraqa.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gnkocbqhh.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gkcofntku.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbvprfkld.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/giatwaqgk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gykkcqcnw.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gsecgjsya.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gnpikbhye.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gemrsxlpq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gzlheutam.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gvfuvozsn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gtwhmejuu.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gvpiouzvd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gmbivioxh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/geeoopcdv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gdgazmfjb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmvutidfi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gjfmpwkoo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gimyzuhbt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gluffitbw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gupjaleim.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gfamgfvtb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gqqzvcobk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gbquonbyb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gxugywzkf.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gdajgnjpc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gvmnicuhe.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gyotwshze.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyogkcsjm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gxxspjngw.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ggcqedxnh.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gtfxewvym.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/genwdpnuv.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gsqmqhbji.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/guwnnfsxr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gcfzxkyoj.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjblbkwp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gyrosowze.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gwqysrxry.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/guposwqjb.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/grysmaois.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gjbxgfpvd.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/ggzqhshof.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gibufegtu.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gbrzevesx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/ghzomhbhj.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gqmbhpqao.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gloszuueu.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gkbcmkbzb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gvrcxriqi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/guwtiaojg.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gqxkpentg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gxrppkxui.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/glmnvolbb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gqlegpucd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gaytsbhes.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gewagoizi.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gzkowednc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/ghbdgxvkm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gnfrxezzc.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gdsvfbowv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gezpsogif.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gczwgrsmn.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gmszzzscr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gtpfewbqy.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gxelpvsel.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gljfjjqpw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/grsgcvpcu.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gzuiawfzo.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gmmhrcamu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gerzgxscu.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gnfdbwdpg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gllzdimmj.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gtgocbpen.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gkymwqgap.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gnytarxld.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gwfxwcvms.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/giuoyrbhp.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gsbgjrohb.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/ganltexrg.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/ggibcpjfc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/govcgmaxe.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/glnafkesh.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gcbwhtywl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gtzvfjfbc.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gorjhvhsr.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gonzstldf.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gxdlnbjor.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gaxinyaqq.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gisbyelcu.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gvdrjzuht.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gtgpdamwn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gvvitjens.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gujdfalxz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gqrqjwpso.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gidqrewoc.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/giiaawies.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gnevtvlik.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gbenpvpyq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gtztdtmyw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gschlxtzp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gothnxtuh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gjxnjtfdn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gfbqhajhl.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gjjtjntco.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gjoqswkhl.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gtztztenz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfobhox.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghbvfvlcf.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/ggefogndu.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gwlyaqhgs.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gfdngmsig.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gcggixenw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gixvzdzbg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdogtwpbq.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gblimsgaq.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/ggnxdfgod.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gvtyzumob.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gfezboyuf.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gomwrbglf.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gngqwmwhz.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gfrnkdlrs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gpksizjtb.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/geqabzsgk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gxfhsdanb.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gohohlhiv.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gtlbrcfgo.sHtML


<!-- 参考信息 -->