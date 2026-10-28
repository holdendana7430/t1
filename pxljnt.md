代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.jinqigfzy.top/gtmowiwvgr.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtmsicbriw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhijiandao.cn/gtacrctuwd.html

[R65] 查看端口占用
来源：http://hz.meibo888.top/gtmtqifeba.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hfpthk.cn/gtwhsurdzh.html

[R66] 定时任务
来源：http://hz.ehwqpu.com/gtlufjojge.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtnpexnnvr.html

[R67] 生成随机十六进制串
来源：http://hz.svipenyu.cn/gtbdoejoja.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gtafyobrfk.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtojuzlkcz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtfvtwallm.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gthsaiyezn.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtoyqhdzpd.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtexihkomg.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gtlgrlkjec.html

[R71] 日期格式化
来源：http://hz.yangfankeji.com/gteigmprkj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gttvtfujhu.html

[R72] 等待端口就绪
来源：http://hz.sysykeji.top/gtvucgrhvq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtrgjvpuzp.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gtreivhyfi.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtrgpabzxx.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtqsusxxjt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtujglhdua.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gtygvdurpg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tian-w.cn/gtuezkcxqv.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtocfurcaq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtoyeobtfd.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtlceqcsvb.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtnpyqxsiq.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtyzkhcqub.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtkdbanmgp.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtplwmguiv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtjmnuucyt.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gtskfpkjcy.html

time ./run.sh
来源：http://hz.tian-w.cn/gtaasgiunc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjzcmrxqu.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gttsbcekbm.html

================================================================================
来源：http://hz.guannengcc.top/gtgysimxhz.html

[S01] C：Hello World
来源：http://hz.fengsongda.top/gtaliitrvd.html

#include <stdio.h>
来源：http://hz.jqgufenzy.top/gtspkxpdxh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtueflslhf.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gtwblqwfbt.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtfeftpwit.html

[S03] C：读入整数
来源：http://hz.jyoumei.cn/gtwfeamumi.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtmompnoeg.html

[S04] C：字符串复制
来源：http://hz.xingfuxueyuan.xyz/gtjxapdyej.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gtkpafppva.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtcukvksyl.html

strlen(s)
来源：http://hz.andypj.xyz/gtugidyazl.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtnlvsmukl.html

strcmp(a, b) == 0
来源：http://hz.dashuyun.cn/gtpnjcieil.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gthfydsmnr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gtvsimduph.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtlldqnklg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nwbrower.top/gtyvpqwiuq.html

[S09] C：结构体定义与初始化
来源：http://hz.fzhhl.top/gtqqmndkin.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtguiiyvgh.html

[S10] C：指针与解引用
来源：http://hz.sysykeji.top/gtjxzlhqaz.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gthviwqkpy.html

[S11] C：逐行读文件
来源：http://hz.wangdashe.top/gtibephldw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shuidangran.top/gtmjrnsjrk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtvdldszlt.html

fclose(f);
来源：http://hz.yuanzhike.top/gtjbmkpwki.html

[S12] C：写文件
来源：http://hz.shangyingyoupin.top/gtatprrsqf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gtavdwjldf.html

[S13] C：宏定义
来源：http://hz.gogol.net.cn/gttvncijcc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sweek.top/gtnxsxsfcg.html

[S14] C：枚举
来源：http://hz.daria6918.cn/gtpnheicid.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtxiqpxwfc.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtuptroxuu.html

(double) a / b
来源：http://hz.yueranfly.top/gtwsgufxnc.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtpbzabrth.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtofhxrqjx.html

[S17] C：安全拼接字符串
来源：http://hz.tianlin.xyz/gtxgszuzrp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtvpewfxpc.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtaavcuofx.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtokulbbqk.html

[S19] C：快速排序
来源：http://hz.dashuyun.cn/gtuvknsflc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtnzxpgxut.html

[S20] C：二分查找
来源：http://hz.gogol.net.cn/gtgzjtmfxy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtbtxqlkno.html

[S21] C：字符类别判断
来源：http://hz.zhaomingkeji.xyz/gtzhdejdgr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.andypj.xyz/gtiudqlswu.html

[S22] C：字符串转数字
来源：http://hz.yonumen.top/gtehuooufj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gzhubu.top/gtxigbvcow.html

[S23] C：随机数
来源：http://hz.tian-w.cn/gtriizwlfn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtbesrmwoy.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtrowbzxsp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cucudq.cn/gtdfldzvvs.html

[S25] C：内存拷贝
来源：http://hz.yvedp.cn/gtvcxninth.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtwcuooowr.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gthtkfnfjd.html

memset(a, 0, sizeof a);
来源：http://hz.cheryme.top/gteeiqlhot.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtxjldrkjd.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtsqungezv.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtodpgvcds.html

static int counter = 0;
来源：http://hz.fengsongda.top/gtizdlryls.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtbzbefcds.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yueranfly.top/gtzwiqnodp.html

[S30] C：头文件保护
来源：http://hz.zhaomingkeji.xyz/gtolakvhbh.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gthidfiwad.html

#define X_H
来源：http://hz.aizwys.cn/gtyimzxpjh.html

#endif
来源：http://hz.9152youxi.cn/gtbdhjikpk.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtcqqkpwid.html

#include <iostream>
来源：http://hz.tian-w.cn/gtpkdaqazu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtrocyfksv.html

[S32] C++：字符串
来源：http://hz.ivvv.top/gttdcfebhv.html

std::string s = "hi";  s += "!";
来源：http://hz.cashguo.top/gtulizsfgc.html

[S33] C++：vector 增删
来源：http://hz.chenjidiqi.icu/gtvrzvyrky.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sweek.top/gtdbkffgcv.html

[S34] C++：遍历 vector
来源：http://hz.yj202588.top/gtkxviuika.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtgzodfiqs.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtjaxfvdpr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtbxmvfjtx.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtvzeihuri.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtefeecijt.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtmsmzeekd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtnnvfjqwu.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtvkjfcabt.html

std::sort(v.begin(), v.end());
来源：http://hz.shangyingyoupin.top/gtrzvndghy.html

[S39] C++：自定义比较器排序
来源：http://hz.feifeiyinyue.top/gtklwyauvw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ywan-chungtsiang.top/gtibsmlygk.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtansbykba.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sufxvd.cn/gtkqzbhcup.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtnvrnlcey.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gtzhtayfum.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtbeswuasf.html

class B : public Base { public: void f() override {} };
来源：http://hz.yongpay.top/gtpqkldbru.html

[S43] C++：智能指针
来源：http://hz.jianghu66.top/gtneigmznw.html

auto p = std::make_unique<int>(5);
来源：http://hz.pengpengdd.cyou/gtayshctgq.html

[S44] C++：引用传参
来源：http://hz.jlsjyb.cn/gtjqhujyyz.html

void inc(int &x) { ++x; }
来源：http://hz.guowangkeji.top/gtrbiszcdc.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtcpcyoqxg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgfzy.top/gtqrlazdqx.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtqgwhjoio.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.smart0.xyz/gtkmengome.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtdgzubxms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cheryme.top/gtpdooezvp.html

[S48] C++：逐行读文件
来源：http://hz.ivvv.top/gtmyrxfepj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtsceknoea.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtyegikznj.html

[S49] C++：写文件
来源：http://hz.feifeiyinyue.top/gtlpvtmggl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gogol.net.cn/gtuntusgdf.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtpejynjah.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtdzbpdzyy.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtxlguddcz.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtatciomyl.html

[S52] C++：const 与 noexcept
来源：http://hz.yanxiufei.cn/gtfmtiivqx.html

int size() const noexcept { return n_; }
来源：http://hz.ivvv.top/gtrswclfte.html

[S53] C++：移动语义
来源：http://hz.wangdashe.top/gtfoslpqtu.html

std::vector<int> w = std::move(v);
来源：http://hz.c1oappe.top/gtsefliaqf.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtdjghaubk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gtnoelyupq.html

[S55] C++：结构化绑定
来源：http://hz.dashuyun.cn/gtnroxonda.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj202588.top/gtbvvhuxwl.html

[S56] C++：optional
来源：http://hz.yuanzhike.top/gtyhkcjnvi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtibqunjxu.html

[S57] C++：编译期常量
来源：http://hz.chenjidiqi.icu/gtvwqnidhs.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtajqilbou.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtlovuuhfe.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtvdsrpyee.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtilevhgho.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.9152youxi.cn/gtljcfnmjr.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gthdlrnsdz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.meibo888.top/gtnvizcibt.html

================================================================================
来源：http://hz.hammf.cn/gtzsgvpwfs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtqocndety.html

================================================================================
来源：http://hz.zycfv.cn/gtqhofshle.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gtajmdnsfn.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtjtatfamg.html

[T02] Kotlin：变量
来源：http://hz.meibo888.top/gtmqtiatnc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtcgmgnqrb.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtykcwitbe.html

"值: $b"
来源：http://hz.yuxming.cn/gtajhpcihy.html

[T04] Kotlin：空安全
来源：http://hz.havefunace.top/gtesfdkgxe.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtuzfkusmu.html

[T05] Kotlin：when 表达式
来源：http://hz.chenjidiqi.icu/gtvaiblsvw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtiyqrgjqq.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtqtvnetuu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtqosvlxxs.html

[T07] Kotlin：集合过滤
来源：http://hz.yj202588.top/gtxyufuhcn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtdjxkbbuw.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gturvmeazh.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtsvykscir.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtiocwszbm.html

fun String.exclaim() = this + "!"
来源：http://hz.zhongyouzk.top/gtbzhufltp.html

[T10] Kotlin：默认参数
来源：http://hz.havefunace.top/gtgjjxfaag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sweek.top/gtkyjagufk.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtcygvxnqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtlsgesgbh.html

[T12] Kotlin：解构声明
来源：http://hz.chenlongwang.top/gtowrqqtyj.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhengqikj.top/gtigaufdru.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtcoccifao.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangkeji.top/gtemaklovv.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtezilshyt.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtnsorcyef.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtrnshlftc.html

interface Shape { fun area(): Double }
来源：http://hz.aibaodan.cn/gtmuclfdzv.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gttrbmixgv.html

print("Hello")
来源：http://hz.aibaodan.cn/gtjbvdwdat.html

[T17] Swift：变量与常量
来源：http://hz.zycfv.cn/gttngchtay.html

var a = 1;  let b = 2
来源：http://hz.316326.xyz/gthkklpaia.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gthlvehycb.html

"值: \(b)"
来源：http://hz.316326.xyz/gtuepfoqgc.html

[T19] Swift：可选绑定
来源：http://hz.nanxuanxn.top/gtlnqnqdqp.html

if let n = opt { print(n) }
来源：http://hz.guannengcc.top/gtaywgqvdj.html

[T20] Swift：数组操作
来源：http://hz.52xcode.cn/gtotjiicrp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.52xcode.cn/gtplckfuwb.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtvimpgdfg.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtjgcsijtn.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtmkkahput.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhiwuduotai.top/gtcnbypffp.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gtgikfujuo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtsdxslfft.html

[T24] Swift：闭包
来源：http://hz.zhijiandao.cn/gtoapcyylo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258888.top/gtxwztsanv.html

[T25] Swift：结构体
来源：http://hz.yuxming.cn/gtpjnksddc.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gthxztukyu.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtphvibuob.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtyqzsshid.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gtphrvyudt.html

do { try f() } catch { print(error) }
来源：http://hz.yj202588.top/gtvpuldnrq.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gteynhzhdx.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtrodshqrk.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gthmazoftx.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtmddnwinc.html

[T30] Swift：协议
来源：http://hz.zhiwuduotai.top/gtomgoubzu.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gtamseevhj.html

[T31] Lua：Hello World
来源：http://hz.shangyingyoupin.top/gtqialznbq.html

print("Hello")
来源：http://hz.jinyuanbaomall.cn/gtbvobteqk.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtzgeqrmpq.html

local a = 1
来源：http://hz.yuanzhike.top/gtduxfesiw.html

[T33] Lua：表（数组）
来源：http://hz.svipenyu.cn/gttiwmvmno.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.mhx1999.top/gtfquwmewt.html

[T34] Lua：遍历表
来源：http://hz.yangfankeji.com/gtfdqdgdgi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhixingplan.top/gtxiniirhr.html

[T35] Lua：字典表
来源：http://hz.9152youxi.cn/gtwsiqlrzp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhoulong.xyz/gtmvhvckjv.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gtnnaxpntl.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtizlszviw.html

[T37] Lua：字符串拼接
来源：http://hz.gaohongyu789.top/gtubpxrtif.html

"a" .. "b"
来源：http://hz.xziqi.cn/gtrwqhlvpc.html

[T38] Lua：条件
来源：http://hz.ybcxt.top/gtsfhdnxap.html

if x > 0 then print("正") end
来源：http://hz.feifeiyinyue.top/gtwgyihoin.html

[T39] Lua：模式匹配
来源：http://hz.kuanghao11.cn/gtdpmjisty.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtbjfjwpyy.html

[T40] Lua：元表
来源：http://hz.xziqi.cn/gtnrkjijdv.html

setmetatable({}, { __index = base })
来源：http://hz.316326.xyz/gtfnjpyffu.html

[T41] Perl：Hello World
来源：http://hz.xuetiantiany.cn/gtxjsmkkxe.html

print "Hello\n";
来源：http://hz.quarkkingdee.top/gtsaxpiywq.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtzmetttse.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuetiantiany.cn/gtywviwvkg.html

[T43] Perl：字符串插值
来源：http://hz.hnqzz.top/gtzyenbluc.html

"值: $a"
来源：http://hz.svipenyu.cn/gtsjnhrbqd.html

[T44] Perl：条件
来源：http://hz.cheryme.top/gtlfaltbea.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gtxxvqnlrh.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtewrtbftc.html

for my $x (@arr) { print $x; }
来源：http://hz.feifeiyinyue.top/gtxajpyekp.html

[T46] Perl：哈希操作
来源：http://hz.gotoacloud.top/gtokswftlt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.0kj1m.cn/gtkpxvzaem.html

[T47] Perl：正则捕获
来源：http://hz.zhijiandao.cn/gtqmccrnka.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtmtgqasfe.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gtsrbwldyu.html

$s =~ s/old/new/g;
来源：http://hz.xziqi.cn/gtqbzcncbw.html

[T49] Perl：函数
来源：http://hz.shuidangran.top/gtjsyrfomf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ivvv.top/gtszksxkhq.html

[T50] Perl：逐行读文件
来源：http://hz.fzhhl.top/gtuomvqugo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shangyingyoupin.top/gtxwoxqisb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtikvszukn.html

[T51] Scala：Hello World
来源：http://hz.yanxiufei.cn/gtcmuocqbh.html

println("Hello")
来源：http://hz.guannengcc.top/gttqgpgoip.html

[T52] Scala：变量
来源：http://hz.yueranfly.top/gtggucqhce.html

val a = 1;  var b = 2
来源：http://hz.ywan-chungtsiang.top/gthcthykxk.html

[T53] Scala：字符串插值
来源：http://hz.jqgufenzy.top/gtzynoqanh.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtjzpdllyz.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtwayhxpfk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258888.top/gtpyndjhwk.html

[T55] Scala：集合过滤
来源：http://hz.sxryk.cn/gtwuacsndn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.kuanghao11.cn/gtowipkpdi.html

[T56] Scala：样例类
来源：http://hz.hongshengwenyu.top/gtbvxudwak.html

case class User(name: String, age: Int)
来源：http://hz.wangshuangyany.cn/gtlnhualmg.html

[T57] Scala：模式匹配
来源：http://hz.mhx1999.top/gtfhhfcnqw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhengqikj.top/gtsvwqulnt.html

[T58] Scala：函数定义
来源：http://hz.tanke756.top/gtsyhijqgs.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jiagoushi.top/gtdxelowvq.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtzvzrtesz.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtkchqainw.html

[T60] Scala：折叠
来源：http://hz.0kj1m.cn/gtszbjfqmm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.316326.xyz/gtnpavrewa.html

================================================================================
来源：http://hz.dianchejie.cn/gtehjxjkps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gtaduvtimc.html

================================================================================
来源：http://hz.xziqi.cn/gthpzpejfa.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtwysvxdhx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nanxinkj.top/gthhgnvlbs.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtbwwucwpz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yonumen.top/gtzzuelawr.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gtxhykwmrw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.haohaochexian.top/gtbomuixud.html

[U04] Py：变量调试打印
来源：http://hz.redwolf501.top/gtlxjgzxmd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hywenlv.cn/gtdqauohed.html


<!-- 参考信息 -->