代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.gogol.net.cn/gtrqkmivpf.html

[R64] 结束进程
来源：http://hz.nanxinkj.top/gtqsowdvtd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guannengcc.top/gtfsnaqnzx.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtmstpdptg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gttgupkder.html

[R66] 定时任务
来源：http://hz.nanxuanxn.top/gtjqmlwbox.html

crontab -e;  crontab -l
来源：http://hz.shzxlz.cn/gtbizfnsay.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gtamupnjhg.html

openssl rand -hex 16
来源：http://hz.gzhubu.top/gttlpivbvr.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtlxtjnofp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gttwyoktwi.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtgatqwjxc.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangkeji.top/gtiljwqxgu.html

[R70] 时间戳与互转
来源：http://hz.sufxvd.cn/gtmgiqfkoe.html

date +%s;  date -d @1700000000
来源：http://hz.zhiwuduotai.top/gtskcigfzi.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gtlkeedfzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtvomhbkii.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gtwnuojkwc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtqiinhdry.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtfmrcykkr.html

split -l 1000 big.log part_
来源：http://hz.daria6918.cn/gtbutwybzp.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gtlfhjthjo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtuuexxpvo.html

[R75] 导出环境变量
来源：http://hz.xinyue.icu/gthjnycwxy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtvfncnnaq.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtivxqiipb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtiolqilow.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtgkybrkzd.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtaveimzvd.html

[R78] 交互式菜单
来源：http://hz.tian-w.cn/gtzrdnftfq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtndefywrh.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gtmbpyzqrm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gtygheuokc.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtsxfdpbep.html

time ./run.sh
来源：http://hz.aibaodan.cn/gtdbvojvte.html

================================================================================
来源：http://hz.bjfxy.top/gtudtceupk.html

S. C / C++ 专题
来源：http://hz.shuidangran.top/gtscfxcbro.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwsudhegn.html

[S01] C：Hello World
来源：http://hz.chenlongwang.top/gtrhgaqwcg.html

#include <stdio.h>
来源：http://hz.fzhhl.top/gtlsdsgsff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.svipenyu.cn/gtvbtqzsdb.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gthnoflpka.html

int a = 10; printf("%d\n", a);
来源：http://hz.yangfankeji.com/gtiqynggxc.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtkmsgohua.html

int x; scanf("%d", &x);
来源：http://hz.zhijiandao.cn/gtvxzmeueg.html

[S04] C：字符串复制
来源：http://hz.ehwqpu.com/gtwbrlpfen.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gotoacloud.top/gttjtgzssw.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gthzxaluuo.html

strlen(s)
来源：http://hz.chenzaomai.com/gtrqworfle.html

[S06] C：字符串比较
来源：http://hz.ydjk.org.cn/gtpizrwalg.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gtjdsypnqg.html

[S07] C：数组遍历求和
来源：http://hz.smart0.xyz/gttokzbdxf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.birdmap.top/gtieoxkcgv.html

[S08] C：动态内存分配与释放
来源：http://hz.hysaishi.cn/gtdcapfomw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gthtbwybqj.html

[S09] C：结构体定义与初始化
来源：http://hz.smart0.xyz/gthruojfvi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtrhbnygmz.html

[S10] C：指针与解引用
来源：http://hz.zhoulong.xyz/gtoomnhior.html

int *p = &a;  *p = 5;
来源：http://hz.ywan-chungtsiang.top/gtjtwynlyc.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtrgcabtzg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtmnecbiew.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenlongwang.top/gtmqtartib.html

fclose(f);
来源：http://hz.yj202588.top/gtfahmzzay.html

[S12] C：写文件
来源：http://hz.pengpengdd.cyou/gtohzhprcs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtelxozwpv.html

[S13] C：宏定义
来源：http://hz.pycfn.com/gtgnlaitzr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.0kj1m.cn/gtgamotzrt.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtmngamdjd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtwjbpooys.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtyukssvtu.html

(double) a / b
来源：http://hz.shangyingyoupin.top/gtfovpxnam.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtyiidwjwx.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtdpzmrgdo.html

[S17] C：安全拼接字符串
来源：http://hz.dashuyun.cn/gtticjnwkf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yangfankeji.com/gtclxqgbsr.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtvnfjtskm.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtvtunrsnj.html

[S19] C：快速排序
来源：http://hz.zhaomingkeji.xyz/gthtfliuhl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtpubepwaq.html

[S20] C：二分查找
来源：http://hz.fzhhl.top/gtdcrlwloy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtqorzolmi.html

[S21] C：字符类别判断
来源：http://hz.cdnleiting.top/gtxrqbhyrz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtidboixtq.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtbrwqbgum.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhoulong.xyz/gtwfvasesf.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtifityfbb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hammf.cn/gtsecmawjz.html

[S24] C：获取本地时间
来源：http://hz.wangshuangyany.cn/gtxxiybhje.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtlbxuxaiq.html

[S25] C：内存拷贝
来源：http://hz.daxiang520.top/gtlyinsrpq.html

memcpy(dst, src, n);
来源：http://hz.nanxinkj.top/gtkcjvfqht.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtqucgmosu.html

memset(a, 0, sizeof a);
来源：http://hz.redwolf501.top/gttyjppapm.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gtlmxayabo.html

const double PI = 3.14159;
来源：http://hz.havefunace.top/gtuehpbucs.html

[S28] C：静态变量
来源：http://hz.jinyuanbaomall.cn/gttdjfxkhc.html

static int counter = 0;
来源：http://hz.yvedp.cn/gtlqyojkhp.html

[S29] C：变参函数
来源：http://hz.yj20258888.top/gtqagnwcsh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sxryk.cn/gtgxqhvdzo.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtokpwiyhj.html

#ifndef X_H
来源：http://hz.aizwys.cn/gthusgvdzt.html

#define X_H
来源：http://hz.zycfv.cn/gttqatwils.html

#endif
来源：http://hz.daxiang520.top/gtufcfvdfn.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gtnwmpjusy.html

#include <iostream>
来源：http://hz.daxiang520.top/gtsribaxgb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtivaxeqaj.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gtnpvpyeku.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtdydwnrnw.html

[S33] C++：vector 增删
来源：http://hz.ivvv.top/gtpubmjbks.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtcfgcgunj.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtxslngmnk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xziqi.cn/gtnrwhmeib.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtkgwsxhnc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtbpstqnef.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtpjlhhsip.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtvxkxouxq.html

[S37] C++：set
来源：http://hz.sufxvd.cn/gtgpyadybg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yonumen.top/gtcxkfclxa.html

[S38] C++：排序
来源：http://hz.xingfuxueyuan.xyz/gthjemfonr.html

std::sort(v.begin(), v.end());
来源：http://hz.daxiang520.top/gtxweisevi.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtfmlawylm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtgrkzkxbg.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtatnkwvwk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtjmnthuwy.html

[S41] C++：类与构造函数
来源：http://hz.mhx1999.top/gthgnkaxpi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtyrelbapn.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtwdewwjcz.html

class B : public Base { public: void f() override {} };
来源：http://hz.guannengcc.top/gtsbzrfcvw.html

[S43] C++：智能指针
来源：http://hz.hnqzz.top/gtisfajdoh.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtzueoojfc.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gtvbgfhfjj.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtjivkyaym.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gthseigtgx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtdjzpshll.html

[S46] C++：函数模板
来源：http://hz.shuidangran.top/gtrvafdtmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtmdcdtrfu.html

[S47] C++：结构化绑定遍历
来源：http://hz.haohaochexian.top/gtkjqloqhi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj202588.top/gtmbthmmlc.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gthskhibju.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guowangkeji.top/gtzwewrakh.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtpvyradna.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtrymwjdlb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtnwauoiou.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtkneomlha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yvedp.cn/gtrmppnkwj.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtkefhccqa.html

static_cast<double>(a) / b
来源：http://hz.jinqigfzy.top/gtaloouxkb.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtwoaswhnx.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtudlvyzya.html

[S53] C++：移动语义
来源：http://hz.mhx1999.top/gtrtkqnsld.html

std::vector<int> w = std::move(v);
来源：http://hz.aibaodan.cn/gtvccordjo.html

[S54] C++：异常处理
来源：http://hz.hfpthk.cn/gtiqaaefpy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gtggmdelmy.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtguvugefh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtwocfszyn.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtjgycqbbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gtqfyvgrxw.html

[S57] C++：编译期常量
来源：http://hz.jinghuilouyu.cn/gtszwtgmru.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtjdengrhu.html

[S58] C++：命名空间
来源：http://hz.xingfuxueyuan.xyz/gtbeejqwqa.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtxxgszocu.html

[S59] C++：静态断言
来源：http://hz.snrcjt.cn/gtmpmqufwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtyxfgcnfi.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtvqdgfmlv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.52xcode.cn/gtggnfjahf.html

================================================================================
来源：http://hz.cdnleiting.top/gtrtfuimcx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtpdunsqgv.html

================================================================================
来源：http://hz.ppjwa.cn/gtkhdizxbh.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtfugsygwb.html

println("Hello")
来源：http://hz.yuxming.cn/gtpgrperux.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtdcyuyayp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtxydkiikh.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gtgtggxgno.html

"值: $b"
来源：http://hz.zycfv.cn/gtpqunlkht.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gthuyqftsu.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtgabirjcr.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtyatjgfef.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtwgukwedf.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gtbsuttnrb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtnxlrkglt.html

[T07] Kotlin：集合过滤
来源：http://hz.gzhubu.top/gtlswhepkw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtpmasaquf.html

[T08] Kotlin：数据类
来源：http://hz.tian-w.cn/gtfbsdrkdn.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gtfwynakzg.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtrqesntwn.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtmsdirzrm.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtmaptixvx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gtkphytouw.html

[T11] Kotlin：协程
来源：http://hz.jlsjyb.cn/gtaaoycoqn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtafqnupnv.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtpkgegufh.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtzvdplatd.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtmssnxsky.html

val m = mapOf("a" to 1)
来源：http://hz.sweek.top/gtuqhggdnm.html

[T14] Kotlin：循环
来源：http://hz.aizwys.cn/gtgbhyukum.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtghqahasa.html

[T15] Kotlin：接口
来源：http://hz.zhiwuduotai.top/gtkstitnah.html

interface Shape { fun area(): Double }
来源：http://hz.smart0.xyz/gtbfwvzerk.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtqlvqwups.html

print("Hello")
来源：http://hz.gzhubu.top/gtpkfsawnm.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtlmesechu.html

var a = 1;  let b = 2
来源：http://hz.yonumen.top/gtfkdyeeax.html

[T18] Swift：字符串插值
来源：http://hz.andypj.xyz/gtrsoddjqr.html

"值: \(b)"
来源：http://hz.aibaodan.cn/gtwlmgadwp.html

[T19] Swift：可选绑定
来源：http://hz.gogol.net.cn/gtbtxftipt.html

if let n = opt { print(n) }
来源：http://hz.shzxlz.cn/gtucpjapva.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gtymntplqd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ywan-chungtsiang.top/gthrwmnyrt.html

[T21] Swift：遍历
来源：http://hz.shanyushiyangkeji.top/gtnwugkhhy.html

for x in a { print(x) }
来源：http://hz.bjfxy.top/gtudrwnswk.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gtdbdgotfd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yangfankeji.com/gtnvuklimx.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtxlatlclc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuanzhike.top/gtggkuezqq.html

[T24] Swift：闭包
来源：http://hz.zhengqikj.top/gthbdgsqwn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtixiudxzj.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtjqqjlcuz.html

struct P { var x: Int }
来源：http://hz.pycfn.com/gtudjilduz.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gthkkpqkld.html

class A: Base { override func f() {} }
来源：http://hz.9152youxi.cn/gtcdvtgfdg.html

[T27] Swift：错误处理
来源：http://hz.birdmap.top/gtlsbqknbg.html

do { try f() } catch { print(error) }
来源：http://hz.nwbrower.top/gtjpegvojf.html

[T28] Swift：枚举
来源：http://hz.hnxiangtu.top/gtzbgrcggv.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gtnwmbayik.html

[T29] Swift：guard 提前返回
来源：http://hz.cashguo.top/gtrakjbwoe.html

guard let x = opt else { return }
来源：http://hz.aizwys.cn/gtkskqqruk.html

[T30] Swift：协议
来源：http://hz.sxryk.cn/gtsnjxtdob.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtzdqwjhbm.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gtoknylziw.html

print("Hello")
来源：http://hz.kuanghao11.cn/gthnrpgfqu.html

[T32] Lua：局部变量
来源：http://hz.gzhubu.top/gtizfzjdyw.html

local a = 1
来源：http://hz.sufxvd.cn/gttofsvkdm.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtgbhsfetp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtdormnmel.html

[T34] Lua：遍历表
来源：http://hz.ydzc1.top/gtnqxnqzkt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xylfe.cn/gtuegitwjy.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtvbrzrnqa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gtbqvfjwwi.html

[T36] Lua：函数
来源：http://hz.jqgufenzy.top/gtdubqxked.html

function add(a, b) return a + b end
来源：http://hz.hywenlv.cn/gteaybclvm.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gtjxgugwaz.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtdsgdljbp.html

[T38] Lua：条件
来源：http://hz.cashguo.top/gtxthjcphv.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtbteydjiu.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtkezktseg.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtxpkdwwam.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gtcxgpjqyx.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtrhqeiogo.html

[T41] Perl：Hello World
来源：http://hz.feifeiyinyue.top/gtgjtwafyv.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtgpeqnqan.html

[T42] Perl：变量类型
来源：http://hz.tianlin.xyz/gtpbfyembm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yangfankeji.com/gtpipjjiml.html

[T43] Perl：字符串插值
来源：http://hz.pycfn.com/gtydsiurcv.html

"值: $a"
来源：http://hz.nanxinkj.top/gtqmbvkkpt.html

[T44] Perl：条件
来源：http://hz.havefunace.top/gtzwcznprb.html

if ($a > 0) { print "正"; }
来源：http://hz.zhoulong.xyz/gtbvpdcxna.html

[T45] Perl：数组遍历
来源：http://hz.smart0.xyz/gtovfkgsci.html

for my $x (@arr) { print $x; }
来源：http://hz.iojbl.cn/gtyrrzcpyj.html

[T46] Perl：哈希操作
来源：http://hz.snrcjt.cn/gttwsnmgai.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daria6918.cn/gtdlamvftg.html

[T47] Perl：正则捕获
来源：http://hz.daxiang520.top/gtxzsmliqy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pengpengdd.cyou/gtrsoemash.html

[T48] Perl：正则替换
来源：http://hz.andypj.xyz/gtkdfwzaqa.html

$s =~ s/old/new/g;
来源：http://hz.guowangkeji.top/gtnaqeygqm.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtpuhbwudu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gthdaefclh.html

[T50] Perl：逐行读文件
来源：http://hz.hnqzz.top/gtizuhwhza.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.mhx1999.top/gtwidgsocz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtthvuuvru.html

[T51] Scala：Hello World
来源：http://hz.haohaochexian.top/gtaibnsmjy.html

println("Hello")
来源：http://hz.yj20258888.top/gtgqskuenb.html

[T52] Scala：变量
来源：http://hz.hammf.cn/gtyqjbomon.html

val a = 1;  var b = 2
来源：http://hz.jinqigufen.top/gtjoengcyo.html

[T53] Scala：字符串插值
来源：http://hz.yvedp.cn/gtfxkqmhpt.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtfzdezjln.html

[T54] Scala：集合映射
来源：http://hz.dashuyun.cn/gtnbgrtuzx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tian-w.cn/gtixggtajq.html

[T55] Scala：集合过滤
来源：http://hz.ivvv.top/gtjpedyxio.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ehwqpu.com/gtxuykoscd.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtipvvojjo.html

case class User(name: String, age: Int)
来源：http://hz.kuanghao11.cn/gtjejtazzc.html

[T57] Scala：模式匹配
来源：http://hz.fzhhl.top/gtzboyxnde.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gogol.net.cn/gtphqlohvz.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtrutciwle.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtucmpzunf.html

[T59] Scala：循环
来源：http://hz.xziqi.cn/gtpqmgfivy.html

for (i <- 1 to 10) println(i)
来源：http://hz.guowangkeji.top/gtgpnujqel.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gtycihabgz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ywan-chungtsiang.top/gtcsjsbqzo.html

================================================================================
来源：http://hz.gogol.net.cn/gtxlsmctnc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangkeji.top/gtnhymvcgg.html

================================================================================
来源：http://hz.nanxinkj.top/gthifozosx.html

[U01] Py：创建虚拟环境
来源：http://hz.gotoacloud.top/gthqiwbimo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ivvv.top/gtuqbmyzbo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.mhx1999.top/gtqohjkirb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hammf.cn/gtsbpsfxgk.html

[U03] Py：加载 .env 配置
来源：http://hz.tianlin.xyz/gtyyqrwiqx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jlsjyb.cn/gtrgpicvcl.html

[U04] Py：变量调试打印
来源：http://hz.guannengcc.top/gtwzxnudqv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hnqzz.top/gttrrmpnip.html


<!-- 参考信息 -->