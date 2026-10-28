代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtokgzdmwl.html

[R66] 定时任务
来源：http://hz.hongshengwenyu.top/gtkubmdvad.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtxspyjfbx.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtirvfrzqj.html

openssl rand -hex 16
来源：http://hz.ivvv.top/gthbcreici.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtkkaezfth.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj20258888.top/gtllutvonx.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gtrilbncio.html

head -c 16 /dev/urandom | base64
来源：http://hz.sufxvd.cn/gtewcsehzw.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtcjwwiejn.html

date +%s;  date -d @1700000000
来源：http://hz.nanxuanxn.top/gtsybitdkx.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtpozvwvba.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtcmhjpjmy.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gtemvuplzc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtlawihoio.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gtyolcsliq.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtyqvyfusk.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtqytxrjvx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtinpvazhn.html

[R75] 导出环境变量
来源：http://hz.jqgfzy.top/gtxbejpxjm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cheryme.top/gtajpznxjd.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtnrwlgmho.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtqlumezjn.html

[R77] 读取用户输入
来源：http://hz.feifeiyinyue.top/gturdaclwz.html

read -rp "请输入: " ans
来源：http://hz.gogol.net.cn/gtdpgfffgo.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtlxbgaxek.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dianchejie.cn/gtkqelfpnq.html

[R79] 解析命令行选项
来源：http://hz.daria6918.cn/gttikpbcmj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.iojbl.cn/gtttnjpsob.html

[R80] 查看脚本执行耗时
来源：http://hz.jlsjyb.cn/gtohujfhpg.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtndyyqmri.html

================================================================================
来源：http://hz.c1oappe.top/gtvlgftqpx.html

S. C / C++ 专题
来源：http://hz.yueranfly.top/gttzurbiqt.html

================================================================================
来源：http://hz.yvedp.cn/gtngevoxzj.html

[S01] C：Hello World
来源：http://hz.zhongyouzk.top/gtegwmcoil.html

#include <stdio.h>
来源：http://hz.cqqwz.cn/gttahkcpsy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnqzz.top/gtsctgjocf.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtgbsmxnqw.html

int a = 10; printf("%d\n", a);
来源：http://hz.svipenyu.cn/gtjiwwykfo.html

[S03] C：读入整数
来源：http://hz.yvedp.cn/gtweeyaeth.html

int x; scanf("%d", &x);
来源：http://hz.fzhhl.top/gtspvwcqqv.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gtnmhqsznb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtnzrfzfwc.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtecjizupb.html

strlen(s)
来源：http://hz.daxiang520.top/gtpoxfrjrx.html

[S06] C：字符串比较
来源：http://hz.feifeiyinyue.top/gtpwaxbgkm.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtwqrykfvr.html

[S07] C：数组遍历求和
来源：http://hz.cucudq.cn/gtgprvrbtd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhongyouzk.top/gtfssotodx.html

[S08] C：动态内存分配与释放
来源：http://hz.sufxvd.cn/gtfhqzanjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtekpwrwdn.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gtlwasedom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtgvczqpzi.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gttastffax.html

int *p = &a;  *p = 5;
来源：http://hz.pycfn.com/gtehuwfvxv.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtwefnmrye.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtxnmweosl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gteibstjfl.html

fclose(f);
来源：http://hz.nanxinkj.top/gtbikdllbs.html

[S12] C：写文件
来源：http://hz.hammf.cn/gthxhehfib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gogol.net.cn/gtcbbthuce.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtjnqvmqiu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gtrymiqadj.html

[S14] C：枚举
来源：http://hz.jinqigfzy.top/gtlbcuivmi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtbakqofdn.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtrjlnxcyq.html

(double) a / b
来源：http://hz.nwbrower.top/gtigiuixdt.html

[S16] C：位操作置位
来源：http://hz.hywenlv.cn/gtclcyqrod.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtehqctgmc.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtfykatsgs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtunknsloj.html

[S18] C：命令行参数
来源：http://hz.shzxlz.cn/gtxpqljijq.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gtgqfzxwgh.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gteqfpkfrl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtfwsbqmhe.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtupbagyje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtbqfcztrq.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtslzohzaw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gthnfosagg.html

[S22] C：字符串转数字
来源：http://hz.hysaishi.cn/gttblczojm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zycfv.cn/gtlqydrpxq.html

[S23] C：随机数
来源：http://hz.gotoacloud.top/gtemtezfbw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.9152youxi.cn/gtrjhguwyq.html

[S24] C：获取本地时间
来源：http://hz.yuxming.cn/gtehunowqp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtuqkpuagw.html

[S25] C：内存拷贝
来源：http://hz.hfpthk.cn/gtbhxpdgzy.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtzoxiprmn.html

[S26] C：内存清零
来源：http://hz.hnqzz.top/gtqbxaogiz.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtgdlzqcfx.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtxcuquuvu.html

const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtxvrcvzfs.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtqsgveail.html

static int counter = 0;
来源：http://hz.fengsongda.top/gtmnbtrwln.html

[S29] C：变参函数
来源：http://hz.sysykeji.top/gtrcszacky.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gteceqcpxx.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtkcvizldk.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtdztgudsj.html

#define X_H
来源：http://hz.sufxvd.cn/gtonhhsiuc.html

#endif
来源：http://hz.chenjidiqi.icu/gtnqdzohku.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtgbdggofe.html

#include <iostream>
来源：http://hz.fzhhl.top/gtmyrzqyyg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenlongwang.top/gtrvkptwjh.html

[S32] C++：字符串
来源：http://hz.hnqzz.top/gtrtbeacuf.html

std::string s = "hi";  s += "!";
来源：http://hz.andypj.xyz/gtgnpmljai.html

[S33] C++：vector 增删
来源：http://hz.redwolf501.top/gtcdztsgdd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtfualyrya.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtmsyghbmf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtyxbaqksu.html

[S35] C++：map
来源：http://hz.zhiwuduotai.top/gtlajvqqya.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtjjejtupi.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtdqbnozng.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtmxwinptd.html

[S37] C++：set
来源：http://hz.jinyuanbaomall.cn/gthdehdytx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gtoenrhfta.html

[S38] C++：排序
来源：http://hz.yuanzhike.top/gtbmxydmjk.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtcrdbdddu.html

[S39] C++：自定义比较器排序
来源：http://hz.zhaomingkeji.xyz/gtouuoiqii.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.birdmap.top/gtzaumqyxq.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtnylzonfs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtkwyupnzn.html

[S41] C++：类与构造函数
来源：http://hz.sufxvd.cn/gtufulgtjh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtytjydcrr.html

[S42] C++：继承与虚函数
来源：http://hz.gaohongyu789.top/gtlgullrdm.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtjvucrhtm.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gttiauknau.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtqvkyhcsj.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtmmexmiud.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gtzzaptnxu.html

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtewnbjxme.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.svipenyu.cn/gtnleqbqcf.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtfuvkzcos.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangdashe.top/gtsoyewdxj.html

[S47] C++：结构化绑定遍历
来源：http://hz.zycfv.cn/gtnjxkahed.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxuanxn.top/gtiuoeozzv.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gtcakxgiaz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhengqikj.top/gtyrfpscda.html

while (std::getline(in, line)) { }
来源：http://hz.yanxiufei.cn/gtfodiaufz.html

[S49] C++：写文件
来源：http://hz.aizwys.cn/gtqkrttwgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtkechusoj.html

[S50] C++：格式化数字
来源：http://hz.cucudq.cn/gtgpztajrc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gttffqpias.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtfrkzunwm.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtiwiyiaqz.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtfwvaruxd.html

int size() const noexcept { return n_; }
来源：http://hz.vqdsnc.cn/gtmxhwybtc.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gtufdsrpqi.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtfajsjmhe.html

[S54] C++：异常处理
来源：http://hz.fzhhl.top/gtgwekbysq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangkeji.top/gtspdomfnz.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtpuudcfiq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtzojkkktk.html

[S56] C++：optional
来源：http://hz.guannengcc.top/gtastrztlq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gthwulaghh.html

[S57] C++：编译期常量
来源：http://hz.xziqi.cn/gtzyodtjzd.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtpejgkggu.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtqrmsevtk.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtkdtseugy.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtfwbmbkcn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtgfbbbteq.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtebezzdbl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gtrjrodpvl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpmfbiwzw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtgjptxxkq.html

================================================================================
来源：http://hz.daxiang520.top/gtmfrnuzze.html

[T01] Kotlin：Hello World
来源：http://hz.c1oappe.top/gtuzhishgz.html

println("Hello")
来源：http://hz.nwbrower.top/gthynxlkyn.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtuitqycjl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtdiclkqih.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gtubnvteke.html

"值: $b"
来源：http://hz.yongpay.top/gtwvcjyvps.html

[T04] Kotlin：空安全
来源：http://hz.daria6918.cn/gtpjhcqzqc.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtiawzxozn.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtinoweacz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hongshengwenyu.top/gtenicawfa.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtfssfcjps.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gtldxspebi.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gtnywyhnxh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxinkj.top/gtfivljrhe.html

[T08] Kotlin：数据类
来源：http://hz.yangfankeji.com/gtuoiugdla.html

data class User(val name: String, val age: Int)
来源：http://hz.shangyingyoupin.top/gtjyxozqik.html

[T09] Kotlin：扩展函数
来源：http://hz.sysykeji.top/gtwygjvygg.html

fun String.exclaim() = this + "!"
来源：http://hz.chenlongwang.top/gtylnzkqxh.html

[T10] Kotlin：默认参数
来源：http://hz.chenzaomai.com/gthxvxnztl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gtogqrwdgj.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtzbakjkko.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yongpay.top/gtauyessrd.html

[T12] Kotlin：解构声明
来源：http://hz.snrcjt.cn/gtxtdeidhs.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtzskxrtwd.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgfzy.top/gtrzshqrzv.html

val m = mapOf("a" to 1)
来源：http://hz.jyoumei.cn/gtfgqqmpmh.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gtdfbrljlm.html

for (i in 1..10) println(i)
来源：http://hz.jyoumei.cn/gtcnclztdx.html

[T15] Kotlin：接口
来源：http://hz.zhijiandao.cn/gtubjceoyk.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtngvsbhof.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtofkigavj.html

print("Hello")
来源：http://hz.hnqzz.top/gtskahiloz.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gtpjrvkvyw.html

var a = 1;  let b = 2
来源：http://hz.aibaodan.cn/gtcddchdnq.html

[T18] Swift：字符串插值
来源：http://hz.hywenlv.cn/gtzhimxkto.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtirhbjmzk.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtivulzhjs.html

if let n = opt { print(n) }
来源：http://hz.jinqigfzy.top/gthvklewrg.html

[T20] Swift：数组操作
来源：http://hz.chenlongwang.top/gthvlgnioz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtlwhtmzny.html

[T21] Swift：遍历
来源：http://hz.hfpthk.cn/gtrtuqtjct.html

for x in a { print(x) }
来源：http://hz.ydjk.org.cn/gtehcllprw.html

[T22] Swift：字典
来源：http://hz.xylfe.cn/gtznxyfdju.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtbyatveyd.html

[T23] Swift：函数
来源：http://hz.gzhubu.top/gtvrjwtupp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtjlkobqpg.html

[T24] Swift：闭包
来源：http://hz.gaohongyu789.top/gtsfvsreqz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtprhlqaip.html

[T25] Swift：结构体
来源：http://hz.zhixingplan.top/gtceasckpo.html

struct P { var x: Int }
来源：http://hz.xylfe.cn/gtxiicuqqc.html

[T26] Swift：类与重写
来源：http://hz.hongshengwenyu.top/gtateqaomq.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtpxfnuyid.html

[T27] Swift：错误处理
来源：http://hz.yvedp.cn/gtndfwbujg.html

do { try f() } catch { print(error) }
来源：http://hz.zhongyouzk.top/gtuelumcfg.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtoerjdtzw.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gthsbxeabg.html

[T29] Swift：guard 提前返回
来源：http://hz.ivvv.top/gtrtnqrrtj.html

guard let x = opt else { return }
来源：http://hz.gotoacloud.top/gtambiywol.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtrmlqdtjv.html

protocol Shape { func area() -> Double }
来源：http://hz.xingfuxueyuan.xyz/gthdrdsdyo.html

[T31] Lua：Hello World
来源：http://hz.cashguo.top/gtbopqsmda.html

print("Hello")
来源：http://hz.shzxlz.cn/gtibnstybz.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtakiuahos.html

local a = 1
来源：http://hz.dianchejie.cn/gtvvkkfqdq.html

[T33] Lua：表（数组）
来源：http://hz.birdmap.top/gtvphtrjtu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cdnleiting.top/gtihfcjhfk.html

[T34] Lua：遍历表
来源：http://hz.tian-w.cn/gtwfwptmva.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yongpay.top/gtemniplsj.html

[T35] Lua：字典表
来源：http://hz.hysaishi.cn/gtyhmxpakk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gtuhedifxm.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtomisnorn.html

function add(a, b) return a + b end
来源：http://hz.sxryk.cn/gtxhgdmyvt.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtjdgwramf.html

"a" .. "b"
来源：http://hz.xuanzx.com/gtquofcblh.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gtoapftoye.html

if x > 0 then print("正") end
来源：http://hz.gaohongyu789.top/gtqbqxkoos.html

[T39] Lua：模式匹配
来源：http://hz.nanxinkj.top/gtgfrynplq.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtodelprwk.html

[T40] Lua：元表
来源：http://hz.tianlin.xyz/gtsbbfgwrq.html

setmetatable({}, { __index = base })
来源：http://hz.cashguo.top/gtgydfryfx.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangtech.top/gtiljjymsn.html

print "Hello\n";
来源：http://hz.quarkkingdee.top/gtxudcvdvg.html

[T42] Perl：变量类型
来源：http://hz.xingfuxueyuan.xyz/gtgmjwvcan.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guannengcc.top/gtmpdvcomm.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtpgiufmni.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gttgegeapq.html

[T44] Perl：条件
来源：http://hz.chenzaomai.com/gtrdmjvlex.html

if ($a > 0) { print "正"; }
来源：http://hz.jiagoushi.top/gtbjvutwfa.html

[T45] Perl：数组遍历
来源：http://hz.tianlin.xyz/gtglofdiis.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtpnyxayur.html

[T46] Perl：哈希操作
来源：http://hz.chenlongwang.top/gtbbxkhbmk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangkeji.top/gtzmqdwnrt.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtpcqsesrs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.quarkkingdee.top/gtvcmakosn.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtdqtsigyg.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gtkzbvlbkj.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtkpcwsxbe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gteeapxysg.html

[T50] Perl：逐行读文件
来源：http://hz.cashguo.top/gtuiklegfz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenzaomai.com/gtqcnpjbyk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtngpswgvb.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtglsbkmjz.html

println("Hello")
来源：http://hz.ydzc1.top/gtquxmpcvf.html

[T52] Scala：变量
来源：http://hz.hongshengwenyu.top/gtiodwmqvk.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gtxburzwox.html

[T53] Scala：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtrytabwis.html

s"值: $b"
来源：http://hz.snrcjt.cn/gtlsqjgxtl.html

[T54] Scala：集合映射
来源：http://hz.ivvv.top/gtegxakjcw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuanzx.com/gtvzfqlekl.html

[T55] Scala：集合过滤
来源：http://hz.guowangkeji.top/gtqzblohvq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shuidangran.top/gtdkowdqxr.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtqashodwi.html

case class User(name: String, age: Int)
来源：http://hz.zhiwuduotai.top/gthmdusbms.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gttvoaleux.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nwbrower.top/gtzhxoqcxb.html

[T58] Scala：函数定义
来源：http://hz.ybcxt.top/gtcbkvvadu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtwlenimsx.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtwizdoeoz.html

for (i <- 1 to 10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtnqgebaje.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtmagxwbho.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gtgqngoclk.html

================================================================================
来源：http://hz.birdmap.top/gtovjqcmte.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtcgqmesif.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpdnkxpkb.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxinkj.top/gtgipzvapj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shzxlz.cn/gthlzjreap.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhengqikj.top/gtbbaiycgx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tian-w.cn/gtgpmwxpad.html

[U03] Py：加载 .env 配置
来源：http://hz.0kj1m.cn/gtpbxhpbhg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hywenlv.cn/gtsfektdzh.html

[U04] Py：变量调试打印
来源：http://hz.dianchejie.cn/gtrrmanvqh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxinkj.top/gtmsyxpbxc.html

[U05] Py：列表去重且保序
来源：http://hz.yuanzhike.top/gtkdgxsjbl.html

list(dict.fromkeys(arr))
来源：http://hz.gaohongyu789.top/gtkfsrcgos.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtefvbxzce.html

{**a, **b}
来源：http://hz.guowangkeji.top/gtcrcwfedb.html


<!-- 参考信息 -->