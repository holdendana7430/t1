代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gthxhjbnhs.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtxhlykvmy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gthyaoatev.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtaykfkqxe.html

read -rp "请输入: " ans
来源：http://hz.pycfn.com/gtbvmdrkpl.html

[R78] 交互式菜单
来源：http://hz.shzxlz.cn/gtddpyijgx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daxiang520.top/gtizmjwixe.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtctmbunvi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtgjhcmnyv.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gtdvisnqrf.html

time ./run.sh
来源：http://hz.fengsongda.top/gtzefevads.html

================================================================================
来源：http://hz.yonumen.top/gtdavnuppc.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtqfsrrltx.html

================================================================================
来源：http://hz.sxryk.cn/gtlunuwtay.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtussgvswo.html

#include <stdio.h>
来源：http://hz.yuxming.cn/gtwurdtpxy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtsnpzjfgy.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gtywumoepw.html

int a = 10; printf("%d\n", a);
来源：http://hz.pengpengdd.cyou/gtecjdxrnw.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtodzdbglp.html

int x; scanf("%d", &x);
来源：http://hz.cashguo.top/gtajtqfgeu.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtfzgggiox.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gtiixarrlu.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtirmqcxhl.html

strlen(s)
来源：http://hz.jyoumei.cn/gtmgejvhmm.html

[S06] C：字符串比较
来源：http://hz.vqdsnc.cn/gtfwkleclj.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtmmcmtoov.html

[S07] C：数组遍历求和
来源：http://hz.zdqjudy.top/gtszclpzvj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigfzy.top/gtvmeckdmf.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gteznvgdmo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhixingplan.top/gtbpktzjwp.html

[S09] C：结构体定义与初始化
来源：http://hz.cdnleiting.top/gthctgsleu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gtjeboqtty.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gttgveosgv.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtcjftyxdr.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtzyuabxtr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtcsbzgbfw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtmbymckmf.html

fclose(f);
来源：http://hz.ywan-chungtsiang.top/gthkaukiwc.html

[S12] C：写文件
来源：http://hz.316326.xyz/gtqjgfbzte.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangshuangyany.cn/gtcidsizsu.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gthictowlt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jiagoushi.top/gtgurhmpyu.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtlpqblvpl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnqzz.top/gtqcyonpms.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtemfvcjuj.html

(double) a / b
来源：http://hz.chenzaomai.com/gtkqabhjjc.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gttrfeuvyy.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtawczgrdx.html

[S17] C：安全拼接字符串
来源：http://hz.shangyingyoupin.top/gtzxfzryri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtoiyfytmu.html

[S18] C：命令行参数
来源：http://hz.vqdsnc.cn/gtentetwcr.html

int main(int argc, char **argv)
来源：http://hz.svipenyu.cn/gttaniknle.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtbvlqikci.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtdkekxepz.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtihvpzosk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gtrpqbcyde.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gtgkrihggb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtiohcgqgp.html

[S22] C：字符串转数字
来源：http://hz.zhixingplan.top/gtuzcyvaug.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.kuanghao11.cn/gtrrpjvywx.html

[S23] C：随机数
来源：http://hz.yongpay.top/gtxkygzwsf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sxryk.cn/gtrzbwsjzg.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtjmllyupp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pengpengdd.cyou/gthvfztkty.html

[S25] C：内存拷贝
来源：http://hz.quarkkingdee.top/gtdwnoeoir.html

memcpy(dst, src, n);
来源：http://hz.guannengcc.top/gtkgeddpep.html

[S26] C：内存清零
来源：http://hz.chenlongwang.top/gtllicojew.html

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gthmyafhpz.html

[S27] C：定义常量
来源：http://hz.svipenyu.cn/gtneoteiuk.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtindgnozx.html

[S28] C：静态变量
来源：http://hz.ppjwa.cn/gtfddwdfeb.html

static int counter = 0;
来源：http://hz.smart0.xyz/gtxxaaevmb.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gtzcshnmpp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yonumen.top/gtsqtuzcay.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtithzacpc.html

#ifndef X_H
来源：http://hz.daria6918.cn/gttzrdfwax.html

#define X_H
来源：http://hz.mhx1999.top/gttswjdlyf.html

#endif
来源：http://hz.daxiang520.top/gtcqkgpcvy.html

[S31] C++：Hello World
来源：http://hz.yuxming.cn/gtirevkpgg.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtpaqdgvxb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtwnmxmqry.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtigggeggy.html

std::string s = "hi";  s += "!";
来源：http://hz.tianlin.xyz/gtibijxgbq.html

[S33] C++：vector 增删
来源：http://hz.xylfe.cn/gtnrmcrexv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gtsikcvhky.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gthnigenpn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aibaodan.cn/gtyqmywkxk.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtzanejmut.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtnebvdvxx.html

[S36] C++：unordered_map
来源：http://hz.gogol.net.cn/gtssxpvhxq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtwmhtoblk.html

[S37] C++：set
来源：http://hz.nanxuanxn.top/gtnzdbjrmd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nwbrower.top/gtroetzlvz.html

[S38] C++：排序
来源：http://hz.xylfe.cn/gtalhvcuns.html

std::sort(v.begin(), v.end());
来源：http://hz.zycfv.cn/gtpuyezyra.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangtech.top/gtdlrmwrsg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtdhrmbyyi.html

[S40] C++：查找元素
来源：http://hz.ybcxt.top/gtzfsuphpn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.feifeiyinyue.top/gtfslsubbl.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtcnogyfur.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtmfibavua.html

[S42] C++：继承与虚函数
来源：http://hz.iojbl.cn/gtkdlhyyhg.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtrdbnlpwn.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gtpawhxbgz.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtfpgoerbe.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtcskhojdn.html

void inc(int &x) { ++x; }
来源：http://hz.gotoacloud.top/gtipfqcjeg.html

[S45] C++：lambda
来源：http://hz.jiagoushi.top/gthmyiqlqj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtdzoxgeqk.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtvnnkjwpk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtaoalkmzs.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtmrdasqqr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hammf.cn/gtiinndmnn.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtqwbmuzjg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtxrstacng.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtpmmypwsh.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtmevailpx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtgmujqgrn.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtsttqposo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ivvv.top/gtwuisjyst.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtpemfgsvz.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtwbyfhvyl.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtwvlluniw.html

int size() const noexcept { return n_; }
来源：http://hz.yueranfly.top/gtrutqngsr.html

[S53] C++：移动语义
来源：http://hz.guannengcc.top/gtcrcfxvbn.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gttmjkoupq.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gtvxwmgojp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yueranfly.top/gthbvgqycq.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtsdfldfkh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtpvgotjmj.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtgoprvjhw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtdmdwdvuq.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gtegchiqsp.html

constexpr int N = 10;
来源：http://hz.hnxiangtu.top/gthhzisnns.html

[S58] C++：命名空间
来源：http://hz.pycfn.com/gtwhwvjrih.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtdethqxrf.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtcwdrzopt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daxiang520.top/gtgusquvbc.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtuymmodzk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtuxdlvjou.html

================================================================================
来源：http://hz.chenzaomai.com/gtkqawxezn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtilivqcvd.html

================================================================================
来源：http://hz.birdmap.top/gtrwdtjopv.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtcleeiaxj.html

println("Hello")
来源：http://hz.zhixingplan.top/gtebuyjhbz.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtxiytfakq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtlmmkihcr.html

[T03] Kotlin：字符串模板
来源：http://hz.ydzc1.top/gtwcfmybzm.html

"值: $b"
来源：http://hz.yj20258888.top/gtfhcvvesj.html

[T04] Kotlin：空安全
来源：http://hz.gotoacloud.top/gtqzwanwzm.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtprrxtziz.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gtfqlhxvcm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hywenlv.cn/gtnjzagvkm.html

[T06] Kotlin：集合映射
来源：http://hz.dashuyun.cn/gtgpfpqkin.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigfzy.top/gtdwupylgr.html

[T07] Kotlin：集合过滤
来源：http://hz.xuanzx.com/gthghwmutj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gtplizflta.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtzahkkukv.html

data class User(val name: String, val age: Int)
来源：http://hz.chenjidiqi.icu/gtdpagktvl.html

[T09] Kotlin：扩展函数
来源：http://hz.redwolf501.top/gtujnjpdqe.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtwummesuu.html

[T10] Kotlin：默认参数
来源：http://hz.yongpay.top/gteuejqofl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenlongwang.top/gtgfrvkfvz.html

[T11] Kotlin：协程
来源：http://hz.zhengqikj.top/gtckwjaxqt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtohkumrin.html

[T12] Kotlin：解构声明
来源：http://hz.tianlin.xyz/gtcimbemuz.html

val (a, b) = Pair(1, 2)
来源：http://hz.hongshengwenyu.top/gthmvwolbc.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtvvxnfmns.html

val m = mapOf("a" to 1)
来源：http://hz.zycfv.cn/gtkvmnovqi.html

[T14] Kotlin：循环
来源：http://hz.xinyue.icu/gtpfdbhjsa.html

for (i in 1..10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtpsanlglt.html

[T15] Kotlin：接口
来源：http://hz.ivvv.top/gtohhvagoc.html

interface Shape { fun area(): Double }
来源：http://hz.yuxming.cn/gtzarojuir.html

[T16] Swift：Hello World
来源：http://hz.zycfv.cn/gtygyqmdhh.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtcfebtfra.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gteimvliii.html

var a = 1;  let b = 2
来源：http://hz.birdmap.top/gtwdpcekax.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtdyvkkrlj.html

"值: \(b)"
来源：http://hz.hywenlv.cn/gtnlrdedlt.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtbpbcwrwv.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtqiajqqow.html

[T20] Swift：数组操作
来源：http://hz.nanxinkj.top/gtymgdbhuk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtfdvtuvsf.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtosgapdwu.html

for x in a { print(x) }
来源：http://hz.ehwqpu.com/gtrfqflbgd.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gttavnwtsx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tianlin.xyz/gtyelclpns.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gthtvpxtwb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigfzy.top/gtohgzrkdg.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtygcvhrrs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhixingplan.top/gtgrzlpvva.html

[T25] Swift：结构体
来源：http://hz.cdnleiting.top/gtlacwbppn.html

struct P { var x: Int }
来源：http://hz.meibo888.top/gtsxaflujm.html

[T26] Swift：类与重写
来源：http://hz.fzhhl.top/gtcgldhxev.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gtsuclzqsp.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gtpmqthjmd.html

do { try f() } catch { print(error) }
来源：http://hz.birdmap.top/gtnjuyhkxq.html

[T28] Swift：枚举
来源：http://hz.yj20258.top/gtimpgkxhh.html

enum Color { case red, green }
来源：http://hz.zhiwuduotai.top/gtwihdrcbe.html

[T29] Swift：guard 提前返回
来源：http://hz.wangshuangyany.cn/gteczaihsy.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gtoazunvdr.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gtjnzqjeiv.html

protocol Shape { func area() -> Double }
来源：http://hz.c1oappe.top/gtjaiydywv.html

[T31] Lua：Hello World
来源：http://hz.shangyingyoupin.top/gthjkccswj.html

print("Hello")
来源：http://hz.xinyue.icu/gtzdjzrogb.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gtvjzubdwy.html

local a = 1
来源：http://hz.hnqzz.top/gtyrhimuwq.html

[T33] Lua：表（数组）
来源：http://hz.gzhubu.top/gtrtjctjyu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dashuyun.cn/gtlvnptytt.html

[T34] Lua：遍历表
来源：http://hz.yj202588.top/gtxfhyifsb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tian-w.cn/gtugxrehnb.html

[T35] Lua：字典表
来源：http://hz.cheryme.top/gthnpmbymg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.aibaodan.cn/gtylxzyiqg.html

[T36] Lua：函数
来源：http://hz.cucudq.cn/gtsuvnjwmg.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gtktsxunhi.html

[T37] Lua：字符串拼接
来源：http://hz.jianghu66.top/gtavsrglai.html

"a" .. "b"
来源：http://hz.wangdashe.top/gtrrfzjlxx.html

[T38] Lua：条件
来源：http://hz.sweek.top/gtarvlulpw.html

if x > 0 then print("正") end
来源：http://hz.jinqigfzy.top/gthisyxiyo.html

[T39] Lua：模式匹配
来源：http://hz.tian-w.cn/gtucevezma.html

string.find(s, "%d+")
来源：http://hz.fzhhl.top/gtspqjjbts.html

[T40] Lua：元表
来源：http://hz.shangyingyoupin.top/gtgmvapygp.html

setmetatable({}, { __index = base })
来源：http://hz.guowangkeji.top/gtbucfeakq.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gtbbkccbwi.html

print "Hello\n";
来源：http://hz.gotoacloud.top/gttlizxchx.html

[T42] Perl：变量类型
来源：http://hz.haohaochexian.top/gtcducryed.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yangfankeji.com/gtsdxvbzgo.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gthplwxcjd.html

"值: $a"
来源：http://hz.jyoumei.cn/gtjzzphjns.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtiydpjebr.html

if ($a > 0) { print "正"; }
来源：http://hz.havefunace.top/gtqopncctq.html

[T45] Perl：数组遍历
来源：http://hz.yj20258888.top/gtdbsuiswm.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtvwnnytqx.html

[T46] Perl：哈希操作
来源：http://hz.ydzc1.top/gtwntoxryr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtecxebiwd.html

[T47] Perl：正则捕获
来源：http://hz.yvedp.cn/gtorhemmoz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.aibaodan.cn/gtodxiavvw.html

[T48] Perl：正则替换
来源：http://hz.birdmap.top/gtyfiwbkpp.html

$s =~ s/old/new/g;
来源：http://hz.hnxiangtu.top/gtqfdfueyb.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtyojmtzmv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yangfankeji.com/gtblhftqlr.html

[T50] Perl：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtzqxbizck.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yueranfly.top/gtziatydjo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangdashe.top/gtmcvroqxp.html

[T51] Scala：Hello World
来源：http://hz.hysaishi.cn/gtzanwkpap.html

println("Hello")
来源：http://hz.zycfv.cn/gtjqmqxpbs.html

[T52] Scala：变量
来源：http://hz.zhongyouzk.top/gtxopzpxfk.html

val a = 1;  var b = 2
来源：http://hz.ppjwa.cn/gtbeqgyzei.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gtjnbvcgpq.html

s"值: $b"
来源：http://hz.sysykeji.top/gtwwxvohmn.html

[T54] Scala：集合映射
来源：http://hz.gogol.net.cn/gtionmhoaw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtsrcmsgic.html

[T55] Scala：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtvjaeaete.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aibaodan.cn/gtqtutstpi.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gtwplvncde.html

case class User(name: String, age: Int)
来源：http://hz.jinyuanbaomall.cn/gtsvimkaih.html

[T57] Scala：模式匹配
来源：http://hz.havefunace.top/gtteytfsen.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenjidiqi.icu/gtlatfoztw.html

[T58] Scala：函数定义
来源：http://hz.cheryme.top/gtbbqigobz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ywan-chungtsiang.top/gtlcmapeqm.html

[T59] Scala：循环
来源：http://hz.shanyushiyangkeji.top/gthpexulvd.html

for (i <- 1 to 10) println(i)
来源：http://hz.birdmap.top/gtxuyddcwx.html

[T60] Scala：折叠
来源：http://hz.sweek.top/gtourhpyfo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.smart0.xyz/gtsejdaqnh.html

================================================================================
来源：http://hz.zdqjudy.top/gtlkerkxsb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gtregiutdz.html

================================================================================
来源：http://hz.haohaochexian.top/gtepedjsod.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gtsriqyuni.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pycfn.com/gtwnvsrkxq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xziqi.cn/gtovfcpalp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangtech.top/gtempspksn.html

[U03] Py：加载 .env 配置
来源：http://hz.hongshengwenyu.top/gtrcecvtuw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258.top/gtdsoolmme.html

[U04] Py：变量调试打印
来源：http://hz.nwbrower.top/gttsfzsbxe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jyoumei.cn/gtoobgfupm.html

[U05] Py：列表去重且保序
来源：http://hz.ivvv.top/gtuuhzhgkc.html

list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtpqvdhqgm.html

[U06] Py：合并两个字典
来源：http://hz.yuanzhike.top/gtemhhnkud.html

{**a, **b}
来源：http://hz.zhongyouzk.top/gtfsiyqpkr.html

[U07] Py：反转字典键值
来源：http://hz.nwbrower.top/gthnuyogzu.html

{v: k for k, v in d.items()}
来源：http://hz.ywan-chungtsiang.top/gthazdighm.html

[U08] Py：展平二维列表
来源：http://hz.daria6918.cn/gtzsladero.html

[y for x in nested for y in x]
来源：http://hz.chenjidiqi.icu/gtenriqegt.html

[U09] Py：字典取最大值的键
来源：http://hz.zdqjudy.top/gtmgfpbqdd.html

max(d, key=d.get)
来源：http://hz.yuxming.cn/gtabtdcayb.html

[U10] Py：按值排序字典
来源：http://hz.cheryme.top/gtmudnympm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shzxlz.cn/gtiqgqdfbw.html

[U11] Py：生成器表达式
来源：http://hz.ybcxt.top/gtyjpzomra.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gteuxqxgia.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258.top/gthjjzrain.html

Counter(arr).most_common(3)
来源：http://hz.zhiwuduotai.top/gtqdfyruax.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtntotazin.html

deque(maxlen=10)
来源：http://hz.redwolf501.top/gtrywcwjgu.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtruxqzkff.html

defaultdict(list)
来源：http://hz.c1oappe.top/gtfzutxlfo.html

[U15] Py：高精度计时
来源：http://hz.hnqzz.top/gtikklxodv.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtejvhkikv.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtxfauldol.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtlfivtxcl.html


<!-- 参考信息 -->