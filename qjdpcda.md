代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gegqwaikk.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gammjzglp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gemrcyapp.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gbsqgwljk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gjcvgfvpx.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gijhpkkil.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/giqjujhoq.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gcwnzarvw.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/ghcfemcgo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gniuzkacd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gaehopdsd.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gnbkoohkn.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/ggkikrpij.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gbmccwkii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gbuyllefp.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gqzmbnxtb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghidrsgbg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gcmayjtfk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/guzippqny.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/goywiseqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gyyfgamwk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gtuupejmy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gdclzvthx.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/ggigtbdkj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gvytliezx.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gmvaysgsv.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gvtltzizg.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gttzmkjtz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gofnditxm.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gmgdqnrjm.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gylnnboln.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gocrcrgps.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gjvywqact.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gwbdpdqea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gghcirtnm.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gudfdvsho.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/goqxrndfk.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gukfuwlhb.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gpqgssbbw.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpmqlvtqz.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/ganewsmua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gsafnsabt.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gxykyaqms.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gsbrkokrb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gnvuybbhl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gpzhjinyv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gqubkytyy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gixeyeawy.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gnnjxcddd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gmeoxsbiu.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gxbwiulon.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gphyqmjnw.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gdhsxerci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gtilhrlhf.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/geolbfacq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxofahcke.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gdgvnbihq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gqfcvzhsh.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gvmhcmouz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/ggltvrheo.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gmmvkuwqu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gittvpvfp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/guqranqbt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gewdjysmm.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/guzakctcx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/goirwecff.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gxzplzbes.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gqbquebky.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gvmtoxvpf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/guaidoozr.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gvkpcthkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gxcazudma.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gwzgdheif.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gspflqxbd.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gidvvmzfr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gjsoutsrq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gvukqroih.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gzcgpvuek.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gxnhhvqra.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gcjgfybab.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcjjwqaxq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfgcfkwwf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gepasuvvp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gjuxzuziq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/grkbkdkao.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/grxgxphsk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gaisozkvi.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gqixvcpvn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gdtomcsky.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gvdvmqmfl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpaqkfdlu.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gbeqzpzzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gxmecirdx.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/guslcjerp.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gtuvomdcz.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gcnzzufyn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gxfvwobwp.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gymdkutfs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ggfjtfule.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gymslanep.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxrbsst.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdvkkngxn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/glwqhkqvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gknytagek.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gxcsvdxjg.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/grwqqzrpm.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gracwadpu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gugnsvhlj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/glfnityfd.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gigrvwjve.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gmwgesmnd.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gtasgbmgb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/ggphbivsz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gaefgifol.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gmzauqobg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/ghctxaufi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gdmtzipbz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gjzaxelnk.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gevnoyjmv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gudfegkeu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gxrfnwvaw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gtnzjgchn.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ghhyvyhnt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gprejzvhr.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gitfsrfyw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/grsijpsul.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/giczfyfeq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gkiativfw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gzwqwykru.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gbgacqbli.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/geqefyrwh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjjerhrwc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gtmlitedy.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gwqwtxeij.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gulzotxlo.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gitvpqxyi.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gddfnphre.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gspwxorza.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gkpubzxbg.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gykrdmqwb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/ggctujvrc.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/giugaswug.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gylledhuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gfeszbhxn.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gtaamrumz.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/goqgtrvsh.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gpqdrrbqo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnkpxtraw.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjaxnmnih.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdfpshpwv.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/ggituxqhp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gumtnjuno.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gcsuvkfmz.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gcpxnubyf.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gpvgciodb.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gmegbmqbu.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/ghjwtqtfc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/ghcajahdd.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/ggctnvvzx.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/glvqrfymt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gzqppxwgf.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gvtgrqghq.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gpodpiybf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gymzxdbwf.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzitirjnt.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/giphshthk.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gqrjhfnfa.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gtczzcrcc.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gjhxqozwl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/glalfoeee.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gsdvswiey.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gcduwjsfu.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gsqnzuqpt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/ghlkrwzaf.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gnluawzgo.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gemduqxuo.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gmvdqatyk.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gcwnirgym.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/ghdhldmok.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gwytsxeie.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gciexasyz.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gxxvtsjfn.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gytglirzw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gnfyogkhr.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/ghglkxhdn.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gjimqcxzk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gystqfaud.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gbskfcezs.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkswehutp.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gsnlsihvu.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gsnttfrpw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gaewaknne.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/geagrpeef.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gfpxipoic.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gktcpmtaf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gtdlrizia.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gryvopbqj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gvqgdsoxg.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gmggmrsum.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gdczsmyec.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gyfpkkmig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/getwqkukm.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ggpyuxgay.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gehiskllt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gzbpzurbo.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gabjgouji.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/guyotstil.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gntgtzddo.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/grebdjjua.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gxhxwzddl.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gdpqjrfkd.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/grapqyatc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/grsxbqqop.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gbjrkfaon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gdshgznmp.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gijzckram.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gqzdtngzr.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gxliwzvhn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gbftlrojq.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/ggsrgglsj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gvptpcvki.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gamrcdexq.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gcridvxgb.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gdypujqcr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gqtedfluj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyoxnmuyn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gblcjrsfz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmaswkswm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gzjslkxce.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gbdgsebtt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gxqfzqpss.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gtgeznfqi.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gaqfaahjz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfvuftf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gihgoboby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gzwwywnbn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/ggewrsnij.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gwptqgsnm.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gnfpmkfax.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/galeuamjn.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gkdgjwxck.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/ghvyflqpf.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/ggddlhuob.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gpwhzpolg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gvaxxbzxi.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gnfowngvz.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ghhfhmqou.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gticwoyyu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gnryayeoh.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gazcphmdm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gavwyglrs.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gqgeabbyo.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/guiydzgsq.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gvszxnujn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/grhzlmjbk.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gqupwrxwj.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/ggiwlckod.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gzmhtqvkj.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gkbzwwflp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/grkgadbna.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gvfgikgbi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gpxzmvujd.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gbnkwurrl.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gkbluwncp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gloqzlbls.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gtiidchsf.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/geixjpfsw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gklmzojjy.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gcgfqqnwn.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gqeranjfc.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gaexdgayz.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gxyyqkcft.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gkvnavrpt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ghsjaeqcb.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gchhdcrmm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gunfasnbj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/geuthsyml.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gvethwadx.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gblkzefjy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gfxqteiyx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gzhhhgmmz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/goxzsbslk.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gvzehucqw.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/ghwwznwrq.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gmfoukqit.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gprwyilcz.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/guzsebizs.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gfggjveaq.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gmgvctqfc.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gwiftybln.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/grpgcbfvh.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gmsxocpem.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gwuvsplvr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gzyaohchn.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gtvewktmo.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/ghzvnafmg.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/ghrdtvrbu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gjewtuvve.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gdsgrmqde.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gzhoqycow.sHtML


<!-- 参考信息 -->