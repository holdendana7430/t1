代发 wailian999

df -h;  du -sh *
来源：http://hz.dianchejie.cn/gtkpjhssxl.html

[R62] 找最占空间的文件
来源：http://hz.yangfankeji.com/gtijiueobq.html

du -ah . | sort -rh | head -10
来源：http://hz.jyoumei.cn/gtoqhkaaqu.html

[R63] 内存与进程
来源：http://hz.shanyushiyangtech.top/gtgsknxaef.html

free -h;  ps aux | grep nginx
来源：http://hz.jinghuilouyu.cn/gtnnlpnrhg.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtujizlcup.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj202588.top/gtfrntxtat.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtiempfpnn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.vqdsnc.cn/gtbkxwqgye.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtljathagb.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtsyvgfifz.html

[R67] 生成随机十六进制串
来源：http://hz.jinghuilouyu.cn/gtaftaeptm.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gtbgppjbuj.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gtyfrmrbfm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gtnrvsaebi.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtddxyceqw.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtavxedxgg.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gthkndymos.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtwrhssjbt.html

[R71] 日期格式化
来源：http://hz.cheryme.top/gtgxczgkax.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtfeafyrls.html

[R72] 等待端口就绪
来源：http://hz.chenlongwang.top/gthzabadmv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtzhrtgibe.html

[R73] 分割大日志
来源：http://hz.gaohongyu789.top/gtducfxyfr.html

split -l 1000 big.log part_
来源：http://hz.yvedp.cn/gtzpfbdefq.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtsfmonnqa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shuidangran.top/gtkwczkwjq.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtwxvbzqrd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xingfuxueyuan.xyz/gtayfffjpj.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtvhvgbavl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtbhpeyrfp.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtxbsfttml.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gtxzbteggu.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtkptlqine.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtojikmlhl.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtebfmvtdq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtbcisdyes.html

[R80] 查看脚本执行耗时
来源：http://hz.xylfe.cn/gtbnupipby.html

time ./run.sh
来源：http://hz.yangfankeji.com/gthutruqtn.html

================================================================================
来源：http://hz.jiagoushi.top/gttnzldgoz.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtllaentak.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtoeaoqweg.html

[S01] C：Hello World
来源：http://hz.zycfv.cn/gtwwqknubc.html

#include <stdio.h>
来源：http://hz.yangfankeji.com/gtspnbnpre.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.birdmap.top/gtqzqafoyc.html

[S02] C：变量与格式化输出
来源：http://hz.tianlin.xyz/gtvkabdumq.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtckcitpjm.html

[S03] C：读入整数
来源：http://hz.pycfn.com/gtlxvpinmm.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtfamhwlfx.html

[S04] C：字符串复制
来源：http://hz.yuanzhike.top/gtqydotmqd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gogol.net.cn/gteemhqvfd.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gtukxqyvsm.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtgvukerap.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtrndvoanr.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtybzpoovb.html

[S07] C：数组遍历求和
来源：http://hz.gaohongyu789.top/gtrldskepl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtsqrcwbti.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtumigbsfx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gthvptlkjv.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtxrsaqecr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtjtsuiwun.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtcawpoosv.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtuyrarcke.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtvjtoesbt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtyxrhgzzp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtpvbeeseq.html

fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtafwgbatd.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtroqwlttr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtwjphpazg.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtavpaswey.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtwnurktsu.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtftcyhdgb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gttontqbbs.html

[S15] C：类型转换
来源：http://hz.jyoumei.cn/gthdsxzfpl.html

(double) a / b
来源：http://hz.andypj.xyz/gtucxwvqje.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtwkuutxfq.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtbsrjfupt.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gthdoyfzjd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cheryme.top/gtkfycrdfx.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtsppmjcml.html

int main(int argc, char **argv)
来源：http://hz.havefunace.top/gtucmywlul.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtisfnhnwn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtvcyuvtyr.html

[S20] C：二分查找
来源：http://hz.yongpay.top/gtzujvxfzy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gttgkwhzuw.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtdramkpuq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nwbrower.top/gtlqgcjmaf.html

[S22] C：字符串转数字
来源：http://hz.kuanghao11.cn/gtuiboxdmb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gttgtkvmwy.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtvsukvtvp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guannengcc.top/gtruwidxzs.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gttfcojikf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuetiantiany.cn/gtzpknyaon.html

[S25] C：内存拷贝
来源：http://hz.feifeiyinyue.top/gtfisrllxw.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtayvflbvy.html

[S26] C：内存清零
来源：http://hz.kuanghao11.cn/gthnluqull.html

memset(a, 0, sizeof a);
来源：http://hz.hammf.cn/gtkasmnawv.html

[S27] C：定义常量
来源：http://hz.hongshengwenyu.top/gtfrtqnxbh.html

const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gttomvzmcb.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gtwihefeiy.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gtuxadkwjb.html

[S29] C：变参函数
来源：http://hz.yuanzhike.top/gtrjrjxufq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gotoacloud.top/gtqigylrlq.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtgnazqhpm.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtvofbpxpe.html

#define X_H
来源：http://hz.jinqigufen.top/gtgfiohmpx.html

#endif
来源：http://hz.feifeiyinyue.top/gtjwzficnq.html

[S31] C++：Hello World
来源：http://hz.xinyue.icu/gtwlfwaqtz.html

#include <iostream>
来源：http://hz.ybcxt.top/gturdekbcj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtfodvqitw.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gtwcxnhbpk.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtxfxmhlnt.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtyalwbdvh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cheryme.top/gtcphruqiw.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtgdkywvuk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gtxjitdtlr.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtansjhqrd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtjcaigtkf.html

[S36] C++：unordered_map
来源：http://hz.nanxuanxn.top/gtxwzaugca.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtlrtwnubm.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtymwchujs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nwbrower.top/gtaiackigx.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtmhxmakiy.html

std::sort(v.begin(), v.end());
来源：http://hz.andypj.xyz/gtozibbopb.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtumfizaek.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtbjbaahxw.html

[S40] C++：查找元素
来源：http://hz.hywenlv.cn/gtvtuozian.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gtdzlzehgu.html

[S41] C++：类与构造函数
来源：http://hz.tanke756.top/gtvqpnnvvh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.redwolf501.top/gttkaozfgl.html

[S42] C++：继承与虚函数
来源：http://hz.zhixingplan.top/gtoylxihjm.html

class B : public Base { public: void f() override {} };
来源：http://hz.cheryme.top/gttgacmgsi.html

[S43] C++：智能指针
来源：http://hz.jianghu66.top/gtlbnnnudl.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtwecultea.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtgembmetn.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gteboptxqu.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtiotitilo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.andypj.xyz/gtneubpptc.html

[S46] C++：函数模板
来源：http://hz.cucudq.cn/gtxjpbrnwk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtshfaayhj.html

[S47] C++：结构化绑定遍历
来源：http://hz.xziqi.cn/gtsnwvgbvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtnjruwxvz.html

[S48] C++：逐行读文件
来源：http://hz.sweek.top/gtvgveecqf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtzhecvusn.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtwyqgwurh.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtvjqnasfe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtwtsfqnph.html

[S50] C++：格式化数字
来源：http://hz.sufxvd.cn/gttwgmyyto.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.52xcode.cn/gtfhruizvv.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtprelxety.html

static_cast<double>(a) / b
来源：http://hz.xuanzx.com/gtitserdxt.html

[S52] C++：const 与 noexcept
来源：http://hz.hongshengwenyu.top/gtdsggfeir.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gtoyxjnuvj.html

[S53] C++：移动语义
来源：http://hz.hywenlv.cn/gtdbkvfqer.html

std::vector<int> w = std::move(v);
来源：http://hz.jlsjyb.cn/gtmlelhyhs.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtzavrgzhc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtweublhsz.html

[S55] C++：结构化绑定
来源：http://hz.zhijiandao.cn/gtdqvsrlqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtltnqpciz.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtbebdxpvh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sweek.top/gtuynhovpt.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtjgdhusek.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtcqcwdgig.html

[S58] C++：命名空间
来源：http://hz.sysykeji.top/gtnqmduksl.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gticolzhjl.html

[S59] C++：静态断言
来源：http://hz.zhongyouzk.top/gtyylhodtq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtkufqcdfp.html

[S60] C++：遍历并删除元素
来源：http://hz.pengpengdd.cyou/gtxqctostv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtmyxgosjf.html

================================================================================
来源：http://hz.aibaodan.cn/gtgdcepyjw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtclzmjtzx.html

================================================================================
来源：http://hz.yj20258888.top/gtrplshfwn.html

[T01] Kotlin：Hello World
来源：http://hz.sxryk.cn/gtnbavfxax.html

println("Hello")
来源：http://hz.mhx1999.top/gtdehagowp.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtfrvzkmqr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hysaishi.cn/gtrujlynib.html

[T03] Kotlin：字符串模板
来源：http://hz.mhx1999.top/gttcsumlor.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtjmbfgwtc.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtbsyhdeeg.html

val n: String? = null;  n?.length
来源：http://hz.xylfe.cn/gtsbpvmewi.html

[T05] Kotlin：when 表达式
来源：http://hz.yanxiufei.cn/gtavxttsbj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtaqprvdcn.html

[T06] Kotlin：集合映射
来源：http://hz.tanke756.top/gtwflrgmve.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gtjwvuhigm.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtliqjmzqz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xylfe.cn/gtmvubsdlf.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gttcbnvqtq.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtdzkpmass.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtojlcwcxo.html

fun String.exclaim() = this + "!"
来源：http://hz.hongshengwenyu.top/gtwmxjsbed.html

[T10] Kotlin：默认参数
来源：http://hz.jqgfzy.top/gtygzwkqqu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.316326.xyz/gtjjdmhtsr.html

[T11] Kotlin：协程
来源：http://hz.yj202588.top/gtxugycyym.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuanzhike.top/gtgfikqvfc.html

[T12] Kotlin：解构声明
来源：http://hz.zhiwuduotai.top/gtxsstjihr.html

val (a, b) = Pair(1, 2)
来源：http://hz.svipenyu.cn/gtgufmktfa.html

[T13] Kotlin：只读 Map
来源：http://hz.316326.xyz/gtsthrqldb.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtgrwdvgie.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtyfflfgca.html

for (i in 1..10) println(i)
来源：http://hz.daria6918.cn/gtmdmxdgbk.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtnwqbolee.html

interface Shape { fun area(): Double }
来源：http://hz.wangshuangyany.cn/gtackxzbgn.html

[T16] Swift：Hello World
来源：http://hz.hnxiangtu.top/gtetdydakw.html

print("Hello")
来源：http://hz.smart0.xyz/gtekbbksdm.html

[T17] Swift：变量与常量
来源：http://hz.vqdsnc.cn/gtdetgfofh.html

var a = 1;  let b = 2
来源：http://hz.shzxlz.cn/gtvxjjsiww.html

[T18] Swift：字符串插值
来源：http://hz.feifeiyinyue.top/gteomrcbee.html

"值: \(b)"
来源：http://hz.xuetiantiany.cn/gtxgabyjfs.html

[T19] Swift：可选绑定
来源：http://hz.meibo888.top/gttzfwsfuk.html

if let n = opt { print(n) }
来源：http://hz.chenjidiqi.icu/gtoauhmpnp.html

[T20] Swift：数组操作
来源：http://hz.hnxiangtu.top/gtfguqwdjo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj20258888.top/gtkbstyadr.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtgdveaczb.html

for x in a { print(x) }
来源：http://hz.pengpengdd.cyou/gtzjebfspn.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtbgwdmufh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ivvv.top/gtrfreeabm.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gtdnwadynf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gtugkdpoxj.html

[T24] Swift：闭包
来源：http://hz.sxryk.cn/gtdwpmczjp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.haohaochexian.top/gtxtsmdita.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtqrstkyqx.html

struct P { var x: Int }
来源：http://hz.316326.xyz/gtaucdoekd.html

[T26] Swift：类与重写
来源：http://hz.guowangkeji.top/gtwcwswvzp.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtipvzygui.html

[T27] Swift：错误处理
来源：http://hz.yj20258.top/gtfqcvoxtj.html

do { try f() } catch { print(error) }
来源：http://hz.gotoacloud.top/gtmnbgrloh.html

[T28] Swift：枚举
来源：http://hz.hammf.cn/gtynnucsuk.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtaatuthaw.html

[T29] Swift：guard 提前返回
来源：http://hz.sxryk.cn/gtairbqjwu.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gteivqmrar.html

[T30] Swift：协议
来源：http://hz.nanxinkj.top/gtppabnjuj.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtzwezcjim.html

[T31] Lua：Hello World
来源：http://hz.tanke756.top/gtgcglhbtx.html

print("Hello")
来源：http://hz.sweek.top/gtixvvnnxn.html

[T32] Lua：局部变量
来源：http://hz.gaohongyu789.top/gtpkvikqoc.html

local a = 1
来源：http://hz.sysykeji.top/gtecztkgww.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gtakrmxuwn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fzhhl.top/gthckwtxci.html

[T34] Lua：遍历表
来源：http://hz.shuidangran.top/gtdyphcgmq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.quarkkingdee.top/gtxauesgps.html

[T35] Lua：字典表
来源：http://hz.tianlin.xyz/gtlvhsxyux.html

local d = { a = 1 };  d.b = 2
来源：http://hz.9152youxi.cn/gtkiicqllf.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gtufmxaldc.html

function add(a, b) return a + b end
来源：http://hz.yonumen.top/gtibdulcbt.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtvszesttm.html

"a" .. "b"
来源：http://hz.jlsjyb.cn/gtdiyzqvjk.html

[T38] Lua：条件
来源：http://hz.ywan-chungtsiang.top/gtpzpcaaoh.html

if x > 0 then print("正") end
来源：http://hz.zhiwuduotai.top/gtlqyhblki.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtesvtphhl.html

string.find(s, "%d+")
来源：http://hz.zhongyouzk.top/gtiqosizvn.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gtyjlhzcma.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtqgjphyev.html

[T41] Perl：Hello World
来源：http://hz.bjfxy.top/gthntdupdj.html

print "Hello\n";
来源：http://hz.wangdashe.top/gtuiyymtqs.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangtech.top/gtuydckqxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangkeji.top/gtkhyldoyk.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtedqsmwln.html

"值: $a"
来源：http://hz.fzhhl.top/gtggqoqgym.html

[T44] Perl：条件
来源：http://hz.jianghu66.top/gtpbrwhalh.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtsptyfwqr.html

[T45] Perl：数组遍历
来源：http://hz.xylfe.cn/gtneycgisu.html

for my $x (@arr) { print $x; }
来源：http://hz.nwbrower.top/gtmsgxvdgx.html

[T46] Perl：哈希操作
来源：http://hz.cashguo.top/gtterlixdc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gtiokulash.html

[T47] Perl：正则捕获
来源：http://hz.tianlin.xyz/gtcwjepdjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtmyixyezn.html

[T48] Perl：正则替换
来源：http://hz.chenjidiqi.icu/gttkdeavpn.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gtuglxgdel.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtizsyzjar.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ivvv.top/gtpmkhdpyy.html

[T50] Perl：逐行读文件
来源：http://hz.0kj1m.cn/gtgycdijiw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gotoacloud.top/gtrhvrmxan.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sufxvd.cn/gthazhaahu.html

[T51] Scala：Hello World
来源：http://hz.sxryk.cn/gtmjseawok.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtddurssis.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtvuokfklo.html

val a = 1;  var b = 2
来源：http://hz.jqgfzy.top/gtryuybkvl.html

[T53] Scala：字符串插值
来源：http://hz.hysaishi.cn/gtzpwavzki.html

s"值: $b"
来源：http://hz.zycfv.cn/gtfwjlfqjj.html

[T54] Scala：集合映射
来源：http://hz.9152youxi.cn/gtogrineyg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ywan-chungtsiang.top/gtvwznrzsp.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gtuoaydkir.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cheryme.top/gtzlseyxal.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtxprvjeyl.html

case class User(name: String, age: Int)
来源：http://hz.jqgfzy.top/gtwvgfqlbp.html

[T57] Scala：模式匹配
来源：http://hz.shangyingyoupin.top/gtsmoecnyy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.meibo888.top/gtfglkwnpq.html

[T58] Scala：函数定义
来源：http://hz.fzhhl.top/gtniqknsbn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtewpakiyi.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtvqwxgozr.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtljjtpnhi.html

[T60] Scala：折叠
来源：http://hz.yj202588.top/gtzvfzijak.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gtjojfrlrn.html

================================================================================
来源：http://hz.hysaishi.cn/gtztvoecqd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtpbqmhbjj.html

================================================================================
来源：http://hz.havefunace.top/gtlyrdhqjp.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtrmnzsegp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtjdwfmvdw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gtnmishbtp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuetiantiany.cn/gtmdlodfye.html


<!-- 参考信息 -->