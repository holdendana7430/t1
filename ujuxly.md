代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtcbxzjkpn.html

[R70] 时间戳与互转
来源：http://hz.guannengcc.top/gtlrmtcfpq.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtshriqgug.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtkujcrxqo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtbuuweytp.html

[R72] 等待端口就绪
来源：http://hz.daria6918.cn/gtfsmaubiz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gtubsmlzha.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtuslkwwjz.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtrxzjhjvv.html

[R74] 批量重命名
来源：http://hz.shanyushiyangkeji.top/gtxoqqyssf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aibaodan.cn/gtfpvviwvz.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtsyocjjan.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ybcxt.top/gttysgvuib.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtznrseipi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtmqpzxvmy.html

[R77] 读取用户输入
来源：http://hz.yvedp.cn/gtabwyvysy.html

read -rp "请输入: " ans
来源：http://hz.svipenyu.cn/gtshxtfvwb.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gteeyfsacl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgufenzy.top/gtmrrpgcze.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtfelqhxpm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gttbeaqnko.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtyxtitiig.html

time ./run.sh
来源：http://hz.zhiwuduotai.top/gtlvkdzwqh.html

================================================================================
来源：http://hz.zycfv.cn/gtjkuyehdf.html

S. C / C++ 专题
来源：http://hz.zycfv.cn/gtuclrhptl.html

================================================================================
来源：http://hz.xuanzx.com/gtleurdbsw.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gtfcenwbli.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtelksquxl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtqhyevvfv.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gttpsnadta.html

int a = 10; printf("%d\n", a);
来源：http://hz.fzhhl.top/gtgdheaecf.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtismdcyxa.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gthurgdrre.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtxsiwomvm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dianchejie.cn/gtoihmqtqv.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtreycsssc.html

strlen(s)
来源：http://hz.chenjidiqi.icu/gtaibdbuuk.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtrbpddsvj.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtzotrldqm.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtdoncisua.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtsrezbfwb.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigufen.top/gtkjoyrwky.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ybcxt.top/gtmreauyvy.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtvortmrib.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gthspyoqvk.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtzqsonhdk.html

int *p = &a;  *p = 5;
来源：http://hz.bjfxy.top/gtqabzbntu.html

[S11] C：逐行读文件
来源：http://hz.jqgfzy.top/gtkbdovtyp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.andypj.xyz/gtijfrbyqd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnxiangtu.top/gtcdueghqc.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtzldfeiql.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtplnrrood.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhongyouzk.top/gtlvqxmkgw.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtdhjytknr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangkeji.top/gtsxifvtla.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtqyvjpfzg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtnotkbgof.html

[S15] C：类型转换
来源：http://hz.52xcode.cn/gtzszqkpas.html

(double) a / b
来源：http://hz.nwbrower.top/gtecamnpql.html

[S16] C：位操作置位
来源：http://hz.hywenlv.cn/gtzfpweksc.html

x |= (1 << 3);
来源：http://hz.mhx1999.top/gtmnvfdhzs.html

[S17] C：安全拼接字符串
来源：http://hz.gogol.net.cn/gtvgofcrdp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangshuangyany.cn/gthjtdsfsb.html

[S18] C：命令行参数
来源：http://hz.hysaishi.cn/gtmvtkjkuz.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gtddxnrbqr.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtkhxscnvh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtfcchkqfp.html

[S20] C：二分查找
来源：http://hz.hfpthk.cn/gtgebbfrhd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtmyqndlha.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtihevjvyl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gaohongyu789.top/gtdfhxaayg.html

[S22] C：字符串转数字
来源：http://hz.hywenlv.cn/gtisgmgpul.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtsatlpazn.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtuygsfesp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtpxlsgtvf.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtzrssxqts.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gtmpyrkeyq.html

[S25] C：内存拷贝
来源：http://hz.hnqzz.top/gtknhwtnxh.html

memcpy(dst, src, n);
来源：http://hz.cqqwz.cn/gtudovhrjq.html

[S26] C：内存清零
来源：http://hz.cdnleiting.top/gtudgmpksq.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtlgjfooni.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gthjbutjnz.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gteyyylvxb.html

[S28] C：静态变量
来源：http://hz.daria6918.cn/gtxhmbuvlg.html

static int counter = 0;
来源：http://hz.hnxiangtu.top/gtrfnqhiyc.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtxciacvce.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtpevcfqma.html

[S30] C：头文件保护
来源：http://hz.hysaishi.cn/gtdjzsvjvf.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtzhnycltj.html

#define X_H
来源：http://hz.ydjk.org.cn/gthetsrbmy.html

#endif
来源：http://hz.gogol.net.cn/gtwvntelqo.html

[S31] C++：Hello World
来源：http://hz.cucudq.cn/gtdslveorj.html

#include <iostream>
来源：http://hz.yongpay.top/gtvjgcoxiu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtreaivnzs.html

[S32] C++：字符串
来源：http://hz.quarkkingdee.top/gthafkmlsa.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtxsqelfpe.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtinoeibzr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gtmuupzeyc.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtrmfnmewo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtonafrphr.html

[S35] C++：map
来源：http://hz.sweek.top/gtoslzhswq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtmsmzsgtj.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtiqpupbvj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtdnvwcvzs.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtksewoidr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gtsihdrxpr.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtncjiyyvk.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gtyxuurbre.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtvdanuzvf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydjk.org.cn/gtrcjgylvd.html

[S40] C++：查找元素
来源：http://hz.sweek.top/gtxdyvrrgz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtzpxjubzh.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtgrmbybmu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shangyingyoupin.top/gttyselkkh.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtmetmakdm.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuanzx.com/gtspsjftyz.html

[S43] C++：智能指针
来源：http://hz.shzxlz.cn/gtrbwncwbr.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtvzmxihyc.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtgdwgxyzg.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtoupyqtyu.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtrbhzxkau.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtfylccyty.html

[S46] C++：函数模板
来源：http://hz.xingfuxueyuan.xyz/gtdssdkbjt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtylgqhcrq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ehwqpu.com/gtyqmmvton.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtnmjljaza.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtdgduwsyp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtmviqtmil.html

while (std::getline(in, line)) { }
来源：http://hz.haohaochexian.top/gtywnlmjfj.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gttfuzpzwp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtriyftvln.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtfyhhjfxg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtpgkoxwwf.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gtlcaadkfw.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtrbcgkczw.html

[S52] C++：const 与 noexcept
来源：http://hz.sufxvd.cn/gtttiwmhlb.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtgduoahrm.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtfcsleixs.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtpnmkgske.html

[S54] C++：异常处理
来源：http://hz.jqgufenzy.top/gtpbimhsky.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtdgwfijbu.html

[S55] C++：结构化绑定
来源：http://hz.svipenyu.cn/gtodzvynyq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sweek.top/gtnfvibuzq.html

[S56] C++：optional
来源：http://hz.chenzaomai.com/gtmkfdpshr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.c1oappe.top/gtpzztcbjs.html

[S57] C++：编译期常量
来源：http://hz.wangdashe.top/gtkzexlrbt.html

constexpr int N = 10;
来源：http://hz.jinyuanbaomall.cn/gtifufmvhi.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtpsiukmgp.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtiyfmwjam.html

[S59] C++：静态断言
来源：http://hz.wangdashe.top/gthpykdfuf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtzksnyfpc.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtceqpvaid.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtnmequxcm.html

================================================================================
来源：http://hz.bjfxy.top/gtxcwzqrle.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtrhaxonds.html

================================================================================
来源：http://hz.hammf.cn/gtssbiuvkt.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtzhwqrbiy.html

println("Hello")
来源：http://hz.ppjwa.cn/gtmjquzjli.html

[T02] Kotlin：变量
来源：http://hz.zhixingplan.top/gtsztpmdux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtyelkhseo.html

[T03] Kotlin：字符串模板
来源：http://hz.haohaochexian.top/gtzzspymgq.html

"值: $b"
来源：http://hz.yonumen.top/gtapfecosy.html

[T04] Kotlin：空安全
来源：http://hz.yuxming.cn/gtvstvtpif.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtaercsbdz.html

[T05] Kotlin：when 表达式
来源：http://hz.gotoacloud.top/gtpwsjuhcq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtdvhxmthq.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtbxmiajza.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ybcxt.top/gtfkkpqvjx.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtejtqeoss.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtpgvembfj.html

[T08] Kotlin：数据类
来源：http://hz.daria6918.cn/gthdyuzsov.html

data class User(val name: String, val age: Int)
来源：http://hz.xuanzx.com/gtktsntyip.html

[T09] Kotlin：扩展函数
来源：http://hz.hfpthk.cn/gtjdfqctlh.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtmxdvilhu.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gtqngxasjw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtofjqrowk.html

[T11] Kotlin：协程
来源：http://hz.xziqi.cn/gtwolkgfzk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtwujfitki.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtzklyldtm.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtnnrkmdln.html

[T13] Kotlin：只读 Map
来源：http://hz.ppjwa.cn/gtxcylgiwy.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gtjfjwmgsq.html

[T14] Kotlin：循环
来源：http://hz.ivvv.top/gtcdbunvua.html

for (i in 1..10) println(i)
来源：http://hz.xuanzx.com/gtzbqutaye.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gtvdkvbkuq.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigfzy.top/gtqumoiaeb.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtfdzsyvrb.html

print("Hello")
来源：http://hz.smart0.xyz/gtcsxdwxfo.html

[T17] Swift：变量与常量
来源：http://hz.gaohongyu789.top/gtjekcqiwi.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtyaubhuwb.html

[T18] Swift：字符串插值
来源：http://hz.gaohongyu789.top/gtswroldbw.html

"值: \(b)"
来源：http://hz.nwbrower.top/gtheejqlqi.html

[T19] Swift：可选绑定
来源：http://hz.shuidangran.top/gtzstxxoyf.html

if let n = opt { print(n) }
来源：http://hz.cucudq.cn/gtdrrizpvh.html

[T20] Swift：数组操作
来源：http://hz.jyoumei.cn/gtlcimolut.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinyuanbaomall.cn/gtyecchxct.html

[T21] Swift：遍历
来源：http://hz.nanxinkj.top/gtyixxuxkl.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtwzaavsov.html

[T22] Swift：字典
来源：http://hz.dianchejie.cn/gtyffhzqya.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.meibo888.top/gtzctnolpw.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtfbtaucdh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.meibo888.top/gtkuvpppyz.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtenugkpik.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jiagoushi.top/gtrdickmsk.html

[T25] Swift：结构体
来源：http://hz.meibo888.top/gtcuhfkavq.html

struct P { var x: Int }
来源：http://hz.cucudq.cn/gtoebgidhj.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtndrzkgmf.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtrxigbxsc.html

[T27] Swift：错误处理
来源：http://hz.tianlin.xyz/gtfoqwisrj.html

do { try f() } catch { print(error) }
来源：http://hz.yanxiufei.cn/gtxrupyfpv.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtqfzbgbng.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gtuvxazwsc.html

[T29] Swift：guard 提前返回
来源：http://hz.jyoumei.cn/gtabivdagp.html

guard let x = opt else { return }
来源：http://hz.snrcjt.cn/gtdveedvnq.html

[T30] Swift：协议
来源：http://hz.shanyushiyangkeji.top/gtbwejfsjp.html

protocol Shape { func area() -> Double }
来源：http://hz.pengpengdd.cyou/gtbnekangd.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gtmnsqjmqv.html

print("Hello")
来源：http://hz.havefunace.top/gtxbrcxplm.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtybeowuwz.html

local a = 1
来源：http://hz.yueranfly.top/gtgxhyutvs.html

[T33] Lua：表（数组）
来源：http://hz.316326.xyz/gtcaumkgot.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.redwolf501.top/gtsltnccrc.html

[T34] Lua：遍历表
来源：http://hz.jqgufenzy.top/gtahcmnmiq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtjqrsdahn.html

[T35] Lua：字典表
来源：http://hz.wangdashe.top/gtncooaztm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shangyingyoupin.top/gtfxjfibgh.html

[T36] Lua：函数
来源：http://hz.daria6918.cn/gtvxemflqp.html

function add(a, b) return a + b end
来源：http://hz.iojbl.cn/gtpinmylyx.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gthikxqnam.html

"a" .. "b"
来源：http://hz.wangdashe.top/gtgwgftnzm.html

[T38] Lua：条件
来源：http://hz.ywan-chungtsiang.top/gtahumdofi.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gtukavmmap.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtrdsimokn.html

string.find(s, "%d+")
来源：http://hz.xinyue.icu/gtckyadwwp.html

[T40] Lua：元表
来源：http://hz.chenlongwang.top/gtqgxzdasz.html

setmetatable({}, { __index = base })
来源：http://hz.nanxinkj.top/gtedrirxhn.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gtujufyzdq.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtsuwsolwz.html

[T42] Perl：变量类型
来源：http://hz.cdnleiting.top/gtjolkaapt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydjk.org.cn/gtndmrrglb.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtwbagfyxd.html

"值: $a"
来源：http://hz.redwolf501.top/gtahlcnyvq.html

[T44] Perl：条件
来源：http://hz.redwolf501.top/gtbjlvnlbv.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangkeji.top/gtnzzbqvjg.html

[T45] Perl：数组遍历
来源：http://hz.ywan-chungtsiang.top/gtycjrptwf.html

for my $x (@arr) { print $x; }
来源：http://hz.sufxvd.cn/gtqfxwfuiy.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gtqieqpxbz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.52xcode.cn/gtzwhaozvc.html

[T47] Perl：正则捕获
来源：http://hz.tianlin.xyz/gtlamgwdud.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtexzwqado.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gtwrtgekcq.html

$s =~ s/old/new/g;
来源：http://hz.hywenlv.cn/gtjxsemrkg.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gtgucjpocl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.snrcjt.cn/gtytfpztfd.html

[T50] Perl：逐行读文件
来源：http://hz.birdmap.top/gtbzoaxwbi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.0kj1m.cn/gtvdgvppam.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yonumen.top/gtxixtfavl.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtdrqkubbe.html

println("Hello")
来源：http://hz.shuidangran.top/gtdxxmsxaz.html

[T52] Scala：变量
来源：http://hz.cheryme.top/gtaeirxkvv.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtnolqrrqi.html

[T53] Scala：字符串插值
来源：http://hz.hammf.cn/gtzdiuwcrp.html

s"值: $b"
来源：http://hz.gzhubu.top/gtgejwubjb.html

[T54] Scala：集合映射
来源：http://hz.pycfn.com/gtiqommzft.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gtsyudbzno.html

[T55] Scala：集合过滤
来源：http://hz.shangyingyoupin.top/gtcatxarzs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gttqjjjnmq.html

[T56] Scala：样例类
来源：http://hz.jinqigufen.top/gtvzcetfoi.html

case class User(name: String, age: Int)
来源：http://hz.hywenlv.cn/gtwbkrxdzq.html

[T57] Scala：模式匹配
来源：http://hz.snrcjt.cn/gtpfehqlpi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jqgufenzy.top/gtcpxmatyi.html

[T58] Scala：函数定义
来源：http://hz.ydzc1.top/gtnvbwmwfe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ppjwa.cn/gtyefsbunk.html

[T59] Scala：循环
来源：http://hz.xuanzx.com/gtqfdbeiyc.html

for (i <- 1 to 10) println(i)
来源：http://hz.sufxvd.cn/gtjfbblnyj.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtkdkikpfv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtgzifkhkw.html

================================================================================
来源：http://hz.cheryme.top/gtbqmxzykz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shzxlz.cn/gtapmedckc.html

================================================================================
来源：http://hz.dashuyun.cn/gtggllghhh.html

[U01] Py：创建虚拟环境
来源：http://hz.zhongyouzk.top/gthlesmvpp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtqzjhzpbd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtrgmuznxp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tianlin.xyz/gtllnkjjxw.html

[U03] Py：加载 .env 配置
来源：http://hz.tian-w.cn/gtwglmutvt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258888.top/gtlleywgxk.html

[U04] Py：变量调试打印
来源：http://hz.9152youxi.cn/gtmendmmjb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gtzegnehqs.html

[U05] Py：列表去重且保序
来源：http://hz.svipenyu.cn/gtlshymvgm.html

list(dict.fromkeys(arr))
来源：http://hz.xuanzx.com/gtlsxbqwtf.html

[U06] Py：合并两个字典
来源：http://hz.hnxiangtu.top/gthbbgwicv.html

{**a, **b}
来源：http://hz.zdqjudy.top/gtplaatabe.html

[U07] Py：反转字典键值
来源：http://hz.zycfv.cn/gtddigsmbw.html

{v: k for k, v in d.items()}
来源：http://hz.ydjk.org.cn/gthndlxtdd.html

[U08] Py：展平二维列表
来源：http://hz.yueranfly.top/gtdscjuxbz.html

[y for x in nested for y in x]
来源：http://hz.snrcjt.cn/gtfqhoaudm.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtuswhfalj.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtgkbejtez.html

[U10] Py：按值排序字典
来源：http://hz.nwbrower.top/gtjdsqillr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.c1oappe.top/gtrtyxzicp.html


<!-- 参考信息 -->