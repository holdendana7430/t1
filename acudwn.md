代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtqdeuqpqs.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtgireqdzz.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtghatjfxv.html

[R67] 生成随机十六进制串
来源：http://hz.fengsongda.top/gtjugdmjoj.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtjzrngtkh.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtdgxvotli.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtchnezrxn.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gtyjputmfn.html

head -c 16 /dev/urandom | base64
来源：http://hz.ywan-chungtsiang.top/gtfgljbrps.html

[R70] 时间戳与互转
来源：http://hz.jlsjyb.cn/gtolovekfh.html

date +%s;  date -d @1700000000
来源：http://hz.andypj.xyz/gtvbomgqmq.html

[R71] 日期格式化
来源：http://hz.mhx1999.top/gtygaeekwa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nwbrower.top/gtuwfpaxwy.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gtvxakssfq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sysykeji.top/gtrpuxsgma.html

[R73] 分割大日志
来源：http://hz.yangfankeji.com/gtgmhgucuo.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtrymoepmf.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtfpgugelo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtpralmwib.html

[R75] 导出环境变量
来源：http://hz.yj202588.top/gtdsbcmbxf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtyrjgybfg.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtoswlntpc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtirqwssov.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtbfzasyqm.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtregyfcwm.html

[R78] 交互式菜单
来源：http://hz.tian-w.cn/gttwwdtrfx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtxnxfvmky.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtuyblhsvy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtmajpewiw.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtmjlwvjib.html

time ./run.sh
来源：http://hz.hywenlv.cn/gtqesipnag.html

================================================================================
来源：http://hz.ehwqpu.com/gtellmnrsh.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtimkvqedk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxkfuqaci.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtdzkrvkwf.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtcuegkbja.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fzhhl.top/gtzpxxrnke.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtdqpnxtsx.html

int a = 10; printf("%d\n", a);
来源：http://hz.zycfv.cn/gtotnqxame.html

[S03] C：读入整数
来源：http://hz.yj202588.top/gtilijxwma.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtutdxwsdj.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtyiewlkdc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuxming.cn/gtfslzihld.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtxxvcthvs.html

strlen(s)
来源：http://hz.cqqwz.cn/gtcmuolrvt.html

[S06] C：字符串比较
来源：http://hz.shuidangran.top/gtsfkoxrrp.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gtxnuzxivl.html

[S07] C：数组遍历求和
来源：http://hz.yonumen.top/gtpqdacpea.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtynrkjpax.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtpypdcnhh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtakvtejhe.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtlrxaabgs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gttouiimmf.html

[S10] C：指针与解引用
来源：http://hz.yangfankeji.com/gtkbcpvekx.html

int *p = &a;  *p = 5;
来源：http://hz.cheryme.top/gtpbbwnjil.html

[S11] C：逐行读文件
来源：http://hz.gotoacloud.top/gtirqprzpr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtgchrjppt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtvgtejqpc.html

fclose(f);
来源：http://hz.mhx1999.top/gttiierhwr.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gtkrsrsauj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hfpthk.cn/gtwvihcrsb.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtjelsxnak.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hfpthk.cn/gtljfeohpy.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtkyjfuszi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tian-w.cn/gtcyyfkwig.html

[S15] C：类型转换
来源：http://hz.shzxlz.cn/gtscyooepd.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtnrbjomti.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtvpkiwhnu.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtcdsfqzqx.html

[S17] C：安全拼接字符串
来源：http://hz.jianghu66.top/gtqraonaoy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.0kj1m.cn/gtnconabud.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtiswrdimm.html

int main(int argc, char **argv)
来源：http://hz.jinqigufen.top/gtyantdpua.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtmbrcoyat.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtvlsaecfp.html

[S20] C：二分查找
来源：http://hz.shuidangran.top/gthpovhcuh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtpssqddse.html

[S21] C：字符类别判断
来源：http://hz.fzhhl.top/gtyvkrcxqb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydjk.org.cn/gtwtccwhbt.html

[S22] C：字符串转数字
来源：http://hz.chenjidiqi.icu/gtcaprggaa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hongshengwenyu.top/gtsimbmfum.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtgynatedc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gtanlooopw.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtxyznqrpy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtbqicbjeh.html

[S25] C：内存拷贝
来源：http://hz.jinghuilouyu.cn/gthqeesvem.html

memcpy(dst, src, n);
来源：http://hz.yongpay.top/gtquhygals.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtaflitifp.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtudjccmap.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtsuqcbflt.html

const double PI = 3.14159;
来源：http://hz.iojbl.cn/gtffdghpxh.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtexvdpfcv.html

static int counter = 0;
来源：http://hz.tianlin.xyz/gtrbsuavoz.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtzinmdjqj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtdmwctoxy.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtqvnvrvbi.html

#ifndef X_H
来源：http://hz.cashguo.top/gtubvzkueg.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtmtjtgkzk.html

#endif
来源：http://hz.zhoulong.xyz/gtmiqxgxxc.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtlhtqmvtg.html

#include <iostream>
来源：http://hz.jiagoushi.top/gtnlhwjrnj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigufen.top/gtwlhscocw.html

[S32] C++：字符串
来源：http://hz.dianchejie.cn/gtzmnabjah.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtzsdkpmqs.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtojohkugz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtnopepxrg.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtebnvdxqz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenlongwang.top/gtfrjnffqi.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtnebdmjjo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gthpfcutms.html

[S36] C++：unordered_map
来源：http://hz.nanxinkj.top/gtbfqhnbww.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtjnsuazwh.html

[S37] C++：set
来源：http://hz.jinqigfzy.top/gtgvdrdaei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtzpdznilp.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gtdkglndue.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gttrqrjhbz.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gtujrvhrmq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtrnktwqty.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gtsquovqgx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtsnwbgino.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtljjousgm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gthnxcseqa.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtyrpttvbh.html

class B : public Base { public: void f() override {} };
来源：http://hz.haohaochexian.top/gtvtdrkqko.html

[S43] C++：智能指针
来源：http://hz.mhx1999.top/gtstpmdwsm.html

auto p = std::make_unique<int>(5);
来源：http://hz.fengsongda.top/gtdowxjqja.html

[S44] C++：引用传参
来源：http://hz.cdnleiting.top/gtarxhferu.html

void inc(int &x) { ++x; }
来源：http://hz.jyoumei.cn/gtvqtvpuhd.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtfshlmior.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtphqkworu.html

[S46] C++：函数模板
来源：http://hz.nanxuanxn.top/gtsahpkvah.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtpulrgabz.html

[S47] C++：结构化绑定遍历
来源：http://hz.shangyingyoupin.top/gtnaqzcqxr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gtflzplxfs.html

[S48] C++：逐行读文件
来源：http://hz.havefunace.top/gtcfqdptge.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.andypj.xyz/gtfovkgfns.html

while (std::getline(in, line)) { }
来源：http://hz.tianlin.xyz/gtriqwikrl.html

[S49] C++：写文件
来源：http://hz.yvedp.cn/gtcwoqqnze.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuanzx.com/gtwbrypxit.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtnhbionvi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.0kj1m.cn/gtinvdfhna.html

[S51] C++：显式类型转换
来源：http://hz.hywenlv.cn/gtmhdxkuiv.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtcnmzlwlu.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtphqkuyfa.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtakmthskb.html

[S53] C++：移动语义
来源：http://hz.c1oappe.top/gtbittduea.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtopjavfxf.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtltclauqu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.birdmap.top/gtrvwgrjfm.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtembglytk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cucudq.cn/gtptualazw.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gtuhsqbtpn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtwyxbvzkn.html

[S57] C++：编译期常量
来源：http://hz.zhoulong.xyz/gtkscmqjbf.html

constexpr int N = 10;
来源：http://hz.yuanzhike.top/gtvjkcclas.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtfsgulymy.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtinjwqhqt.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtzrwdzrqa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtzigeiehg.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtufkjiesv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtyuxbnnxz.html

================================================================================
来源：http://hz.nwbrower.top/gtpnjlhcvu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtgljqzcqw.html

================================================================================
来源：http://hz.jianghu66.top/gtqgyksgxs.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtgiepzwsx.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtpxpvkmfh.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gtrvwrysyg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtfwwuxcjc.html

[T03] Kotlin：字符串模板
来源：http://hz.xziqi.cn/gtxsuaalis.html

"值: $b"
来源：http://hz.yuxming.cn/gtttltguga.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gtvikofdaj.html

val n: String? = null;  n?.length
来源：http://hz.chenjidiqi.icu/gtvhuhvzri.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gtkavhcqdi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtbmqudluh.html

[T06] Kotlin：集合映射
来源：http://hz.yuanzhike.top/gtblaifhxx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gtidigxysg.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtwruwpoqx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtpthwnjns.html

[T08] Kotlin：数据类
来源：http://hz.guannengcc.top/gthczmvwsf.html

data class User(val name: String, val age: Int)
来源：http://hz.gzhubu.top/gtdtakzvly.html

[T09] Kotlin：扩展函数
来源：http://hz.zdqjudy.top/gtvunzzkgc.html

fun String.exclaim() = this + "!"
来源：http://hz.jinyuanbaomall.cn/gtoywxdznr.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gttqaqrzgu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtsjyaxohj.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtezfavvbg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtkcuvstip.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtlgzygvns.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtflrteloc.html

[T13] Kotlin：只读 Map
来源：http://hz.c1oappe.top/gtgphqwzcn.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gteaputtik.html

[T14] Kotlin：循环
来源：http://hz.hnqzz.top/gtxmuzdwkn.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtoewjpils.html

[T15] Kotlin：接口
来源：http://hz.fengsongda.top/gtbjjplait.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtapsqvinw.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtservzedc.html

print("Hello")
来源：http://hz.guannengcc.top/gtpehhecfa.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gtbdbuyulp.html

var a = 1;  let b = 2
来源：http://hz.yonumen.top/gtjobtwydp.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtgpzqzxnr.html

"值: \(b)"
来源：http://hz.aizwys.cn/gtfomqmhwe.html

[T19] Swift：可选绑定
来源：http://hz.nanxinkj.top/gtydmoaqqe.html

if let n = opt { print(n) }
来源：http://hz.cdnleiting.top/gtoyzihuum.html

[T20] Swift：数组操作
来源：http://hz.kuanghao11.cn/gtgdcribun.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhongyouzk.top/gtwjifkoer.html

[T21] Swift：遍历
来源：http://hz.zhoulong.xyz/gtflvddcoo.html

for x in a { print(x) }
来源：http://hz.sysykeji.top/gthhkigbvb.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtnzewxmgy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gtyjwyapwx.html

[T23] Swift：函数
来源：http://hz.daxiang520.top/gtrujzspxl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.bjfxy.top/gtbrgvvtcl.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gtslfeaels.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yvedp.cn/gtynwvabxp.html

[T25] Swift：结构体
来源：http://hz.hnqzz.top/gtrtjtnlmg.html

struct P { var x: Int }
来源：http://hz.cashguo.top/gtwkajgqmh.html

[T26] Swift：类与重写
来源：http://hz.yj202588.top/gtmngekoud.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtptotvqfy.html

[T27] Swift：错误处理
来源：http://hz.ivvv.top/gtuvtedsdm.html

do { try f() } catch { print(error) }
来源：http://hz.feifeiyinyue.top/gtgvtpwemb.html

[T28] Swift：枚举
来源：http://hz.xingfuxueyuan.xyz/gtuructoxu.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtojwnnxwu.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtmkcwcovn.html

guard let x = opt else { return }
来源：http://hz.hywenlv.cn/gtjhynecps.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtfpcgywoa.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtnxabgzcc.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gttsxyqxsg.html

print("Hello")
来源：http://hz.hnxiangtu.top/gtofonsmmg.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtmzhaxeie.html

local a = 1
来源：http://hz.jinyuanbaomall.cn/gttbywwbwz.html

[T33] Lua：表（数组）
来源：http://hz.yvedp.cn/gtoupxgcfk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtedtyiqsg.html

[T34] Lua：遍历表
来源：http://hz.gzhubu.top/gtycrqxkcx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.daxiang520.top/gthedvkfkp.html

[T35] Lua：字典表
来源：http://hz.quarkkingdee.top/gtxwzzsbgz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jlsjyb.cn/gtbgdndofp.html

[T36] Lua：函数
来源：http://hz.nwbrower.top/gtlbqvqlsb.html

function add(a, b) return a + b end
来源：http://hz.jinqigufen.top/gtuxibzlge.html

[T37] Lua：字符串拼接
来源：http://hz.snrcjt.cn/gtyzppuqlb.html

"a" .. "b"
来源：http://hz.jyoumei.cn/gtysjhbvfo.html

[T38] Lua：条件
来源：http://hz.bjfxy.top/gtupnnuqrb.html

if x > 0 then print("正") end
来源：http://hz.snrcjt.cn/gtdicvpkzs.html

[T39] Lua：模式匹配
来源：http://hz.tian-w.cn/gtduoqnzgb.html

string.find(s, "%d+")
来源：http://hz.ppjwa.cn/gtyraqepwi.html

[T40] Lua：元表
来源：http://hz.cashguo.top/gtdjfoyjfx.html

setmetatable({}, { __index = base })
来源：http://hz.dashuyun.cn/gtuuijtlsz.html

[T41] Perl：Hello World
来源：http://hz.zhixingplan.top/gtgidurruk.html

print "Hello\n";
来源：http://hz.sufxvd.cn/gttnfbgogb.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtkfgkymfs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gzhubu.top/gtcjirdgba.html

[T43] Perl：字符串插值
来源：http://hz.quarkkingdee.top/gtlnktephq.html

"值: $a"
来源：http://hz.sxryk.cn/gtsoegzqwk.html

[T44] Perl：条件
来源：http://hz.fengsongda.top/gtqgcfljwq.html

if ($a > 0) { print "正"; }
来源：http://hz.xingfuxueyuan.xyz/gtlmkpnjap.html

[T45] Perl：数组遍历
来源：http://hz.fzhhl.top/gtyvfwypay.html

for my $x (@arr) { print $x; }
来源：http://hz.meibo888.top/gtboulcjbm.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gthiherhdq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnxiangtu.top/gtqokftkuq.html

[T47] Perl：正则捕获
来源：http://hz.hywenlv.cn/gtyhzjiwug.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cucudq.cn/gtezvgfpxe.html

[T48] Perl：正则替换
来源：http://hz.shanyushiyangkeji.top/gtmxnzosbm.html

$s =~ s/old/new/g;
来源：http://hz.haohaochexian.top/gtmybezqjv.html

[T49] Perl：函数
来源：http://hz.zhengqikj.top/gtzfrfqlmd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtzeormbxu.html

[T50] Perl：逐行读文件
来源：http://hz.yueranfly.top/gtmvhegrsu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtslpycdvw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhixingplan.top/gtfctadubs.html

[T51] Scala：Hello World
来源：http://hz.birdmap.top/gtsihuywbi.html

println("Hello")
来源：http://hz.9152youxi.cn/gtjagodgls.html

[T52] Scala：变量
来源：http://hz.zhengqikj.top/gtqrdqqyne.html

val a = 1;  var b = 2
来源：http://hz.shuidangran.top/gtxnbbpupy.html

[T53] Scala：字符串插值
来源：http://hz.nwbrower.top/gttzxybnlm.html

s"值: $b"
来源：http://hz.tianlin.xyz/gtobbbkcyk.html

[T54] Scala：集合映射
来源：http://hz.pengpengdd.cyou/gtwjfmfmek.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigufen.top/gtjvfecxhf.html

[T55] Scala：集合过滤
来源：http://hz.cdnleiting.top/gtpzpktxhj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hnxiangtu.top/gtfzcsjrio.html

[T56] Scala：样例类
来源：http://hz.nanxuanxn.top/gtlxmehrch.html

case class User(name: String, age: Int)
来源：http://hz.zycfv.cn/gteglpuvpd.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtkirfqxge.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtsozjqcfg.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gtwqtescyw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gtzhjtobar.html

[T59] Scala：循环
来源：http://hz.sysykeji.top/gtjjlotqec.html

for (i <- 1 to 10) println(i)
来源：http://hz.shuidangran.top/gtcgesfrhm.html

[T60] Scala：折叠
来源：http://hz.cashguo.top/gtrkgzkruo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.mhx1999.top/gtllgexvbi.html

================================================================================
来源：http://hz.yonumen.top/gtgfjpacms.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtqvdytwev.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsbumspwk.html

[U01] Py：创建虚拟环境
来源：http://hz.shuidangran.top/gtpkepkucz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtmekyljyu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgufenzy.top/gtbfosonby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.birdmap.top/gtrbdnfxig.html

[U03] Py：加载 .env 配置
来源：http://hz.nwbrower.top/gtqtcjyplm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sufxvd.cn/gttdwhtuoz.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gtmqehrgfj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cashguo.top/gteispplpg.html

[U05] Py：列表去重且保序
来源：http://hz.ydjk.org.cn/gtflcbfidf.html

list(dict.fromkeys(arr))
来源：http://hz.svipenyu.cn/gtdimnhpjl.html

[U06] Py：合并两个字典
来源：http://hz.hnqzz.top/gtiavipjgr.html

{**a, **b}
来源：http://hz.jinqigfzy.top/gtvdbwtbem.html


<!-- 参考信息 -->