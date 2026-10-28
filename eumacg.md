代发 wailian999

openssl rand -hex 16
来源：http://hz.tianlin.xyz/gtijoevnkr.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gttgknpbns.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtardkaxbk.html

[R69] 生成随机密码
来源：http://hz.jqgfzy.top/gtybnpbjda.html

head -c 16 /dev/urandom | base64
来源：http://hz.c1oappe.top/gtvbhpdsdi.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtqmthjuld.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtvqzsgcpu.html

[R71] 日期格式化
来源：http://hz.cqqwz.cn/gtmunnegoo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gthbcvgdgi.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtwujyeagr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gtqjzsbhku.html

[R73] 分割大日志
来源：http://hz.ivvv.top/gtjwklusnk.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtlalhfrtn.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtskyzbeed.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtagyleitq.html

[R75] 导出环境变量
来源：http://hz.daria6918.cn/gtngcnyziq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj202588.top/gtuawbpynj.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtqjcutgyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtbgifxrii.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtzlzcilqz.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtfmhkjiao.html

[R78] 交互式菜单
来源：http://hz.yonumen.top/gthynuyfnd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuetiantiany.cn/gtaowdblyv.html

[R79] 解析命令行选项
来源：http://hz.chenjidiqi.icu/gthcujkmjd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuetiantiany.cn/gtckbsezaz.html

[R80] 查看脚本执行耗时
来源：http://hz.gaohongyu789.top/gtqayldxqj.html

time ./run.sh
来源：http://hz.gogol.net.cn/gtapwailhr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkkyiaxgk.html

S. C / C++ 专题
来源：http://hz.hnxiangtu.top/gtfzrnqsrp.html

================================================================================
来源：http://hz.sufxvd.cn/gtzifbznmt.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtbgxnuvgi.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtidkisfke.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtdqndakpl.html

[S02] C：变量与格式化输出
来源：http://hz.andypj.xyz/gtcnqnqeeu.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gtlnakekoc.html

[S03] C：读入整数
来源：http://hz.quarkkingdee.top/gtrxemepja.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangtech.top/gtpotkmasc.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtekeosvxy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtqbvuchml.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtsfqqliwb.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtioorxgeg.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gteovccfxh.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtyjcoktll.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtdaqlzgmc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gthttalmum.html

[S08] C：动态内存分配与释放
来源：http://hz.nwbrower.top/gtxwvfsqtr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtbvkcyawm.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgfzy.top/gtqaoaplkv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.52xcode.cn/gtvlkxjsul.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtgwumqmxt.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtbkpnraka.html

[S11] C：逐行读文件
来源：http://hz.hnqzz.top/gtfpjktsqm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtfprssacj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.c1oappe.top/gtdsntokeg.html

fclose(f);
来源：http://hz.hnqzz.top/gtbizoewfa.html

[S12] C：写文件
来源：http://hz.birdmap.top/gtruwxgfpj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtnduranid.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gtxamkexbq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuetiantiany.cn/gtfvflxzur.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtmjfpkssf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnqzz.top/gtmvalxpwi.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gtsfzmwhoi.html

(double) a / b
来源：http://hz.aizwys.cn/gtjqfmjxkr.html

[S16] C：位操作置位
来源：http://hz.jinghuilouyu.cn/gtanwjryjx.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtorpdxoxx.html

[S17] C：安全拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtmlghpbie.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtlfygkwba.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtfxcjated.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtowlsskur.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtzsljpeoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtqrepnien.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtjjvcymnp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gttoormqsj.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtbzvuoyxt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtcblmdnml.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtmcspemrj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtnpqddneg.html

[S23] C：随机数
来源：http://hz.tianlin.xyz/gtvnfyxjdm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydzc1.top/gtpbqgdazb.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gttybejdir.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ybcxt.top/gtlahveojv.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtnpcsbmnb.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gtaiheqrnp.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtpkgisqfj.html

memset(a, 0, sizeof a);
来源：http://hz.fzhhl.top/gtdygqfnlk.html

[S27] C：定义常量
来源：http://hz.kuanghao11.cn/gtobhecxfh.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtpfodwdhi.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtdkcdbtvt.html

static int counter = 0;
来源：http://hz.bjfxy.top/gtmiyjetje.html

[S29] C：变参函数
来源：http://hz.zhijiandao.cn/gtlkhgclig.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtkjiavdgn.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gthygctikm.html

#ifndef X_H
来源：http://hz.52xcode.cn/gthsvtngab.html

#define X_H
来源：http://hz.yuanzhike.top/gthlsxnooe.html

#endif
来源：http://hz.jinghuilouyu.cn/gtvtcffasf.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtsucejyrd.html

#include <iostream>
来源：http://hz.yongpay.top/gtpapfoten.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtqwdqutdi.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gtztgeaikw.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtixcfwyhf.html

[S33] C++：vector 增删
来源：http://hz.zycfv.cn/gtesivntav.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.52xcode.cn/gtfkhbitwb.html

[S34] C++：遍历 vector
来源：http://hz.xinyue.icu/gtsedszomj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtirmbezsj.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtwaxyvoio.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtftjpqnzh.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtqflwfdhr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtkljsrwbw.html

[S37] C++：set
来源：http://hz.havefunace.top/gtuypxmkoo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.52xcode.cn/gtqhghergf.html

[S38] C++：排序
来源：http://hz.daxiang520.top/gtswvphxjt.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtadgxjpxb.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtwugdidom.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtjccxfcjw.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtdqtgkoox.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gtzjlupiqx.html

[S41] C++：类与构造函数
来源：http://hz.sysykeji.top/gtpyekqkyj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtdnpylizs.html

[S42] C++：继承与虚函数
来源：http://hz.hongshengwenyu.top/gtaxhrhxib.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtvdvrvztf.html

[S43] C++：智能指针
来源：http://hz.redwolf501.top/gtotqexsug.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtmwsavqbd.html

[S44] C++：引用传参
来源：http://hz.jlsjyb.cn/gtwqkufngy.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtufaoowus.html

[S45] C++：lambda
来源：http://hz.yanxiufei.cn/gtccbmzfls.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnxiangtu.top/gtbsnpmcui.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gtrgooxvgg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigfzy.top/gtznvybgjk.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtgbfvkxro.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinghuilouyu.cn/gteszhtllt.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtpugyzezw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtbkazndju.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gtfrlhvudi.html

[S49] C++：写文件
来源：http://hz.hnxiangtu.top/gtjsobtjcq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gterkofcsm.html

[S50] C++：格式化数字
来源：http://hz.ydzc1.top/gtbhwusanm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtuafsskhx.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtwjcprqwu.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gthzapveuv.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtukezfcai.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gtfwvnwfue.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gtlmxlgrfd.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtxltowvcb.html

[S54] C++：异常处理
来源：http://hz.sxryk.cn/gtxcbkkrsn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.andypj.xyz/gtpvnxbsnw.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtlhruixtn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgfzy.top/gtffxmuweu.html

[S56] C++：optional
来源：http://hz.ybcxt.top/gtgbcgqrdu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtlgjtjvax.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtrknhytax.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtnktzswfi.html

[S58] C++：命名空间
来源：http://hz.tanke756.top/gtybnqrlir.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gtuyujoghi.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtqkqlgdhd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gtxsuptsft.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtfojpubso.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtunybbudw.html

================================================================================
来源：http://hz.jinqigufen.top/gtatvgouqb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gthsnzfngm.html

================================================================================
来源：http://hz.gogol.net.cn/gtpmnifnwv.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtgxliftdm.html

println("Hello")
来源：http://hz.xuanzx.com/gtkrslezgr.html

[T02] Kotlin：变量
来源：http://hz.wangdashe.top/gtdfouclyz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.svipenyu.cn/gtuufwqueu.html

[T03] Kotlin：字符串模板
来源：http://hz.hywenlv.cn/gtppglnjft.html

"值: $b"
来源：http://hz.cheryme.top/gttozzemaa.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtcyleijhn.html

val n: String? = null;  n?.length
来源：http://hz.jiagoushi.top/gtymckriom.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtnbzxlukj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dianchejie.cn/gtdedxdluw.html

[T06] Kotlin：集合映射
来源：http://hz.chenjidiqi.icu/gtmsytdmvr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gtweeslrrf.html

[T07] Kotlin：集合过滤
来源：http://hz.yuanzhike.top/gtvhqqvsuc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtufpahwpf.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtxkrweeqx.html

data class User(val name: String, val age: Int)
来源：http://hz.shuidangran.top/gtyklbqpdk.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtugtszbyx.html

fun String.exclaim() = this + "!"
来源：http://hz.aizwys.cn/gtxzmrwske.html

[T10] Kotlin：默认参数
来源：http://hz.xuetiantiany.cn/gtqfbzueke.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jlsjyb.cn/gtnnmxqoxi.html

[T11] Kotlin：协程
来源：http://hz.havefunace.top/gtucpcrata.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jyoumei.cn/gtitchyyro.html

[T12] Kotlin：解构声明
来源：http://hz.jiagoushi.top/gtjdmnznbg.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtqrabftnm.html

[T13] Kotlin：只读 Map
来源：http://hz.jinghuilouyu.cn/gtwlypbgdy.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gtjurmtmff.html

[T14] Kotlin：循环
来源：http://hz.jiagoushi.top/gtusdxtdif.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtjeqdvzzf.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtfwxievha.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258.top/gtbrxzupji.html

[T16] Swift：Hello World
来源：http://hz.bjfxy.top/gtqnuesvwe.html

print("Hello")
来源：http://hz.daria6918.cn/gtujndhezl.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtzzoddfon.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtxwskqhbg.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtojbergse.html

"值: \(b)"
来源：http://hz.mhx1999.top/gtqzlcfnrb.html

[T19] Swift：可选绑定
来源：http://hz.hongshengwenyu.top/gtutkwrcei.html

if let n = opt { print(n) }
来源：http://hz.cqqwz.cn/gtawchcpeo.html

[T20] Swift：数组操作
来源：http://hz.vqdsnc.cn/gtxcalfqfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtfzwcfkrr.html

[T21] Swift：遍历
来源：http://hz.sweek.top/gtynhdrgsg.html

for x in a { print(x) }
来源：http://hz.chenjidiqi.icu/gttfspetbk.html

[T22] Swift：字典
来源：http://hz.hfpthk.cn/gtonzwsgiv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.9152youxi.cn/gtasmeukxc.html

[T23] Swift：函数
来源：http://hz.jyoumei.cn/gtethkdtng.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.9152youxi.cn/gtmtcjunfd.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtisrpgbtt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ywan-chungtsiang.top/gttbyzgxgg.html

[T25] Swift：结构体
来源：http://hz.ydjk.org.cn/gtpjxqolcy.html

struct P { var x: Int }
来源：http://hz.0kj1m.cn/gtrkqiegwj.html

[T26] Swift：类与重写
来源：http://hz.redwolf501.top/gtvplnktfz.html

class A: Base { override func f() {} }
来源：http://hz.cqqwz.cn/gtxcagelje.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtrkyurues.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigufen.top/gtloshlzzh.html

[T28] Swift：枚举
来源：http://hz.havefunace.top/gtkgdnaive.html

enum Color { case red, green }
来源：http://hz.tanke756.top/gtaugmvwxt.html

[T29] Swift：guard 提前返回
来源：http://hz.yonumen.top/gthnlsbisv.html

guard let x = opt else { return }
来源：http://hz.xuanzx.com/gtylkagtsh.html

[T30] Swift：协议
来源：http://hz.zhongyouzk.top/gtgyjfrgwo.html

protocol Shape { func area() -> Double }
来源：http://hz.daria6918.cn/gtmfihbgaq.html

[T31] Lua：Hello World
来源：http://hz.iojbl.cn/gtvhjjozmp.html

print("Hello")
来源：http://hz.jiagoushi.top/gtevlbrrxv.html

[T32] Lua：局部变量
来源：http://hz.ywan-chungtsiang.top/gtbsvdchzo.html

local a = 1
来源：http://hz.yangfankeji.com/gtiqrxmgkz.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gttiohxwus.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dashuyun.cn/gtlcfynivi.html

[T34] Lua：遍历表
来源：http://hz.9152youxi.cn/gthpoxlspf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ehwqpu.com/gtozkinsci.html

[T35] Lua：字典表
来源：http://hz.jyoumei.cn/gtrndglnui.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtcvghoidw.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtszqbiakg.html

function add(a, b) return a + b end
来源：http://hz.chenjidiqi.icu/gtjnsgwets.html

[T37] Lua：字符串拼接
来源：http://hz.aizwys.cn/gtxbvamemp.html

"a" .. "b"
来源：http://hz.tian-w.cn/gtsxuuntag.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gtsouvzqpc.html

if x > 0 then print("正") end
来源：http://hz.cdnleiting.top/gtdzggzjru.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtiyhcwzfg.html

string.find(s, "%d+")
来源：http://hz.hysaishi.cn/gtzuvfgsev.html

[T40] Lua：元表
来源：http://hz.zhongyouzk.top/gtfoakypno.html

setmetatable({}, { __index = base })
来源：http://hz.fzhhl.top/gtpcujnslk.html

[T41] Perl：Hello World
来源：http://hz.jyoumei.cn/gtfkmuxndh.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtnvrnhstd.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gtvysksofj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hywenlv.cn/gtxnvnrqew.html

[T43] Perl：字符串插值
来源：http://hz.yj20258888.top/gtalefixuq.html

"值: $a"
来源：http://hz.havefunace.top/gtnfedzqkd.html

[T44] Perl：条件
来源：http://hz.fzhhl.top/gtrftghbnv.html

if ($a > 0) { print "正"; }
来源：http://hz.jinyuanbaomall.cn/gtsipidzdl.html

[T45] Perl：数组遍历
来源：http://hz.meibo888.top/gtypbcfgyc.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangkeji.top/gtparpjdwz.html

[T46] Perl：哈希操作
来源：http://hz.quarkkingdee.top/gthmlwxcfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xinyue.icu/gtniasxzqt.html

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtucbhcafz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtazfviuqr.html

[T48] Perl：正则替换
来源：http://hz.xuanzx.com/gtuojdgigz.html

$s =~ s/old/new/g;
来源：http://hz.dashuyun.cn/gtoxdvbblv.html

[T49] Perl：函数
来源：http://hz.shanyushiyangkeji.top/gtrkggzock.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtmzraosio.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtbsyknlqc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cqqwz.cn/gtmczxvjuf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tian-w.cn/gtbpocndof.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gtmsrdlxxw.html

println("Hello")
来源：http://hz.haohaochexian.top/gtppyfqtsc.html

[T52] Scala：变量
来源：http://hz.xuetiantiany.cn/gtjjntsyvp.html

val a = 1;  var b = 2
来源：http://hz.52xcode.cn/gtstqwskzp.html

[T53] Scala：字符串插值
来源：http://hz.hysaishi.cn/gtmtulubwp.html

s"值: $b"
来源：http://hz.sxryk.cn/gtxpklnaio.html

[T54] Scala：集合映射
来源：http://hz.redwolf501.top/gthxmkkpvu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gtllbahwtw.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtrxdkllhn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtbmrmysck.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtoelcmisq.html

case class User(name: String, age: Int)
来源：http://hz.ywan-chungtsiang.top/gtqbceztih.html

[T57] Scala：模式匹配
来源：http://hz.feifeiyinyue.top/gtzysbtzzy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sxryk.cn/gtxanpnwsw.html

[T58] Scala：函数定义
来源：http://hz.zhaomingkeji.xyz/gttyhrlaox.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hfpthk.cn/gtuyrmmvex.html

[T59] Scala：循环
来源：http://hz.shanyushiyangkeji.top/gtbhrhhive.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gthjgienlb.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtxinrnsnf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shzxlz.cn/gtulndsjdp.html

================================================================================
来源：http://hz.gzhubu.top/gtxetqyqpu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cqqwz.cn/gtsdmodibt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlsnhlogp.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtpvacyzmz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtmrbapeqf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dashuyun.cn/gtnoutajhc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtejlzankl.html

[U03] Py：加载 .env 配置
来源：http://hz.quarkkingdee.top/gtxujqvyfz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangshuangyany.cn/gtwwtkvyvh.html

[U04] Py：变量调试打印
来源：http://hz.hongshengwenyu.top/gtotetumyd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ydjk.org.cn/gtyxktsggy.html

[U05] Py：列表去重且保序
来源：http://hz.kuanghao11.cn/gteiglhlcp.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtbgjqiett.html

[U06] Py：合并两个字典
来源：http://hz.daria6918.cn/gtwfyidxzw.html

{**a, **b}
来源：http://hz.smart0.xyz/gtgznhnuht.html

[U07] Py：反转字典键值
来源：http://hz.quarkkingdee.top/gtjxgnxhmv.html

{v: k for k, v in d.items()}
来源：http://hz.jqgufenzy.top/gtytovnexo.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangtech.top/gtthiztzjt.html

[y for x in nested for y in x]
来源：http://hz.ybcxt.top/gtduuasuyh.html


<!-- 参考信息 -->