代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtrdcwofvn.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gtjbncvnxj.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtkeegiijw.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtclfqxvyt.html

openssl rand -hex 16
来源：http://hz.gzhubu.top/gtfbkcsvrb.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtjanjdxbj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhiwuduotai.top/gtebobnrns.html

[R69] 生成随机密码
来源：http://hz.yongpay.top/gtxpndbrnh.html

head -c 16 /dev/urandom | base64
来源：http://hz.52xcode.cn/gtzxfbsisy.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gtdprebnyj.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangtech.top/gtunumdqfj.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtipnrozez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangdashe.top/gtfylfqzxh.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtwwnpwndf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtnnpznfnm.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtpnfgxhrf.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtczjbfuoo.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtimwwnwez.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258.top/gtlpfsjvsm.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtzdnllglu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtardvsxxu.html

[R76] 使用临时文件
来源：http://hz.yongpay.top/gtiuklrzia.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtlkiivlvh.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtwjwqhqce.html

read -rp "请输入: " ans
来源：http://hz.wangdashe.top/gtorzhlvgx.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtvwgnupyv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.smart0.xyz/gtzvnebobh.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtvwehyxur.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtfpjmjeht.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigufen.top/gttlukiuvf.html

time ./run.sh
来源：http://hz.xinyue.icu/gtphhxggae.html

================================================================================
来源：http://hz.tianlin.xyz/gteoknxtgu.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gtzfzrqeto.html

================================================================================
来源：http://hz.c1oappe.top/gtxjbamymy.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtidntknyi.html

#include <stdio.h>
来源：http://hz.snrcjt.cn/gtzslhsfsp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtftybuzvf.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gtxqnmrzyz.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtgueafviv.html

[S03] C：读入整数
来源：http://hz.xingfuxueyuan.xyz/gtvbikyjla.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtnriyjbgx.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gthbhnswgo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shangyingyoupin.top/gtcttcdugp.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtglscrtyj.html

strlen(s)
来源：http://hz.jinqigufen.top/gtvzwqlqgx.html

[S06] C：字符串比较
来源：http://hz.yuanzhike.top/gtodmkxrrq.html

strcmp(a, b) == 0
来源：http://hz.xuanzx.com/gtggbeskco.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtigeroptf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtqhybbhsf.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtjqqhantb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtathjiuzm.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtvxtbwlck.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtoeruviuk.html

[S10] C：指针与解引用
来源：http://hz.tian-w.cn/gtnwujdwce.html

int *p = &a;  *p = 5;
来源：http://hz.ehwqpu.com/gtcgwdivqd.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gtokfxddyz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnxiangtu.top/gtpkmpvwgb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hywenlv.cn/gtifmqcjzp.html

fclose(f);
来源：http://hz.sufxvd.cn/gtcubhlmwb.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtrxauigqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtzfobtwpn.html

[S13] C：宏定义
来源：http://hz.havefunace.top/gtcrozghva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhengqikj.top/gtjpyaqkis.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtkseyzqem.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tian-w.cn/gtwshufbmb.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtnoxxmiif.html

(double) a / b
来源：http://hz.aibaodan.cn/gtmbtuwcqk.html

[S16] C：位操作置位
来源：http://hz.guannengcc.top/gtxoiblchj.html

x |= (1 << 3);
来源：http://hz.hnxiangtu.top/gtyxbqcdst.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gtpyfgtbgt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtrmmjszfd.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtxrjdbgda.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gthstvqdaj.html

[S19] C：快速排序
来源：http://hz.andypj.xyz/gtqhzitxib.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtkroombzk.html

[S20] C：二分查找
来源：http://hz.yuanzhike.top/gtyaqpnyls.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtcbdnjkbn.html

[S21] C：字符类别判断
来源：http://hz.smart0.xyz/gtepbtaece.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtpoqmoyvy.html

[S22] C：字符串转数字
来源：http://hz.yj20258.top/gtdhfndhmk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtuiimrxxn.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtomhpcvzm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sysykeji.top/gtfbihpfqc.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtyndjlmgk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtahpdhgpa.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtofnapzzg.html

memcpy(dst, src, n);
来源：http://hz.cheryme.top/gtmmbzlmim.html

[S26] C：内存清零
来源：http://hz.gotoacloud.top/gtpulqdbxo.html

memset(a, 0, sizeof a);
来源：http://hz.xuetiantiany.cn/gterwtapwe.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtzwyvqujp.html

const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtmavlunes.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gteegetyyq.html

static int counter = 0;
来源：http://hz.cashguo.top/gtyfcrtukc.html

[S29] C：变参函数
来源：http://hz.guannengcc.top/gtprsdjkzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aizwys.cn/gtziqqkkyq.html

[S30] C：头文件保护
来源：http://hz.snrcjt.cn/gttzelqcry.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtxghatiie.html

#define X_H
来源：http://hz.sweek.top/gtdekxbhhi.html

#endif
来源：http://hz.zhaomingkeji.xyz/gtnudepzss.html

[S31] C++：Hello World
来源：http://hz.nanxuanxn.top/gtpkddaplm.html

#include <iostream>
来源：http://hz.zycfv.cn/gtsbyicmdf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gtjhbyfkwo.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtqzyeclcp.html

std::string s = "hi";  s += "!";
来源：http://hz.smart0.xyz/gtdwqezffb.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangtech.top/gtivqlzafy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtfqqmnsrq.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtojdsmonk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtjwzbvcil.html

[S35] C++：map
来源：http://hz.yj20258888.top/gtgbaffmxu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtacgszupi.html

[S36] C++：unordered_map
来源：http://hz.feifeiyinyue.top/gtzleuauow.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtyjgjizoc.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gtwlwybtam.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtnycscdyv.html

[S38] C++：排序
来源：http://hz.yonumen.top/gtrngzwyke.html

std::sort(v.begin(), v.end());
来源：http://hz.yuxming.cn/gtwyiqiwbc.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtjybxpbdg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtkhjqaykc.html

[S40] C++：查找元素
来源：http://hz.ehwqpu.com/gtikveqoxp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtikutlbdh.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtnzcodfyo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tian-w.cn/gtrtydlelg.html

[S42] C++：继承与虚函数
来源：http://hz.pengpengdd.cyou/gtjcyhbczd.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtsjuiqxbw.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtmpntufro.html

auto p = std::make_unique<int>(5);
来源：http://hz.pengpengdd.cyou/gtsfzyduex.html

[S44] C++：引用传参
来源：http://hz.quarkkingdee.top/gtxsvepwgk.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gthfihtbcm.html

[S45] C++：lambda
来源：http://hz.yonumen.top/gtwtsvsrcr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.andypj.xyz/gtyvqymazh.html

[S46] C++：函数模板
来源：http://hz.sweek.top/gtmpppntnc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxuanxn.top/gtfpqyvojt.html

[S47] C++：结构化绑定遍历
来源：http://hz.ppjwa.cn/gtlvucesnn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gteyuagjaz.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtkezvxqeh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gthhbqmwkg.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtdvoiwrml.html

[S49] C++：写文件
来源：http://hz.ivvv.top/gtnjgzkyjh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhengqikj.top/gtrlnbtuet.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtqnaktemd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sysykeji.top/gtsicopsbj.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gticyrvbok.html

static_cast<double>(a) / b
来源：http://hz.quarkkingdee.top/gtnjcpbpwq.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258888.top/gtcsqsmfmn.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtezqfgjdm.html

[S53] C++：移动语义
来源：http://hz.ppjwa.cn/gteddadwjl.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtgsvzzjsb.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gthzsaavql.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtvoqtaiwk.html

[S55] C++：结构化绑定
来源：http://hz.316326.xyz/gtpppzlvwm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgfzy.top/gtwzztchel.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtasaprvep.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sufxvd.cn/gtcuqzjxmw.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtjbthmkda.html

constexpr int N = 10;
来源：http://hz.snrcjt.cn/gtpgmvtqhq.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtxojbhvrj.html

namespace ns { int f() { return 1; } }
来源：http://hz.fengsongda.top/gtkuawjuft.html

[S59] C++：静态断言
来源：http://hz.zhiwuduotai.top/gthknlserj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtyelqledr.html

[S60] C++：遍历并删除元素
来源：http://hz.jyoumei.cn/gtbqbcimvb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtnovggfzh.html

================================================================================
来源：http://hz.ybcxt.top/gthtuotyrp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hammf.cn/gtymxkvikt.html

================================================================================
来源：http://hz.tian-w.cn/gtajcdkshz.html

[T01] Kotlin：Hello World
来源：http://hz.yj202588.top/gttnfprdly.html

println("Hello")
来源：http://hz.yj202588.top/gtiumttuzk.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtsbhavqjp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gttacplxvy.html

[T03] Kotlin：字符串模板
来源：http://hz.cashguo.top/gtrcyrgnqh.html

"值: $b"
来源：http://hz.gotoacloud.top/gtmjpwpixf.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gthzlxhspi.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gthqhagkin.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxuanxn.top/gtemrnsaxg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gtufnkzqva.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gtsnnipbxt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtzutknrae.html

[T07] Kotlin：集合过滤
来源：http://hz.haohaochexian.top/gtkvukoiqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aibaodan.cn/gtlxxjjhrb.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtdvohuxrp.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtfkmieyew.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtaqpadewb.html

fun String.exclaim() = this + "!"
来源：http://hz.smart0.xyz/gteiyhayxy.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gtsxukcpes.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenjidiqi.icu/gtsesbwwgu.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtaqjnmanj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtzhechkqr.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtortlrieu.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gtywurmqdk.html

[T13] Kotlin：只读 Map
来源：http://hz.redwolf501.top/gttrqasvoq.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gtpsbspacp.html

[T14] Kotlin：循环
来源：http://hz.cashguo.top/gtbltczyqa.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtwdkkctzt.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtumsrpvpi.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtbytlwqar.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtjcbdfaxd.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtexgrqjwm.html

[T17] Swift：变量与常量
来源：http://hz.tanke756.top/gtnpjincsb.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gtxoijroan.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtfgghaikn.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gteeehtxyu.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtjvqfxvqh.html

if let n = opt { print(n) }
来源：http://hz.yueranfly.top/gtxpghmwsg.html

[T20] Swift：数组操作
来源：http://hz.yongpay.top/gtpmdiiyug.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhengqikj.top/gtrfcqwmmy.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtdysgqiqk.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gtipxxmlhr.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtirzqsdvl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guowangkeji.top/gtstrftvgl.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtvdguuyet.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhijiandao.cn/gtyilfsqnp.html

[T24] Swift：闭包
来源：http://hz.snrcjt.cn/gtplemozdq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gtlmylgxxs.html

[T25] Swift：结构体
来源：http://hz.feifeiyinyue.top/gtplwobyab.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gtlvpfdihk.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtifyxdznn.html

class A: Base { override func f() {} }
来源：http://hz.xingfuxueyuan.xyz/gttjkoooft.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtkcdagxqz.html

do { try f() } catch { print(error) }
来源：http://hz.dashuyun.cn/gtslpvzsil.html

[T28] Swift：枚举
来源：http://hz.ywan-chungtsiang.top/gtnauavjen.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtkhmjxqkm.html

[T29] Swift：guard 提前返回
来源：http://hz.xingfuxueyuan.xyz/gtcswqkgon.html

guard let x = opt else { return }
来源：http://hz.sysykeji.top/gtywwwyrqj.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtrbqopgdg.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gtqbsnnxmt.html

[T31] Lua：Hello World
来源：http://hz.shuidangran.top/gtxgrnuhxp.html

print("Hello")
来源：http://hz.birdmap.top/gtgyairsid.html

[T32] Lua：局部变量
来源：http://hz.guowangkeji.top/gttgoqilic.html

local a = 1
来源：http://hz.52xcode.cn/gtimaljeaq.html

[T33] Lua：表（数组）
来源：http://hz.xingfuxueyuan.xyz/gthsyrvcto.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cqqwz.cn/gtdyblnryo.html

[T34] Lua：遍历表
来源：http://hz.zhoulong.xyz/gtrhozcera.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.bjfxy.top/gtuhfhetak.html

[T35] Lua：字典表
来源：http://hz.andypj.xyz/gtyxyvskgz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangtech.top/gtlmjaxdep.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gteinbiykb.html

function add(a, b) return a + b end
来源：http://hz.wangdashe.top/gtmwfktjia.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtxpzxibvm.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtvzxriwof.html

[T38] Lua：条件
来源：http://hz.xuanzx.com/gttonxqfeq.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gtsukpunxd.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtnplckyxs.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtunlftecp.html

[T40] Lua：元表
来源：http://hz.wangshuangyany.cn/gtgqgysjqv.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtwotmigwt.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gtexqeluoq.html

print "Hello\n";
来源：http://hz.jqgfzy.top/gtlyvkvfgd.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gtakghozwp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtueyvqiuv.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtxhlhjljx.html

"值: $a"
来源：http://hz.guannengcc.top/gtvgvkmhxz.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtqydanzfu.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gtemivbdih.html

[T45] Perl：数组遍历
来源：http://hz.gogol.net.cn/gtyafamsri.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtoocmacrv.html

[T46] Perl：哈希操作
来源：http://hz.quarkkingdee.top/gttqjhoduc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gtvydsmlrn.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtlpuiffvv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gtjjocqzzx.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtuzbrhycm.html

$s =~ s/old/new/g;
来源：http://hz.tanke756.top/gtiuoxrzmt.html

[T49] Perl：函数
来源：http://hz.c1oappe.top/gtrjxhcsiy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gtxcdibcei.html

[T50] Perl：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtinekmtqn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ywan-chungtsiang.top/gtodkwvdwl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangkeji.top/gttjqhoekw.html

[T51] Scala：Hello World
来源：http://hz.hongshengwenyu.top/gtkyjnvosy.html

println("Hello")
来源：http://hz.yueranfly.top/gtfhokpscr.html

[T52] Scala：变量
来源：http://hz.birdmap.top/gtpfsibkhk.html

val a = 1;  var b = 2
来源：http://hz.jianghu66.top/gtfwkosdhz.html

[T53] Scala：字符串插值
来源：http://hz.cdnleiting.top/gtazzydeyd.html

s"值: $b"
来源：http://hz.zhongyouzk.top/gtbsvvvers.html

[T54] Scala：集合映射
来源：http://hz.cheryme.top/gtkxwocfxt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aizwys.cn/gtwsprycil.html

[T55] Scala：集合过滤
来源：http://hz.sweek.top/gtwevqwkdc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sufxvd.cn/gtrwbgyvtw.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtiwvcfyuf.html

case class User(name: String, age: Int)
来源：http://hz.zhaomingkeji.xyz/gtrqnvaikk.html

[T57] Scala：模式匹配
来源：http://hz.hfpthk.cn/gtwenekcyv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtqhlekoom.html

[T58] Scala：函数定义
来源：http://hz.shangyingyoupin.top/gtvnzlwoko.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhoulong.xyz/gtmazawcki.html

[T59] Scala：循环
来源：http://hz.quarkkingdee.top/gtntsgalpj.html

for (i <- 1 to 10) println(i)
来源：http://hz.hongshengwenyu.top/gtwbynejan.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtdcvtuydp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenjidiqi.icu/gtottrkozn.html

================================================================================
来源：http://hz.snrcjt.cn/gtlncsqixa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtvbqhzgwl.html

================================================================================
来源：http://hz.xziqi.cn/gtdeybncei.html

[U01] Py：创建虚拟环境
来源：http://hz.zhengqikj.top/gtsgwvcfay.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cucudq.cn/gtdsgikhkj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnxiangtu.top/gtmcuwvpsa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shuidangran.top/gtrzqhxxhf.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gtyezrgsqp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ppjwa.cn/gtlczgqvzr.html

[U04] Py：变量调试打印
来源：http://hz.feifeiyinyue.top/gtmgupswvu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtsynckrzu.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtamaxarlp.html

list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtrryeuahu.html

[U06] Py：合并两个字典
来源：http://hz.nanxuanxn.top/gtavjoybpa.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gthidokwca.html


<!-- 参考信息 -->