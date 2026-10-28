代发 wailian999

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtkvnyjqcz.html

[R68] 计算文件校验值
来源：http://hz.yonumen.top/gtxxpaxnpm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtciclmqft.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtowvcigis.html

head -c 16 /dev/urandom | base64
来源：http://hz.kuanghao11.cn/gtvqwivhsp.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gtslpkmtvu.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtdklxipyb.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtbxdaxrkm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gtyycggztj.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtjgujpcay.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtzarlwfmn.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtxeevyjck.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtubwyczro.html

[R74] 批量重命名
来源：http://hz.dashuyun.cn/gtetwvhhwa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtwwuiacla.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gtegzudumr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.svipenyu.cn/gtkgvfktpx.html

[R76] 使用临时文件
来源：http://hz.xziqi.cn/gtbvpgbhyi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtsngqeivc.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtgrgnqhwg.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gtohcmrjuf.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtcnsotdpt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.bjfxy.top/gtsbzyiihs.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtozygupit.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinghuilouyu.cn/gtkfyllrel.html

[R80] 查看脚本执行耗时
来源：http://hz.chenzaomai.com/gtpoiuexqx.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtajuokiiu.html

================================================================================
来源：http://hz.jinqigufen.top/gtliekdtgj.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtswiwmytz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtltcmiihr.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtdbdzhpvj.html

#include <stdio.h>
来源：http://hz.ydjk.org.cn/gtmjhzaafq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.quarkkingdee.top/gtliiqdryl.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gtxrkfakaf.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinghuilouyu.cn/gtfomunvks.html

[S03] C：读入整数
来源：http://hz.shzxlz.cn/gtysccnzsc.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gtumbtaxzs.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gtxblircwr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtyvquedwm.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtlfbgndyi.html

strlen(s)
来源：http://hz.tianlin.xyz/gtsvaxkkxh.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtprkrqgkk.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gttimcrhdw.html

[S07] C：数组遍历求和
来源：http://hz.cdnleiting.top/gtdewdmaeb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sysykeji.top/gtvfslxhhd.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtmtzcoson.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aibaodan.cn/gtclmgmfvy.html

[S09] C：结构体定义与初始化
来源：http://hz.yonumen.top/gtosqjtlcv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gthaxwesdp.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtkuavdkwr.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtfsabjceu.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtgfwfjbef.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.meibo888.top/gttkcchjcs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gtqyhdomwt.html

fclose(f);
来源：http://hz.nwbrower.top/gtilcawwkf.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtbnwdkrwf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhiwuduotai.top/gtaumuffuu.html

[S13] C：宏定义
来源：http://hz.yonumen.top/gtrabjqmrl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gttedpanwp.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gtpszovdqx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuanzhike.top/gtuoflmsts.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gtnpzqjfxe.html

(double) a / b
来源：http://hz.zhixingplan.top/gtjwnpzlly.html

[S16] C：位操作置位
来源：http://hz.xuetiantiany.cn/gtssdipxtg.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtdtjifjmd.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtlstrcprn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aibaodan.cn/gtlliyqegp.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtxoxldrar.html

int main(int argc, char **argv)
来源：http://hz.yj20258888.top/gtqpxafsqj.html

[S19] C：快速排序
来源：http://hz.smart0.xyz/gtbavfhxgf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtwiadsquu.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gtzxsubhpd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtetdiryjm.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtfwdmplsq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtfafqyjis.html

[S22] C：字符串转数字
来源：http://hz.nanxinkj.top/gtjyobhzdq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tianlin.xyz/gtqfpcskjg.html

[S23] C：随机数
来源：http://hz.ivvv.top/gtiwxmebwo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.andypj.xyz/gtepvnovoa.html

[S24] C：获取本地时间
来源：http://hz.tianlin.xyz/gtupscirza.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gthjakuprj.html

[S25] C：内存拷贝
来源：http://hz.haohaochexian.top/gtpomodobx.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtcoegdfym.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtaqjdkjpn.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtwuxnawhm.html

[S27] C：定义常量
来源：http://hz.nwbrower.top/gtkmyqivgu.html

const double PI = 3.14159;
来源：http://hz.guannengcc.top/gtxaiqivat.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtcampxmtq.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtsrcurebw.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gtpohdlzfj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zycfv.cn/gtuuuwopqb.html

[S30] C：头文件保护
来源：http://hz.havefunace.top/gttazbqdhx.html

#ifndef X_H
来源：http://hz.jiagoushi.top/gtuomfgocn.html

#define X_H
来源：http://hz.ivvv.top/gtqhrvingz.html

#endif
来源：http://hz.jqgufenzy.top/gttdwwwkcw.html

[S31] C++：Hello World
来源：http://hz.iojbl.cn/gtgqzcdkvl.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtwaqskhda.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtttpoohws.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtryovktdp.html

std::string s = "hi";  s += "!";
来源：http://hz.iojbl.cn/gtcuyrjyza.html

[S33] C++：vector 增删
来源：http://hz.cdnleiting.top/gtmauuprtp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtpvzgbmho.html

[S34] C++：遍历 vector
来源：http://hz.snrcjt.cn/gtkfzvfsap.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtzfltuzny.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtowwepbcu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtbdhkzrok.html

[S36] C++：unordered_map
来源：http://hz.shuidangran.top/gtbwteivux.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtmybdxara.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtbdfjbgcg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtlgvgewpo.html

[S38] C++：排序
来源：http://hz.tian-w.cn/gtkirptpwx.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtznqjdqqd.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtoqpoisiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtlikkchkm.html

[S40] C++：查找元素
来源：http://hz.chenzaomai.com/gtnfijbupd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtcfytvvcs.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gteglfhvzs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtyjvuckcs.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtzthmfpqy.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhijiandao.cn/gttlibuwxm.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gttebmiapg.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtddlrmqis.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtyflyhzzs.html

void inc(int &x) { ++x; }
来源：http://hz.yangfankeji.com/gttuplttxb.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtwrwqtcip.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gtlpioilpy.html

[S46] C++：函数模板
来源：http://hz.yj20258888.top/gtmytbpirm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sysykeji.top/gtsegubuun.html

[S47] C++：结构化绑定遍历
来源：http://hz.yangfankeji.com/gtitrydlms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtwpvqvdxm.html

[S48] C++：逐行读文件
来源：http://hz.aibaodan.cn/gtshwcbhmk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cucudq.cn/gtnqkekuip.html

while (std::getline(in, line)) { }
来源：http://hz.xingfuxueyuan.xyz/gtecwqrwow.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtrsmfnzsv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gtlkjtjxyo.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gthufykkbh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtkibzyfvx.html

[S51] C++：显式类型转换
来源：http://hz.iojbl.cn/gtpcnmcppe.html

static_cast<double>(a) / b
来源：http://hz.jinqigufen.top/gtqfupaizd.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtnccaebul.html

int size() const noexcept { return n_; }
来源：http://hz.zycfv.cn/gtaaocgemy.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtcmckjtpv.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtgdqqstmp.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gtrxzlohwj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtbltondvd.html

[S55] C++：结构化绑定
来源：http://hz.xylfe.cn/gtsmvtmyjs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtapzqejvf.html

[S56] C++：optional
来源：http://hz.guowangkeji.top/gtnmlmbvov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinqigfzy.top/gtlulhpxbi.html

[S57] C++：编译期常量
来源：http://hz.gogol.net.cn/gtixvcyvse.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtzkdgnznm.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtfgfvldpj.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtufnzhnqf.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtvczdfjis.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtshozpmto.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtfbvgbkez.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinghuilouyu.cn/gtuqxtiodp.html

================================================================================
来源：http://hz.yueranfly.top/gtrutcswvx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtotfflktb.html

================================================================================
来源：http://hz.nwbrower.top/gtlxlkwklf.html

[T01] Kotlin：Hello World
来源：http://hz.redwolf501.top/gtkxlfzhch.html

println("Hello")
来源：http://hz.xziqi.cn/gtfpjbskbv.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtibcooowu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhiwuduotai.top/gtkgfqjwsy.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gttytqmdet.html

"值: $b"
来源：http://hz.yuxming.cn/gtwajdudws.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtpjepuwhn.html

val n: String? = null;  n?.length
来源：http://hz.ybcxt.top/gtcffjqnju.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gttwmxcnby.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj202588.top/gtmfuielrd.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtikbdgknd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtifmajvkg.html

[T07] Kotlin：集合过滤
来源：http://hz.zhiwuduotai.top/gtrvpxxuwu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.dashuyun.cn/gtaeftvgaz.html

[T08] Kotlin：数据类
来源：http://hz.guannengcc.top/gtkeqrwbbn.html

data class User(val name: String, val age: Int)
来源：http://hz.yj202588.top/gtvyazbgee.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtvvcabhcz.html

fun String.exclaim() = this + "!"
来源：http://hz.gaohongyu789.top/gtnfectihp.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtqvruwdpy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dashuyun.cn/gtugffjmtr.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtsbclhesr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuetiantiany.cn/gtaafntxjp.html

[T12] Kotlin：解构声明
来源：http://hz.yueranfly.top/gtffblpkwp.html

val (a, b) = Pair(1, 2)
来源：http://hz.svipenyu.cn/gtmcazksxy.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtmoxiqmrt.html

val m = mapOf("a" to 1)
来源：http://hz.shuidangran.top/gtypawkwce.html

[T14] Kotlin：循环
来源：http://hz.fengsongda.top/gtmgxjleuq.html

for (i in 1..10) println(i)
来源：http://hz.nanxuanxn.top/gtshdyuece.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtyjkbktxw.html

interface Shape { fun area(): Double }
来源：http://hz.pycfn.com/gtwdisuldp.html

[T16] Swift：Hello World
来源：http://hz.xuanzx.com/gtcuudylwx.html

print("Hello")
来源：http://hz.cdnleiting.top/gtpsopqdtw.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtwsdgvddc.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gtjudvrilh.html

[T18] Swift：字符串插值
来源：http://hz.zycfv.cn/gtofovfdbo.html

"值: \(b)"
来源：http://hz.zhengqikj.top/gtwmsjhsqk.html

[T19] Swift：可选绑定
来源：http://hz.birdmap.top/gthwigstmk.html

if let n = opt { print(n) }
来源：http://hz.nanxinkj.top/gtyzghjsyh.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtbczxxpua.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cqqwz.cn/gtduzpnuhm.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gthnuisbza.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtcxtjsmaq.html

[T22] Swift：字典
来源：http://hz.jinqigufen.top/gtmepvvngs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtpsmnvmyf.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtlxsgyzbg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtklpgscds.html

[T24] Swift：闭包
来源：http://hz.hysaishi.cn/gtcwkvgeca.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhixingplan.top/gtjuebqaxa.html

[T25] Swift：结构体
来源：http://hz.ydzc1.top/gtgcwblrup.html

struct P { var x: Int }
来源：http://hz.xylfe.cn/gtrkjmgkys.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gtokpdsnst.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtkifqfknc.html

[T27] Swift：错误处理
来源：http://hz.yueranfly.top/gtwoaefnmp.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtkccrfgum.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangkeji.top/gtdstxcjpd.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gtfpvoaamz.html

[T29] Swift：guard 提前返回
来源：http://hz.xylfe.cn/gtszrvlepp.html

guard let x = opt else { return }
来源：http://hz.hnqzz.top/gtqucxmhlm.html

[T30] Swift：协议
来源：http://hz.zdqjudy.top/gtlforrcnz.html

protocol Shape { func area() -> Double }
来源：http://hz.guowangkeji.top/gtxrwblkvy.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtpzyureuf.html

print("Hello")
来源：http://hz.zycfv.cn/gtoztbqlek.html

[T32] Lua：局部变量
来源：http://hz.dashuyun.cn/gtpjvmtpyu.html

local a = 1
来源：http://hz.andypj.xyz/gtjcawwjuy.html

[T33] Lua：表（数组）
来源：http://hz.cdnleiting.top/gtiioeanhm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gtnlabdlfk.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtgheiberp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cheryme.top/gtqfucvdak.html

[T35] Lua：字典表
来源：http://hz.mhx1999.top/gtmbfsupsp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.havefunace.top/gtdqwlzfrb.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtfcdyrrzk.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtpyjtkelg.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtwnkqjoyk.html

"a" .. "b"
来源：http://hz.zycfv.cn/gtpspwabvl.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gtwqqswera.html

if x > 0 then print("正") end
来源：http://hz.yonumen.top/gthupksekb.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtdxgrqnuw.html

string.find(s, "%d+")
来源：http://hz.sweek.top/gtavwoyepl.html

[T40] Lua：元表
来源：http://hz.hongshengwenyu.top/gtmicxmyit.html

setmetatable({}, { __index = base })
来源：http://hz.tian-w.cn/gtndlzgdlu.html

[T41] Perl：Hello World
来源：http://hz.xuanzx.com/gtrkzmwclg.html

print "Hello\n";
来源：http://hz.feifeiyinyue.top/gtaezpkcng.html

[T42] Perl：变量类型
来源：http://hz.hysaishi.cn/gtniynziza.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hysaishi.cn/gtgznlsxgl.html

[T43] Perl：字符串插值
来源：http://hz.guannengcc.top/gtaylbnlna.html

"值: $a"
来源：http://hz.ivvv.top/gtcxtouvsw.html

[T44] Perl：条件
来源：http://hz.ehwqpu.com/gtxtkuytdy.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtztlotkxu.html

[T45] Perl：数组遍历
来源：http://hz.guannengcc.top/gtbburwzmi.html

for my $x (@arr) { print $x; }
来源：http://hz.zhiwuduotai.top/gtflqdtjli.html

[T46] Perl：哈希操作
来源：http://hz.mhx1999.top/gttlsznitw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.c1oappe.top/gtojrsrcuw.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gthjisfjbk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hnqzz.top/gtevrtaefp.html

[T48] Perl：正则替换
来源：http://hz.chenlongwang.top/gtjxdswzkf.html

$s =~ s/old/new/g;
来源：http://hz.zdqjudy.top/gttmxlerlk.html

[T49] Perl：函数
来源：http://hz.gaohongyu789.top/gtwuevgoyh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gtwqgqwduk.html

[T50] Perl：逐行读文件
来源：http://hz.cqqwz.cn/gtbqozijci.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtzblpqewd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guannengcc.top/gtfejuwloh.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtxggtdcji.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtsanlrbtm.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtvhigohje.html

val a = 1;  var b = 2
来源：http://hz.jianghu66.top/gtymqaifsa.html

[T53] Scala：字符串插值
来源：http://hz.jlsjyb.cn/gtwelhxtxl.html

s"值: $b"
来源：http://hz.zhongyouzk.top/gtqjacwysq.html

[T54] Scala：集合映射
来源：http://hz.shangyingyoupin.top/gtjmdmsgqn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxinkj.top/gthftnjozu.html

[T55] Scala：集合过滤
来源：http://hz.xylfe.cn/gtlozdoucg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jyoumei.cn/gtzbohxjzc.html

[T56] Scala：样例类
来源：http://hz.cashguo.top/gtluygoyne.html

case class User(name: String, age: Int)
来源：http://hz.xinyue.icu/gtsmfdalxr.html

[T57] Scala：模式匹配
来源：http://hz.jinqigfzy.top/gtxwdjtpvd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cdnleiting.top/gtrtovuorm.html

[T58] Scala：函数定义
来源：http://hz.tanke756.top/gtvyyschce.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtuszacsch.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtlxuogfro.html

for (i <- 1 to 10) println(i)
来源：http://hz.guannengcc.top/gtjzotwwpc.html

[T60] Scala：折叠
来源：http://hz.yanxiufei.cn/gtfrzwokmd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hysaishi.cn/gtctqvfyrv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtiiuuvips.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gttysuutek.html

================================================================================
来源：http://hz.ybcxt.top/gtkrxhgnrl.html

[U01] Py：创建虚拟环境
来源：http://hz.snrcjt.cn/gtyxgvszby.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhongyouzk.top/gtqacvdlpt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zdqjudy.top/gtubtvazkl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhongyouzk.top/gtusfrttcy.html

[U03] Py：加载 .env 配置
来源：http://hz.meibo888.top/gttnglxeta.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.c1oappe.top/gtccudvwbi.html

[U04] Py：变量调试打印
来源：http://hz.kuanghao11.cn/gtlwzomrjx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtmsfcwbfz.html

[U05] Py：列表去重且保序
来源：http://hz.fengsongda.top/gtesavrrzu.html

list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtxwjspvbw.html

[U06] Py：合并两个字典
来源：http://hz.jianghu66.top/gtifbljwma.html

{**a, **b}
来源：http://hz.shzxlz.cn/gtzihxiydf.html

[U07] Py：反转字典键值
来源：http://hz.hnxiangtu.top/gtyenzifqx.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtmwbtnunr.html

[U08] Py：展平二维列表
来源：http://hz.yvedp.cn/gtclxigjkn.html

[y for x in nested for y in x]
来源：http://hz.yj202588.top/gtoibpelhm.html


<!-- 参考信息 -->