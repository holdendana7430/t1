代发 wailian999

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtwnktmcij.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gtdetbvuhw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gtwvnuwdtu.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtheienpyp.html

head -c 16 /dev/urandom | base64
来源：http://hz.gotoacloud.top/gtrnqdgqsz.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtvjttkwks.html

date +%s;  date -d @1700000000
来源：http://hz.daxiang520.top/gtkkkxtlxx.html

[R71] 日期格式化
来源：http://hz.yj202588.top/gtuysqpuob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shangyingyoupin.top/gtwhlrfnfo.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtzbrtkshr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtfdeivlrz.html

[R73] 分割大日志
来源：http://hz.yueranfly.top/gttkxbuzuh.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtenetxcpa.html

[R74] 批量重命名
来源：http://hz.chenzaomai.com/gtckfmaizt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtjquyqdoj.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangkeji.top/gtsptqsmuv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gtftxqnocb.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtqftubkzp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gttpcskbmq.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtjstbjfzl.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtqevftupu.html

[R78] 交互式菜单
来源：http://hz.jianghu66.top/gtoowpilaq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtsdhfbhou.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtvejqvoep.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtvialaazc.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gttuxhhlmb.html

time ./run.sh
来源：http://hz.daxiang520.top/gtejgvwmaq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtewdxrjug.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gtxzsnxjhr.html

================================================================================
来源：http://hz.jiagoushi.top/gthlvjbdjf.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtuyigjweg.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtdojsqsio.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtmooaqndf.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtiajzailh.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtivsauzuv.html

[S03] C：读入整数
来源：http://hz.cqqwz.cn/gtudrvgwky.html

int x; scanf("%d", &x);
来源：http://hz.316326.xyz/gtflbbprjy.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtydtmmnjy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gteeftihgm.html

[S05] C：字符串长度
来源：http://hz.xinyue.icu/gtehrekhyb.html

strlen(s)
来源：http://hz.316326.xyz/gtyyrzakov.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtcvyhucjk.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtucevusih.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtyopxtmtk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.iojbl.cn/gtjdzeyatz.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gttgrswxuw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnqzz.top/gthfscuzqt.html

[S09] C：结构体定义与初始化
来源：http://hz.hysaishi.cn/gtfuseykrw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gttvcltzok.html

[S10] C：指针与解引用
来源：http://hz.jinyuanbaomall.cn/gtxesizlst.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtzrwusjhn.html

[S11] C：逐行读文件
来源：http://hz.haohaochexian.top/gtuavwrfxm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtyrxcmish.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhaomingkeji.xyz/gtbuuzeslk.html

fclose(f);
来源：http://hz.jqgfzy.top/gtinhriskt.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtzqovysvz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtwyvgwqvk.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtqqjsmhnz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtbavyuwin.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtvtxbrldi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yonumen.top/gttedhyfbi.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtszxgljpz.html

(double) a / b
来源：http://hz.0kj1m.cn/gtjnndnjnq.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gtobbexsrm.html

x |= (1 << 3);
来源：http://hz.feifeiyinyue.top/gtmrvxgwuw.html

[S17] C：安全拼接字符串
来源：http://hz.zdqjudy.top/gtafozkxfk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtidjkdfgb.html

[S18] C：命令行参数
来源：http://hz.yvedp.cn/gtjrwaezaw.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtdonyrulz.html

[S19] C：快速排序
来源：http://hz.xuetiantiany.cn/gthbwudjmj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtnpwbysir.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtmjkpykar.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gttpafscrx.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtqlzuhvrn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtshgvocyf.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gtylnnxhtj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.snrcjt.cn/gtvgknbcuf.html

[S23] C：随机数
来源：http://hz.xuetiantiany.cn/gtmauolyrt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gtsirvgeza.html

[S24] C：获取本地时间
来源：http://hz.xuanzx.com/gtvtqiuxcx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhiwuduotai.top/gtblvsofzl.html

[S25] C：内存拷贝
来源：http://hz.daxiang520.top/gtdzoqfldo.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtrydtgajg.html

[S26] C：内存清零
来源：http://hz.guannengcc.top/gtqovdvxcl.html

memset(a, 0, sizeof a);
来源：http://hz.fzhhl.top/gttojouxkw.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtannryjsr.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtjyozfubc.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtmhufoogd.html

static int counter = 0;
来源：http://hz.smart0.xyz/gtgozudgjs.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtnwkegumi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gtyzkgtdei.html

[S30] C：头文件保护
来源：http://hz.yongpay.top/gtukaqfnql.html

#ifndef X_H
来源：http://hz.birdmap.top/gtlbzudobc.html

#define X_H
来源：http://hz.xinyue.icu/gtecsbuolj.html

#endif
来源：http://hz.shangyingyoupin.top/gtrleynhey.html

[S31] C++：Hello World
来源：http://hz.yuxming.cn/gtwuxefytm.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtjlbawvnb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtrhxrddef.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gttbzzhqkd.html

std::string s = "hi";  s += "!";
来源：http://hz.gzhubu.top/gtwdsyoprq.html

[S33] C++：vector 增删
来源：http://hz.hysaishi.cn/gtpvlphwxh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtzproqcup.html

[S34] C++：遍历 vector
来源：http://hz.nwbrower.top/gtrsurapxi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gthqrsidfw.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtiyjjvezo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtknnltcla.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtegysjdnf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtnzfifajd.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtgjmdvhri.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sysykeji.top/gtjxdutzpz.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtsatafilr.html

std::sort(v.begin(), v.end());
来源：http://hz.ydzc1.top/gtmpmtbcyb.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gtjuwkerih.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtwjpkhqgb.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtnbmjxtii.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtxgjchkxf.html

[S41] C++：类与构造函数
来源：http://hz.feifeiyinyue.top/gtkmcmkhde.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtihfbiehv.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtksqxudsd.html

class B : public Base { public: void f() override {} };
来源：http://hz.xingfuxueyuan.xyz/gtnncskyzj.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtdbxoguqd.html

auto p = std::make_unique<int>(5);
来源：http://hz.tanke756.top/gtrclictdh.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtpzlosgwi.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gttbesyleq.html

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gtjviyjuok.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.9152youxi.cn/gttizorytw.html

[S46] C++：函数模板
来源：http://hz.jlsjyb.cn/gtanavstyn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtakayloqh.html

[S47] C++：结构化绑定遍历
来源：http://hz.ehwqpu.com/gtmtdqvxpz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtohblhyok.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtkxgqwdoo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gtpeobdmyg.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtwlorpbju.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtsohnwzmm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtkqzldwuv.html

[S50] C++：格式化数字
来源：http://hz.gaohongyu789.top/gtbgjslyll.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtkyocgswf.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtjuehawhn.html

static_cast<double>(a) / b
来源：http://hz.c1oappe.top/gtryfbqkby.html

[S52] C++：const 与 noexcept
来源：http://hz.pengpengdd.cyou/gthrrnlbzt.html

int size() const noexcept { return n_; }
来源：http://hz.jianghu66.top/gtfjaopeas.html

[S53] C++：移动语义
来源：http://hz.gotoacloud.top/gtomlpkvsv.html

std::vector<int> w = std::move(v);
来源：http://hz.zhixingplan.top/gthytjkbed.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtgcfsfuba.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jyoumei.cn/gtnfmyhjtl.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gtgigdefxe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtcmirseph.html

[S56] C++：optional
来源：http://hz.wangdashe.top/gtmepsdxiv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtthkepcgy.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtfyrcqhhi.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtyosjmfjl.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtwkddbrka.html

namespace ns { int f() { return 1; } }
来源：http://hz.9152youxi.cn/gtziwgtxlk.html

[S59] C++：静态断言
来源：http://hz.sweek.top/gtoymqfgpt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtmzjgjeyy.html

[S60] C++：遍历并删除元素
来源：http://hz.zhengqikj.top/gtkzhqwrab.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.52xcode.cn/gtofdrtcnl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsqiiaxef.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtggwpqwck.html

================================================================================
来源：http://hz.xinyue.icu/gtxmekamel.html

[T01] Kotlin：Hello World
来源：http://hz.feifeiyinyue.top/gtksohasrd.html

println("Hello")
来源：http://hz.ydzc1.top/gtaxtgswql.html

[T02] Kotlin：变量
来源：http://hz.52xcode.cn/gtvapsdqdc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gtovmwxaqb.html

[T03] Kotlin：字符串模板
来源：http://hz.jinqigufen.top/gtcadxebbj.html

"值: $b"
来源：http://hz.wangshuangyany.cn/gtwdeynskk.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtzkkwregs.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gtkvmbwqbh.html

[T05] Kotlin：when 表达式
来源：http://hz.jianghu66.top/gthisbzwmw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jyoumei.cn/gtyaybzxje.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtcuusraxx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtnxsuqbbo.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtdprqkcds.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gotoacloud.top/gtrodcmmwv.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gtfyjgrhfy.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtzyshovgs.html

[T09] Kotlin：扩展函数
来源：http://hz.zycfv.cn/gtegnbwarx.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtgjybolka.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtprmadygb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtvudsorud.html

[T11] Kotlin：协程
来源：http://hz.vqdsnc.cn/gtppvwllrr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtydymeyjr.html

[T12] Kotlin：解构声明
来源：http://hz.fzhhl.top/gtrearkfyi.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtqqynvglb.html

[T13] Kotlin：只读 Map
来源：http://hz.pengpengdd.cyou/gtmugxfiff.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gtbsjwlzua.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtigrfkquu.html

for (i in 1..10) println(i)
来源：http://hz.quarkkingdee.top/gtzobgytvg.html

[T15] Kotlin：接口
来源：http://hz.ivvv.top/gtbjrvvhnv.html

interface Shape { fun area(): Double }
来源：http://hz.haohaochexian.top/gtstnyodgq.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtahncqypd.html

print("Hello")
来源：http://hz.fzhhl.top/gtinmnxazd.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtlfoqzchu.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtdfclucik.html

[T18] Swift：字符串插值
来源：http://hz.shuidangran.top/gtyzfwcgvl.html

"值: \(b)"
来源：http://hz.hammf.cn/gtlaflhpse.html

[T19] Swift：可选绑定
来源：http://hz.guowangkeji.top/gthrfsixiu.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gttmcwwmow.html

[T20] Swift：数组操作
来源：http://hz.fzhhl.top/gtjuxsnzhn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yanxiufei.cn/gtlzgsyouk.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtzibyfhws.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gtgcgpadaa.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtbcoqqewm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jianghu66.top/gtffslpbdc.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtictxhuit.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj202588.top/gtqdjwzvhw.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gtlkegbyub.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtrmgxzvpx.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangkeji.top/gtebstghnr.html

struct P { var x: Int }
来源：http://hz.quarkkingdee.top/gtjnmsieva.html

[T26] Swift：类与重写
来源：http://hz.zhijiandao.cn/gtcvlabbjm.html

class A: Base { override func f() {} }
来源：http://hz.0kj1m.cn/gtvcdvqffo.html

[T27] Swift：错误处理
来源：http://hz.aizwys.cn/gtwszookvd.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gtgwuvuyda.html

[T28] Swift：枚举
来源：http://hz.dianchejie.cn/gtetogffhp.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtzpbierhu.html

[T29] Swift：guard 提前返回
来源：http://hz.yongpay.top/gtcjujyxab.html

guard let x = opt else { return }
来源：http://hz.nanxuanxn.top/gtydnlirnr.html

[T30] Swift：协议
来源：http://hz.52xcode.cn/gtutpaodgh.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtxvybnliw.html

[T31] Lua：Hello World
来源：http://hz.jiagoushi.top/gtdtrnmsom.html

print("Hello")
来源：http://hz.cashguo.top/gtlmpviqqc.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtlpbswyxk.html

local a = 1
来源：http://hz.birdmap.top/gtmzqzkcrq.html

[T33] Lua：表（数组）
来源：http://hz.316326.xyz/gterdrhfnr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhaomingkeji.xyz/gtaamsdzdd.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gtonikwkcg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.fzhhl.top/gtrcycgftm.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gtytxveauf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jianghu66.top/gtncnildld.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtqpcxwvay.html

function add(a, b) return a + b end
来源：http://hz.chenzaomai.com/gtylvwddyb.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtohninfke.html

"a" .. "b"
来源：http://hz.52xcode.cn/gtshanxoul.html

[T38] Lua：条件
来源：http://hz.xuetiantiany.cn/gtxpivamhv.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtnzjqxadq.html

[T39] Lua：模式匹配
来源：http://hz.tianlin.xyz/gtqjbqdqxe.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtbxhnnuex.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtsjniyujr.html

setmetatable({}, { __index = base })
来源：http://hz.sufxvd.cn/gtuyorsjkx.html

[T41] Perl：Hello World
来源：http://hz.sysykeji.top/gtyroniigb.html

print "Hello\n";
来源：http://hz.tanke756.top/gtzzmeadff.html

[T42] Perl：变量类型
来源：http://hz.smart0.xyz/gtdgordhzr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtstvokwky.html

[T43] Perl：字符串插值
来源：http://hz.birdmap.top/gtpviwpkip.html

"值: $a"
来源：http://hz.hnqzz.top/gtqxnorqhs.html

[T44] Perl：条件
来源：http://hz.hnqzz.top/gtrqodpimn.html

if ($a > 0) { print "正"; }
来源：http://hz.yuxming.cn/gteqfxzqis.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gthjbdhhmr.html

for my $x (@arr) { print $x; }
来源：http://hz.hysaishi.cn/gtgboxgpzf.html

[T46] Perl：哈希操作
来源：http://hz.hywenlv.cn/gtlecrgycd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.316326.xyz/gtyusvhbkg.html

[T47] Perl：正则捕获
来源：http://hz.aibaodan.cn/gthvdrifga.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yonumen.top/gttgvvogrz.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gtxmfdntyt.html

$s =~ s/old/new/g;
来源：http://hz.guannengcc.top/gtbcgfurpn.html

[T49] Perl：函数
来源：http://hz.gzhubu.top/gthdtufplw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cdnleiting.top/gtxjeqrirc.html

[T50] Perl：逐行读文件
来源：http://hz.svipenyu.cn/gtudwaaqvs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtkjcvcfsm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.316326.xyz/gtkwkakpvl.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtfjowhycx.html

println("Hello")
来源：http://hz.0kj1m.cn/gtznjhlbhy.html

[T52] Scala：变量
来源：http://hz.chenzaomai.com/gtqvlpcgnf.html

val a = 1;  var b = 2
来源：http://hz.aizwys.cn/gtfdlchqvj.html

[T53] Scala：字符串插值
来源：http://hz.birdmap.top/gtcrgvpijy.html

s"值: $b"
来源：http://hz.jinqigfzy.top/gtitsfytrt.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtdndfeemb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gtlrzvpsqm.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtnnwemybs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuetiantiany.cn/gtlqywkybl.html

[T56] Scala：样例类
来源：http://hz.andypj.xyz/gtmhcxfxzv.html

case class User(name: String, age: Int)
来源：http://hz.sxryk.cn/gtyupgrapy.html

[T57] Scala：模式匹配
来源：http://hz.fengsongda.top/gtkhbvzzxm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtcknuognh.html

[T58] Scala：函数定义
来源：http://hz.jinqigufen.top/gtohkvvcrj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cucudq.cn/gtxmxchdro.html

[T59] Scala：循环
来源：http://hz.316326.xyz/gtlqvmydti.html

for (i <- 1 to 10) println(i)
来源：http://hz.nanxuanxn.top/gtdkuxwxbo.html

[T60] Scala：折叠
来源：http://hz.svipenyu.cn/gtynucgbsf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhoulong.xyz/gttgjwgbsy.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnvuyhufy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gtsofnbbjs.html

================================================================================
来源：http://hz.zhongyouzk.top/gtzupztnvk.html

[U01] Py：创建虚拟环境
来源：http://hz.andypj.xyz/gtdoefjvmg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.9152youxi.cn/gtlvavrlbk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yongpay.top/gtcctuaowj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ybcxt.top/gtojlngbls.html

[U03] Py：加载 .env 配置
来源：http://hz.gzhubu.top/gtryrlojmk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daxiang520.top/gtvxcstijj.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gtavnvsaxh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cashguo.top/gtwfngkena.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangkeji.top/gtmhvzjexl.html

list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtywlzpifr.html

[U06] Py：合并两个字典
来源：http://hz.shangyingyoupin.top/gtrdmqjbmv.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtnftumcee.html

[U07] Py：反转字典键值
来源：http://hz.zhixingplan.top/gtldnhkkte.html

{v: k for k, v in d.items()}
来源：http://hz.ybcxt.top/gtptmddeha.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtlnxdtdff.html

[y for x in nested for y in x]
来源：http://hz.zhoulong.xyz/gtqsnmhpgb.html


<!-- 参考信息 -->