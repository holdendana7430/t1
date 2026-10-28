代发 wailian999

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gtgqlxplje.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtzaevlksa.html

[S44] C++：引用传参
来源：http://hz.hammf.cn/gtavflwujw.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtibxrlpoj.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtkgqdojrs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jiagoushi.top/gtjqmdzslt.html

[S46] C++：函数模板
来源：http://hz.tian-w.cn/gtotqwbhqq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xziqi.cn/gtzqnfggot.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtauwyrrwx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtpejtawnm.html

[S48] C++：逐行读文件
来源：http://hz.vqdsnc.cn/gtdfzceugi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtyuotfice.html

while (std::getline(in, line)) { }
来源：http://hz.xinyue.icu/gtvlhdqwbu.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtwuchwexd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.birdmap.top/gtecujybtd.html

[S50] C++：格式化数字
来源：http://hz.guowangkeji.top/gtqflxsbyg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtlxzdhbdi.html

[S51] C++：显式类型转换
来源：http://hz.zhiwuduotai.top/gtiqefmyxk.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtgtqufhkf.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtsiyftlwg.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtwzioqqbg.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gtojxjltqc.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtnpsyjkhi.html

[S54] C++：异常处理
来源：http://hz.jqgfzy.top/gtdkuamkhq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtqmorkpeh.html

[S55] C++：结构化绑定
来源：http://hz.xingfuxueyuan.xyz/gtvhpvkzmq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtwolkqaun.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtjwlxjhmh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtxpknrikr.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtwefeurzr.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtwmgmmoag.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtyrftnhaw.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtsqmnciyn.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtpiyolubm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangdashe.top/gtgiotabek.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gturmdjnrr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtuyxkyxfo.html

================================================================================
来源：http://hz.yuanzhike.top/gtvttacfxn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtqyjvihgn.html

================================================================================
来源：http://hz.nanxuanxn.top/gtthmqkvgh.html

[T01] Kotlin：Hello World
来源：http://hz.ybcxt.top/gtnrxtapbz.html

println("Hello")
来源：http://hz.hnqzz.top/gtbavdkgpb.html

[T02] Kotlin：变量
来源：http://hz.yueranfly.top/gtkykaaqet.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shangyingyoupin.top/gtjgctbalh.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtzsvjxgug.html

"值: $b"
来源：http://hz.ppjwa.cn/gticvjgowi.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gtkiychjuo.html

val n: String? = null;  n?.length
来源：http://hz.c1oappe.top/gtikykkjyf.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gthicmytfh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sweek.top/gthyjghkyb.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtfuscmyux.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtrywvjwkq.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtmtgezbjx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtsnfnwzpb.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtlfwxnhfw.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtkvocvbvz.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gtijpdvnbx.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtuqevklhm.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258.top/gtkwmhszsb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhiwuduotai.top/gthkmkxbhp.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtpgrsftyd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sufxvd.cn/gttlagsrnq.html

[T12] Kotlin：解构声明
来源：http://hz.xuanzx.com/gtuviwqgos.html

val (a, b) = Pair(1, 2)
来源：http://hz.jianghu66.top/gtujidkhqd.html

[T13] Kotlin：只读 Map
来源：http://hz.dashuyun.cn/gtlbftpetd.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gtgfhaghyc.html

[T14] Kotlin：循环
来源：http://hz.fzhhl.top/gtlzrtcvwy.html

for (i in 1..10) println(i)
来源：http://hz.xuanzx.com/gtfkpznqjq.html

[T15] Kotlin：接口
来源：http://hz.vqdsnc.cn/gtxvpiklfr.html

interface Shape { fun area(): Double }
来源：http://hz.daria6918.cn/gtfwksicxv.html

[T16] Swift：Hello World
来源：http://hz.yuxming.cn/gtwpdexbew.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtnquqprpr.html

[T17] Swift：变量与常量
来源：http://hz.mhx1999.top/gtweztsrrj.html

var a = 1;  let b = 2
来源：http://hz.svipenyu.cn/gtxvecpsdl.html

[T18] Swift：字符串插值
来源：http://hz.cucudq.cn/gtvquqkvjc.html

"值: \(b)"
来源：http://hz.0kj1m.cn/gtzptaegxr.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtgwisqgjm.html

if let n = opt { print(n) }
来源：http://hz.jianghu66.top/gtnokdcqfq.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtgauoexcb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtatkhfzzz.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtzuebtknc.html

for x in a { print(x) }
来源：http://hz.tian-w.cn/gtrivtqdpo.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gtkwermhev.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinghuilouyu.cn/gtfyoehsus.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtpfotcjyb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.haohaochexian.top/gtzrjiqrsa.html

[T24] Swift：闭包
来源：http://hz.fzhhl.top/gtwtlhoufl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxuanxn.top/gtrrwfiwno.html

[T25] Swift：结构体
来源：http://hz.aibaodan.cn/gtqjqhpaei.html

struct P { var x: Int }
来源：http://hz.gzhubu.top/gtbrpxfvld.html

[T26] Swift：类与重写
来源：http://hz.hywenlv.cn/gtpmvdinhr.html

class A: Base { override func f() {} }
来源：http://hz.kuanghao11.cn/gtmqfcwtbz.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtppkbulav.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gtrygnnipq.html

[T28] Swift：枚举
来源：http://hz.wangshuangyany.cn/gtgbpexqkq.html

enum Color { case red, green }
来源：http://hz.cheryme.top/gtavmalltl.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gtyrzqukdl.html

guard let x = opt else { return }
来源：http://hz.bjfxy.top/gtajtcgdjk.html

[T30] Swift：协议
来源：http://hz.tianlin.xyz/gtqtmohvcp.html

protocol Shape { func area() -> Double }
来源：http://hz.cucudq.cn/gtziucxjek.html

[T31] Lua：Hello World
来源：http://hz.chenzaomai.com/gtwzaybanc.html

print("Hello")
来源：http://hz.yonumen.top/gtpzhjimgd.html

[T32] Lua：局部变量
来源：http://hz.daria6918.cn/gtrwheypiw.html

local a = 1
来源：http://hz.fzhhl.top/gthykjmibv.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gtmeafhora.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtygdfavyb.html

[T34] Lua：遍历表
来源：http://hz.daxiang520.top/gtpfclmmup.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenjidiqi.icu/gtvmnyhuul.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtsvyvsgmi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtobvisjrp.html

[T36] Lua：函数
来源：http://hz.feifeiyinyue.top/gtujywveid.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gttjjnyxir.html

[T37] Lua：字符串拼接
来源：http://hz.ydzc1.top/gtlgctuoda.html

"a" .. "b"
来源：http://hz.dianchejie.cn/gtjmmodncx.html

[T38] Lua：条件
来源：http://hz.yonumen.top/gtpqjjmcdc.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gtekaixdbl.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtvbtecjao.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtrlltfnkb.html

[T40] Lua：元表
来源：http://hz.jinghuilouyu.cn/gtjzcabmxn.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangkeji.top/gtpwdwpiqp.html

[T41] Perl：Hello World
来源：http://hz.xziqi.cn/gtzaeyabqn.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gtwxrydghl.html

[T42] Perl：变量类型
来源：http://hz.0kj1m.cn/gttgmntbvw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuetiantiany.cn/gtuspgtphw.html

[T43] Perl：字符串插值
来源：http://hz.kuanghao11.cn/gtzlyijtlt.html

"值: $a"
来源：http://hz.svipenyu.cn/gtzstexbaj.html

[T44] Perl：条件
来源：http://hz.shzxlz.cn/gtktpbvlqh.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gttrwpmniz.html

[T45] Perl：数组遍历
来源：http://hz.yj202588.top/gtrywdsnio.html

for my $x (@arr) { print $x; }
来源：http://hz.snrcjt.cn/gtzbhydsmr.html

[T46] Perl：哈希操作
来源：http://hz.haohaochexian.top/gtqazdqmll.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangkeji.top/gtcddbhirq.html

[T47] Perl：正则捕获
来源：http://hz.yongpay.top/gtafboyjni.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhengqikj.top/gttrztoahb.html

[T48] Perl：正则替换
来源：http://hz.hywenlv.cn/gtpzdcrtsa.html

$s =~ s/old/new/g;
来源：http://hz.bjfxy.top/gtuogsfuug.html

[T49] Perl：函数
来源：http://hz.tian-w.cn/gtfosqvvyp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.9152youxi.cn/gtyzjyrdrb.html

[T50] Perl：逐行读文件
来源：http://hz.yj20258.top/gtwnesnajf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenzaomai.com/gtuxyjxdrw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hammf.cn/gthhueyicz.html

[T51] Scala：Hello World
来源：http://hz.sysykeji.top/gtmwkrqgrl.html

println("Hello")
来源：http://hz.meibo888.top/gtczstgcgc.html

[T52] Scala：变量
来源：http://hz.ybcxt.top/gtklqrbgvf.html

val a = 1;  var b = 2
来源：http://hz.shangyingyoupin.top/gtgzelazuh.html

[T53] Scala：字符串插值
来源：http://hz.nwbrower.top/gtydsqnnei.html

s"值: $b"
来源：http://hz.yuxming.cn/gtmlufsjke.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangtech.top/gtagjycqhl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtivubgaxs.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gttjsjmgum.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtzwcpipai.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtuozfrvjs.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gttdkruwpt.html

[T57] Scala：模式匹配
来源：http://hz.tian-w.cn/gtjyskaqnu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sysykeji.top/gtgrczadsh.html

[T58] Scala：函数定义
来源：http://hz.zhijiandao.cn/gtgwuayrtv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.0kj1m.cn/gtcyaqfgwm.html

[T59] Scala：循环
来源：http://hz.sweek.top/gtnigahuho.html

for (i <- 1 to 10) println(i)
来源：http://hz.zycfv.cn/gtuetonzug.html

[T60] Scala：折叠
来源：http://hz.zhijiandao.cn/gtzwblmekm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtettplhqc.html

================================================================================
来源：http://hz.shzxlz.cn/gtdenmjtpb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hfpthk.cn/gtofepumqw.html

================================================================================
来源：http://hz.sysykeji.top/gtpmynoqlc.html

[U01] Py：创建虚拟环境
来源：http://hz.xingfuxueyuan.xyz/gtweqwztda.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtbpliwrpv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtdmkniqvh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gttnzyaxmk.html

[U03] Py：加载 .env 配置
来源：http://hz.nwbrower.top/gtqjtqnxuc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgufenzy.top/gtcxzblvbl.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtbhcpstue.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cucudq.cn/gtbgejspzu.html

[U05] Py：列表去重且保序
来源：http://hz.gzhubu.top/gtbxwzfmkf.html

list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtlwwrgqyj.html

[U06] Py：合并两个字典
来源：http://hz.jinqigufen.top/gtprakftvb.html

{**a, **b}
来源：http://hz.cqqwz.cn/gttspozwfn.html

[U07] Py：反转字典键值
来源：http://hz.shangyingyoupin.top/gtwyxcapcq.html

{v: k for k, v in d.items()}
来源：http://hz.tanke756.top/gtfwejtvki.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtexdtxowh.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtobmelhdb.html

[U09] Py：字典取最大值的键
来源：http://hz.hnqzz.top/gtobxcmsln.html

max(d, key=d.get)
来源：http://hz.hongshengwenyu.top/gtfrvkyvtu.html

[U10] Py：按值排序字典
来源：http://hz.tian-w.cn/gthfduyalb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtvpjgvsdv.html

[U11] Py：生成器表达式
来源：http://hz.jiagoushi.top/gtqztaknkb.html

(x * 2 for x in arr)
来源：http://hz.kuanghao11.cn/gtzvqhtywa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydjk.org.cn/gtvtienbmb.html

Counter(arr).most_common(3)
来源：http://hz.svipenyu.cn/gtvvfmyhgw.html

[U13] Py：固定长度队列
来源：http://hz.gzhubu.top/gtbjfgvmbo.html

deque(maxlen=10)
来源：http://hz.hnxiangtu.top/gtoufggrci.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtwcffzkod.html

defaultdict(list)
来源：http://hz.jqgufenzy.top/gtxqmlbalo.html

[U15] Py：高精度计时
来源：http://hz.cqqwz.cn/gtiqpsahlo.html

t = time.perf_counter()
来源：http://hz.nwbrower.top/gtqgmeoqpu.html

[U16] Py：命令行参数解析
来源：http://hz.chenzaomai.com/gtrmffwxrc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fengsongda.top/gtechbrlfp.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gtaqgxddop.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gtccqoxfti.html

[U18] Py：预编译正则
来源：http://hz.zhoulong.xyz/gtxtrxbvos.html

pat = re.compile(r"\d+")
来源：http://hz.zdqjudy.top/gtndfdrbfh.html

[U19] Py：正则替换带回调
来源：http://hz.sxryk.cn/gtmoocfvxg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtwswjlchq.html

[U20] Py：缓存函数结果
来源：http://hz.quarkkingdee.top/gtpvnuimcx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangkeji.top/gtogbbmvkl.html

[U21] Py：自定义上下文管理器
来源：http://hz.cucudq.cn/gtngprzymz.html

@contextlib.contextmanager
来源：http://hz.bjfxy.top/gtytmvonqx.html

[U22] Py：矩阵转置
来源：http://hz.jlsjyb.cn/gtaqekpqnm.html

list(zip(*m))
来源：http://hz.xylfe.cn/gtipaozies.html

[U23] Py：分块读取大文件
来源：http://hz.ydzc1.top/gthfuqzbmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258.top/gtiqnkfoeq.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtvhzdwmwh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.smart0.xyz/gtdwyvbjpe.html

[U25] Py：CSV 按字典读
来源：http://hz.feifeiyinyue.top/gtsvicwdvs.html

csv.DictReader(f)
来源：http://hz.guannengcc.top/gtkezsditt.html

[U26] Py：并发下载
来源：http://hz.birdmap.top/gtcttjvmku.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yongpay.top/gtfrpbyobi.html

[U27] Py：异步 HTTP
来源：http://hz.jinqigfzy.top/gtlrxthpop.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhoulong.xyz/gtddnstoqw.html

[U28] Py：类型别名
来源：http://hz.dashuyun.cn/gtuwoufwnu.html

UserId = int
来源：http://hz.yongpay.top/gtwwaoblsj.html

[U29] Py：属性校验
来源：http://hz.chenlongwang.top/gtqijnrxyx.html

@property 与 @x.setter 配合
来源：http://hz.daxiang520.top/gtphhwjtyh.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtqgscakun.html

@dataclass(slots=True)
来源：http://hz.jinghuilouyu.cn/gtcbleuccx.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtwoonyxxd.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gtbtmtbksm.html

[U32] Py：代码格式化
来源：http://hz.yueranfly.top/gtotigxpej.html

ruff format . && ruff check --fix .
来源：http://hz.nanxinkj.top/gthdqohkrz.html

[U33] Py：打包发布
来源：http://hz.gotoacloud.top/gtrgfkhdae.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.bjfxy.top/gtnueguolq.html

[U34] Py：判断编码
来源：http://hz.9152youxi.cn/gtrxardlmb.html

chardet.detect(raw)
来源：http://hz.jlsjyb.cn/gtqmqizfip.html

[U35] Py：发送邮件
来源：http://hz.shzxlz.cn/gtidqlpdvr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dianchejie.cn/gtwpkartyr.html

[U36] Py：定时任务
来源：http://hz.jiagoushi.top/gthkroyhza.html

schedule.every(10).minutes.do(job)
来源：http://hz.yangfankeji.com/gtwlpslsvx.html

[U37] Py：读写 Excel
来源：http://hz.ydjk.org.cn/gtexbyogim.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aizwys.cn/gtasojmhxe.html

[U38] Py：获取脚本所在目录
来源：http://hz.wangdashe.top/gtguskbtmx.html

Path(__file__).resolve().parent
来源：http://hz.wangdashe.top/gttsmbmyxz.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtvxbxdder.html

sys.stdout.isatty()
来源：http://hz.yj20258.top/gthgwmqyyy.html

[U40] Py：打印到标准错误
来源：http://hz.9152youxi.cn/gtaqwttjui.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtwitblhlj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.c1oappe.top/gtwibcapad.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hnxiangtu.top/gtlhjfjuyg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuanzx.com/gtfvlssnxl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinghuilouyu.cn/gtxfsqmoji.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangtech.top/gtohixcnqd.html

namespace App\Http;
来源：http://hz.guowangkeji.top/gtcwgchkkf.html

[U44] PHP：开启严格类型
来源：http://hz.zhiwuduotai.top/gtsdznjfka.html

declare(strict_types=1);
来源：http://hz.yj20258888.top/gtfflstaaa.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtilrofbjw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtdivhiqnl.html

[U46] PHP：可空类型
来源：http://hz.mhx1999.top/gtiqwaqger.html

?string $name = null
来源：http://hz.hywenlv.cn/gtfbbwwznz.html

[U47] PHP：联合类型
来源：http://hz.cashguo.top/gttopqjrhw.html

int|string $id
来源：http://hz.hnxiangtu.top/gtzxssuprq.html

[U48] PHP：纯枚举
来源：http://hz.jiagoushi.top/gtoobblbmh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258.top/gtjbvzjeby.html

[U49] PHP：只读属性
来源：http://hz.nanxinkj.top/gtmkpwbgor.html

public readonly string $name
来源：http://hz.kuanghao11.cn/gtqafxakdq.html

[U50] PHP：构造器属性提升
来源：http://hz.jinqigfzy.top/gtjbbvnilf.html

public function __construct(private int $id) {}
来源：http://hz.snrcjt.cn/gthnnwexta.html

[U51] PHP：数组解构
来源：http://hz.feifeiyinyue.top/gtuyxiqvzg.html

[$a, $b] = $arr;
来源：http://hz.cqqwz.cn/gtybavxnej.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtenmhhyst.html

$double = fn($x) => $x * 2;
来源：http://hz.sysykeji.top/gtntqtgube.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gtkorbxkfi.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhaomingkeji.xyz/gtutwymdpp.html

[U54] PHP：空安全调用
来源：http://hz.chenlongwang.top/gtkneguqok.html

$obj?->method()
来源：http://hz.feifeiyinyue.top/gtofnorpvw.html

[U55] PHP：match 表达式
来源：http://hz.wangshuangyany.cn/gtwudqjkpc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhoulong.xyz/gtheowathb.html

[U56] PHP：命名参数
来源：http://hz.gzhubu.top/gtwbygxnhy.html

f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtgjnkjlil.html

[U57] PHP：字符串插值
来源：http://hz.fzhhl.top/gtgcsiqeff.html

"值: {$a}"
来源：http://hz.ivvv.top/gtnykchdqx.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtcfijwrkr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tian-w.cn/gteqgvtyzu.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtncpwvvxg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtxvxdayln.html

[U60] PHP：JSON 编解码
来源：http://hz.chenlongwang.top/gtilqshzns.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nanxuanxn.top/gtyjfgivva.html

[U61] PHP：正则
来源：http://hz.meibo888.top/gtvvnnumxo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gteruvrugx.html

[U62] PHP：日期对象
来源：http://hz.xuetiantiany.cn/gtmovafhzv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fzhhl.top/gtbjwpoxtu.html

[U63] PHP：文件读写
来源：http://hz.bjfxy.top/gtfenskbah.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pycfn.com/gtiwgqnjgo.html

[U64] PHP：目录遍历
来源：http://hz.c1oappe.top/gtwlonbaod.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.52xcode.cn/gtjslbveri.html

[U65] PHP：会话
来源：http://hz.dashuyun.cn/gtwiqqasln.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.havefunace.top/gteyhxwuxf.html

[U66] PHP：设置 Cookie
来源：http://hz.jlsjyb.cn/gthxascvzb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cheryme.top/gtpckgkuzd.html

[U67] PHP：处理文件上传
来源：http://hz.yongpay.top/gtnngsmvrx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangshuangyany.cn/gtqobqeqoi.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangkeji.top/gtvcgieyig.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ywan-chungtsiang.top/gtfoabxbrz.html


<!-- 参考信息 -->