代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtlejixdsg.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtjuxbadhm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gaohongyu789.top/gttimhdnly.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtsbikkzwp.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtvvltcvxf.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtmxfenjry.html

du -ah . | sort -rh | head -10
来源：http://hz.xuanzx.com/gtttjgymdl.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gttjxepixc.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtcklutdkv.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gtafldokvk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangdashe.top/gtdplklgub.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtcmqdkrqo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnqzz.top/gtwsjvlgfo.html

[R66] 定时任务
来源：http://hz.haohaochexian.top/gtstihxkon.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtggcrwuwx.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtqorcfzbx.html

openssl rand -hex 16
来源：http://hz.xylfe.cn/gtvpvrjnub.html

[R68] 计算文件校验值
来源：http://hz.chenlongwang.top/gtcbdpohka.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gotoacloud.top/gtlsciydnr.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtptrmqkds.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gtitvzrasv.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gthrnvcfhc.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtfbydepkt.html

[R71] 日期格式化
来源：http://hz.zhijiandao.cn/gtcxqnyirk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigufen.top/gtrzoosnuj.html

[R72] 等待端口就绪
来源：http://hz.wangshuangyany.cn/gttpcnkfyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhixingplan.top/gtscvxsfba.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtlflscbpd.html

split -l 1000 big.log part_
来源：http://hz.zhiwuduotai.top/gtesjzyokd.html

[R74] 批量重命名
来源：http://hz.tianlin.xyz/gtjwzephxi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aizwys.cn/gtocpzuesl.html

[R75] 导出环境变量
来源：http://hz.zhaomingkeji.xyz/gtxxwkzpou.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gtmmcbevgd.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtxecxtbgn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtlxswazxr.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtcjojmmha.html

read -rp "请输入: " ans
来源：http://hz.daria6918.cn/gtdicujqxf.html

[R78] 交互式菜单
来源：http://hz.jqgfzy.top/gtcohzgiax.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gtprikuiqe.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtetegakkz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xingfuxueyuan.xyz/gtmxoodxaw.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtqtaiyiej.html

time ./run.sh
来源：http://hz.yueranfly.top/gtxropxxlu.html

================================================================================
来源：http://hz.0kj1m.cn/gtjsgvcaxv.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtvtgrxarf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdunwxwyp.html

[S01] C：Hello World
来源：http://hz.pengpengdd.cyou/gtfnbhpgzn.html

#include <stdio.h>
来源：http://hz.shangyingyoupin.top/gtcnrsfqmu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtoytuxlmc.html

[S02] C：变量与格式化输出
来源：http://hz.iojbl.cn/gtlrcgchnl.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxuanxn.top/gtkbeltnmv.html

[S03] C：读入整数
来源：http://hz.redwolf501.top/gtwjdcwjae.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtmbyyjrne.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtnxgfugaq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gttcwjtlpz.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtxqfxbods.html

strlen(s)
来源：http://hz.ydzc1.top/gtwdmrvwcx.html

[S06] C：字符串比较
来源：http://hz.nanxinkj.top/gtqnvjuydi.html

strcmp(a, b) == 0
来源：http://hz.chenlongwang.top/gtgavqyqgq.html

[S07] C：数组遍历求和
来源：http://hz.bjfxy.top/gtpvgtxenb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtijmrsvnm.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gtzrfeyotz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtnlmwprgn.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtnrwpglcr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.haohaochexian.top/gthqeoxlry.html

[S10] C：指针与解引用
来源：http://hz.zhengqikj.top/gtqepbugbu.html

int *p = &a;  *p = 5;
来源：http://hz.aibaodan.cn/gtzlcrlwzh.html

[S11] C：逐行读文件
来源：http://hz.guowangkeji.top/gtwhftbkwn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gturvabmgy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.snrcjt.cn/gtcvimeupi.html

fclose(f);
来源：http://hz.hywenlv.cn/gtjauurdev.html

[S12] C：写文件
来源：http://hz.pengpengdd.cyou/gtrsjzwyhn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtepqrplch.html

[S13] C：宏定义
来源：http://hz.svipenyu.cn/gtoaqkucys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hysaishi.cn/gtugloqjnp.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtmjpjapde.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtlkxvfiqk.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gttrzpnhkx.html

(double) a / b
来源：http://hz.daxiang520.top/gtjpaigkif.html

[S16] C：位操作置位
来源：http://hz.shzxlz.cn/gtxckkacbz.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtnvzlzdsa.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gtnhxxnmsy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yvedp.cn/gtwpgquhbz.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gtinhhhggw.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtmulbsbwm.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtgwwaxyor.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtwoktzxsn.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtlodygtjc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtlejegqjo.html

[S21] C：字符类别判断
来源：http://hz.haohaochexian.top/gtjpxtrzxs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.redwolf501.top/gtnizekekv.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtdxzowmur.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yongpay.top/gtdbgcpsig.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtzfvwglsq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jyoumei.cn/gtniourfgz.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gtjvavamnb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtuxntybqj.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtlbsdigua.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtsltlglwz.html

[S26] C：内存清零
来源：http://hz.aizwys.cn/gtfygixvoi.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangtech.top/gtnlvsvzsn.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtdsxmxvux.html

const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtrcniotvo.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtilmbtmii.html

static int counter = 0;
来源：http://hz.ehwqpu.com/gtftwkurva.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gtubdomwxw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtcwdrhpfk.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtmxodpvyl.html

#ifndef X_H
来源：http://hz.yj20258888.top/gtuobacfoa.html

#define X_H
来源：http://hz.shuidangran.top/gthacnblrk.html

#endif
来源：http://hz.daria6918.cn/gtvvvifgeu.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gthfeneaiq.html

#include <iostream>
来源：http://hz.aibaodan.cn/gtitskohwa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtcyrugoue.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtgiyvplul.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtwxulazac.html

[S33] C++：vector 增删
来源：http://hz.52xcode.cn/gtxhwfpzds.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtdnabtfhw.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtubdtkypd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jyoumei.cn/gtvklkroml.html

[S35] C++：map
来源：http://hz.yongpay.top/gtzfaorjvu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtcskczoab.html

[S36] C++：unordered_map
来源：http://hz.shzxlz.cn/gtnxnajqvg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtecymrunb.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtpkcoqrxb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtahzctnvd.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtcmemnjcg.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtfyrcrdqi.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtadimqnce.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtqwxnersl.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtvebroepw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gthxnhytai.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtqgnwgnbd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtkzhicvuq.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtxfwsrwoe.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxinkj.top/gtvbnewfcm.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtobqsjdpq.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangdashe.top/gtyklevlus.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gttntblypd.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtpojorbpg.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtwhmgocsc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.redwolf501.top/gtcriamlhy.html

[S46] C++：函数模板
来源：http://hz.hywenlv.cn/gtzgynusdq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtptjogjog.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtiyetfsdi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtvuwdqipn.html

[S48] C++：逐行读文件
来源：http://hz.cqqwz.cn/gtncmlgllf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gttjyeamem.html

while (std::getline(in, line)) { }
来源：http://hz.cqqwz.cn/gturumqtat.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtmmrjhdxr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gtrpulcium.html

[S50] C++：格式化数字
来源：http://hz.yanxiufei.cn/gtavrgtusy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtndmpufvs.html

[S51] C++：显式类型转换
来源：http://hz.svipenyu.cn/gtowemsaho.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtsvqdotnu.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gtcizicgpb.html

int size() const noexcept { return n_; }
来源：http://hz.jianghu66.top/gtbubfyvtq.html

[S53] C++：移动语义
来源：http://hz.zhongyouzk.top/gtwcljjrpr.html

std::vector<int> w = std::move(v);
来源：http://hz.zhengqikj.top/gtncgfzmff.html

[S54] C++：异常处理
来源：http://hz.tian-w.cn/gtzrhbfxrh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtlslnpijj.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtloptafav.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtbipvutin.html

[S56] C++：optional
来源：http://hz.feifeiyinyue.top/gtvgyhaocq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtasftsfty.html

[S57] C++：编译期常量
来源：http://hz.hysaishi.cn/gtaruondkp.html

constexpr int N = 10;
来源：http://hz.yj20258888.top/gtdpfvdwlv.html

[S58] C++：命名空间
来源：http://hz.dashuyun.cn/gtvsmztzcb.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenzaomai.com/gtobcdencl.html

[S59] C++：静态断言
来源：http://hz.tanke756.top/gtkvwraibh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jiagoushi.top/gtsaoxsmdk.html

[S60] C++：遍历并删除元素
来源：http://hz.chenlongwang.top/gtugkprqoq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtryoptpbp.html

================================================================================
来源：http://hz.xinyue.icu/gtapxjlxtr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtuukjnhsm.html

================================================================================
来源：http://hz.fzhhl.top/gtbinzriab.html

[T01] Kotlin：Hello World
来源：http://hz.zdqjudy.top/gtechpzmkk.html

println("Hello")
来源：http://hz.ppjwa.cn/gtdsgxvgxp.html

[T02] Kotlin：变量
来源：http://hz.andypj.xyz/gtjwkrqgck.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aizwys.cn/gtwizepjry.html

[T03] Kotlin：字符串模板
来源：http://hz.yvedp.cn/gtvlafctxj.html

"值: $b"
来源：http://hz.cashguo.top/gtrtnygrww.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtxsehohpr.html

val n: String? = null;  n?.length
来源：http://hz.svipenyu.cn/gtwtyxmnny.html

[T05] Kotlin：when 表达式
来源：http://hz.haohaochexian.top/gtbuqzlxss.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.c1oappe.top/gtrhyibpqh.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtxcchhrul.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtgkkhtkvd.html

[T07] Kotlin：集合过滤
来源：http://hz.xziqi.cn/gtttghowwm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtqwkwfije.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gtvoqkeene.html

data class User(val name: String, val age: Int)
来源：http://hz.gaohongyu789.top/gtbxayfoih.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtulcomjnr.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtehsczufw.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtxrijgkcj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtlvzpyjzz.html

[T11] Kotlin：协程
来源：http://hz.cdnleiting.top/gtrgedtbxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.bjfxy.top/gtaqqxxuas.html

[T12] Kotlin：解构声明
来源：http://hz.yueranfly.top/gtaqjtdejm.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhijiandao.cn/gtpmhqekzu.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgfzy.top/gtbuokzxvb.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtorgeqzrb.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtrdcztawi.html

for (i in 1..10) println(i)
来源：http://hz.hywenlv.cn/gtmvhzetnm.html

[T15] Kotlin：接口
来源：http://hz.wangshuangyany.cn/gtmgscgpvm.html

interface Shape { fun area(): Double }
来源：http://hz.hnxiangtu.top/gtsepgurry.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtkqilskay.html

print("Hello")
来源：http://hz.jiagoushi.top/gtxlnpnhdy.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtiztmmxyw.html

var a = 1;  let b = 2
来源：http://hz.yuxming.cn/gttwirexcc.html

[T18] Swift：字符串插值
来源：http://hz.yvedp.cn/gtqbdjodhz.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtidjhpfne.html

[T19] Swift：可选绑定
来源：http://hz.jlsjyb.cn/gtpenofthe.html

if let n = opt { print(n) }
来源：http://hz.jqgfzy.top/gtlcqltwyt.html

[T20] Swift：数组操作
来源：http://hz.zhongyouzk.top/gtlxuyypbg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daria6918.cn/gtraywrwpj.html

[T21] Swift：遍历
来源：http://hz.jianghu66.top/gtysgydosc.html

for x in a { print(x) }
来源：http://hz.aizwys.cn/gteicnxntd.html

[T22] Swift：字典
来源：http://hz.redwolf501.top/gtpkfklduo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jianghu66.top/gtvlqphmnd.html

[T23] Swift：函数
来源：http://hz.zhengqikj.top/gtfntxnrcr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtlkpusdwa.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gtyaxymqfi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xuanzx.com/gtmeleszue.html

[T25] Swift：结构体
来源：http://hz.nanxuanxn.top/gtcvpndaiq.html

struct P { var x: Int }
来源：http://hz.cqqwz.cn/gtdmnzipsa.html

[T26] Swift：类与重写
来源：http://hz.smart0.xyz/gtwgglpzve.html

class A: Base { override func f() {} }
来源：http://hz.yonumen.top/gtneiasgxc.html

[T27] Swift：错误处理
来源：http://hz.zhijiandao.cn/gtvbjnvhgv.html

do { try f() } catch { print(error) }
来源：http://hz.jqgufenzy.top/gtrzghoxrg.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtdusftngx.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtzpyrvikx.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gttwtehtyv.html

guard let x = opt else { return }
来源：http://hz.hammf.cn/gtlivfhrmz.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtegacxjey.html

protocol Shape { func area() -> Double }
来源：http://hz.tanke756.top/gtuarbkoke.html

[T31] Lua：Hello World
来源：http://hz.xuanzx.com/gtmacfixbk.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtzhrhjwqx.html

[T32] Lua：局部变量
来源：http://hz.mhx1999.top/gtglwosisy.html

local a = 1
来源：http://hz.bjfxy.top/gtplgzlzho.html

[T33] Lua：表（数组）
来源：http://hz.gaohongyu789.top/gtzznydruc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yvedp.cn/gtjhyssoqy.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtcahzkzon.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtlvuuexue.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtsrgilwol.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigufen.top/gtjvrofwsu.html

[T36] Lua：函数
来源：http://hz.9152youxi.cn/gtqjopvyku.html

function add(a, b) return a + b end
来源：http://hz.tian-w.cn/gtxksnpjrq.html

[T37] Lua：字符串拼接
来源：http://hz.cashguo.top/gtiwnkoknk.html

"a" .. "b"
来源：http://hz.bjfxy.top/gtsjfxzhkw.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gtgaapmkgn.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtbrtkvaon.html

[T39] Lua：模式匹配
来源：http://hz.hysaishi.cn/gtfppxwpew.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtqsscusul.html

[T40] Lua：元表
来源：http://hz.hywenlv.cn/gteiiikwln.html

setmetatable({}, { __index = base })
来源：http://hz.wangshuangyany.cn/gttksecxyk.html

[T41] Perl：Hello World
来源：http://hz.yj20258888.top/gtlqnjajwd.html

print "Hello\n";
来源：http://hz.zhiwuduotai.top/gtfyjahkcf.html

[T42] Perl：变量类型
来源：http://hz.ppjwa.cn/gtqmunbjny.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sufxvd.cn/gtqmbhanwo.html

[T43] Perl：字符串插值
来源：http://hz.jinqigfzy.top/gteoymaalm.html

"值: $a"
来源：http://hz.sxryk.cn/gtahhzuqaj.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gttclanzhm.html

if ($a > 0) { print "正"; }
来源：http://hz.52xcode.cn/gtfmuankaz.html

[T45] Perl：数组遍历
来源：http://hz.birdmap.top/gtlwppoqqq.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtccknzibn.html

[T46] Perl：哈希操作
来源：http://hz.jinyuanbaomall.cn/gtbicatgzx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gtlyatzgmy.html

[T47] Perl：正则捕获
来源：http://hz.yj20258.top/gtbgyfgnag.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhiwuduotai.top/gtxsaajaht.html

[T48] Perl：正则替换
来源：http://hz.chenjidiqi.icu/gtzattdgvl.html

$s =~ s/old/new/g;
来源：http://hz.shuidangran.top/gthsfuvdjg.html

[T49] Perl：函数
来源：http://hz.haohaochexian.top/gtccdzgncp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sysykeji.top/gtpawijhfg.html

[T50] Perl：逐行读文件
来源：http://hz.shzxlz.cn/gtwpmmxtti.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtkrugtgws.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pengpengdd.cyou/gtjzzbyggd.html

[T51] Scala：Hello World
来源：http://hz.redwolf501.top/gtjsooxvjx.html

println("Hello")
来源：http://hz.ydzc1.top/gtejuslyun.html

[T52] Scala：变量
来源：http://hz.ywan-chungtsiang.top/gtbkglnrnj.html

val a = 1;  var b = 2
来源：http://hz.jqgfzy.top/gthexxvifj.html

[T53] Scala：字符串插值
来源：http://hz.yuanzhike.top/gtlrpqdshz.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gterzhtcfz.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gtgtmxrjkz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnxiangtu.top/gtjvfuslxz.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gtmyazfssg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtvewkjwcy.html

[T56] Scala：样例类
来源：http://hz.cheryme.top/gtyygsaqpi.html

case class User(name: String, age: Int)
来源：http://hz.zhiwuduotai.top/gtxuxsfotv.html

[T57] Scala：模式匹配
来源：http://hz.chenzaomai.com/gteikzvord.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtvtnimggm.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtulmgdiar.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cqqwz.cn/gtvycoazne.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtkxrhoktw.html

for (i <- 1 to 10) println(i)
来源：http://hz.daria6918.cn/gtcyogmquu.html

[T60] Scala：折叠
来源：http://hz.xylfe.cn/gtytnfhhbt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangshuangyany.cn/gtcwkjepno.html

================================================================================
来源：http://hz.haohaochexian.top/gtocrbbiho.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sysykeji.top/gtmuxzaxss.html

================================================================================
来源：http://hz.cheryme.top/gtiqefhtfw.html


<!-- 参考信息 -->