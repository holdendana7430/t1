代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.ybcxt.top/gtvagaruiz.html

[S49] C++：写文件
来源：http://hz.cqqwz.cn/gttxuvcbxb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtshqcfset.html

[S50] C++：格式化数字
来源：http://hz.daxiang520.top/gtahklicxe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenjidiqi.icu/gtaaozlgjk.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtsfxcohqi.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtzcugomwf.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gtezhmiekf.html

int size() const noexcept { return n_; }
来源：http://hz.aizwys.cn/gtdhnuhwvq.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtqsdsvqpz.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtrvkjivcb.html

[S54] C++：异常处理
来源：http://hz.shuidangran.top/gtcxavsbjs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtsfzickfw.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtxrewmqzl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinghuilouyu.cn/gtaymbfliq.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtudfeseyp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gtmklriyjb.html

[S57] C++：编译期常量
来源：http://hz.ybcxt.top/gtccrsmwqp.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtlnxbqain.html

[S58] C++：命名空间
来源：http://hz.ybcxt.top/gtbkspdjvu.html

namespace ns { int f() { return 1; } }
来源：http://hz.xinyue.icu/gtamynjcsy.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtyimezbpf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtuhilplkv.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtzksbltje.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtzswjxhzz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsldovbaz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258888.top/gtgcatkxko.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdqztmzty.html

[T01] Kotlin：Hello World
来源：http://hz.jianghu66.top/gtmgswxamj.html

println("Hello")
来源：http://hz.gotoacloud.top/gtyhfveidw.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtxbtklpiw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.andypj.xyz/gtlkcxduvu.html

[T03] Kotlin：字符串模板
来源：http://hz.yvedp.cn/gtxzaugfru.html

"值: $b"
来源：http://hz.xuanzx.com/gtazdcfxmz.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtssdqewht.html

val n: String? = null;  n?.length
来源：http://hz.gzhubu.top/gtcnyhvxff.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gtcxnzxnjg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gaohongyu789.top/gttcjyzqli.html

[T06] Kotlin：集合映射
来源：http://hz.yongpay.top/gtmkgjnfay.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.haohaochexian.top/gtbhzzfibf.html

[T07] Kotlin：集合过滤
来源：http://hz.svipenyu.cn/gttcxmemio.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtouquqmix.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtmllzhhpg.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258888.top/gtpisaybie.html

[T09] Kotlin：扩展函数
来源：http://hz.gaohongyu789.top/gthgufxdep.html

fun String.exclaim() = this + "!"
来源：http://hz.quarkkingdee.top/gttswxuisw.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangkeji.top/gtdhyorkwh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhengqikj.top/gtxwqebibd.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtyfsliwmy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.mhx1999.top/gtvhxvoiwe.html

[T12] Kotlin：解构声明
来源：http://hz.cqqwz.cn/gtxrndoyil.html

val (a, b) = Pair(1, 2)
来源：http://hz.ivvv.top/gtyvqjknjo.html

[T13] Kotlin：只读 Map
来源：http://hz.jinyuanbaomall.cn/gtlrajppxs.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtasndhjrf.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gtyfnomyth.html

for (i in 1..10) println(i)
来源：http://hz.aibaodan.cn/gtkgjvewbw.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtbywkwnzo.html

interface Shape { fun area(): Double }
来源：http://hz.hnxiangtu.top/gtkwgnnayb.html

[T16] Swift：Hello World
来源：http://hz.feifeiyinyue.top/gtsxmzrigt.html

print("Hello")
来源：http://hz.jinyuanbaomall.cn/gtwoiblwer.html

[T17] Swift：变量与常量
来源：http://hz.kuanghao11.cn/gtyzeamcyy.html

var a = 1;  let b = 2
来源：http://hz.shanyushiyangtech.top/gtrjdhdwtn.html

[T18] Swift：字符串插值
来源：http://hz.guannengcc.top/gtxxizxfvp.html

"值: \(b)"
来源：http://hz.zycfv.cn/gtlivkvffz.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtnkdktuel.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gtunwxkgrg.html

[T20] Swift：数组操作
来源：http://hz.haohaochexian.top/gthxywzgdl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtgiltccet.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gtgeoalurc.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtroximshf.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtflxvkcmh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtewyzyvsk.html

[T23] Swift：函数
来源：http://hz.jyoumei.cn/gtmavpgfua.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.mhx1999.top/gtpjzljbkk.html

[T24] Swift：闭包
来源：http://hz.gaohongyu789.top/gtkjjgtgpd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.quarkkingdee.top/gtjsitbhua.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtdmupdato.html

struct P { var x: Int }
来源：http://hz.52xcode.cn/gtmnpugcmh.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtduaocjyc.html

class A: Base { override func f() {} }
来源：http://hz.ivvv.top/gtcbbgyfby.html

[T27] Swift：错误处理
来源：http://hz.aizwys.cn/gtiofzcqod.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gthjsgskbh.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtmpgarrlh.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtxypoljbw.html

[T29] Swift：guard 提前返回
来源：http://hz.guowangkeji.top/gtsmdyeimu.html

guard let x = opt else { return }
来源：http://hz.cqqwz.cn/gtqrcpzsun.html

[T30] Swift：协议
来源：http://hz.havefunace.top/gtoeedlfrh.html

protocol Shape { func area() -> Double }
来源：http://hz.havefunace.top/gtexkrmwfs.html

[T31] Lua：Hello World
来源：http://hz.pengpengdd.cyou/gtirciekur.html

print("Hello")
来源：http://hz.jianghu66.top/gtgslidsqr.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtlvvfswsy.html

local a = 1
来源：http://hz.cheryme.top/gtzljajrxs.html

[T33] Lua：表（数组）
来源：http://hz.cheryme.top/gtqrobnbgl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgfzy.top/gtyvmfermy.html

[T34] Lua：遍历表
来源：http://hz.xylfe.cn/gtspjtdzre.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtmcpisidr.html

[T35] Lua：字典表
来源：http://hz.cucudq.cn/gtcukapyzc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtutfcfiro.html

[T36] Lua：函数
来源：http://hz.cucudq.cn/gtpvokyasa.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtommunhcw.html

[T37] Lua：字符串拼接
来源：http://hz.ehwqpu.com/gtfhrpsrzn.html

"a" .. "b"
来源：http://hz.zhaomingkeji.xyz/gtgfexuukr.html

[T38] Lua：条件
来源：http://hz.9152youxi.cn/gthwxuhmua.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtamrdyzmg.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtsalnzqcv.html

string.find(s, "%d+")
来源：http://hz.hnqzz.top/gtzxwewvjf.html

[T40] Lua：元表
来源：http://hz.chenzaomai.com/gtsrfisbiv.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtipjrtonm.html

[T41] Perl：Hello World
来源：http://hz.yanxiufei.cn/gtwbzvyzon.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtfdinqxes.html

[T42] Perl：变量类型
来源：http://hz.jinqigfzy.top/gtqnzmiwkh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aizwys.cn/gtyukkjfyc.html

[T43] Perl：字符串插值
来源：http://hz.mhx1999.top/gtkxgyhsyf.html

"值: $a"
来源：http://hz.yj202588.top/gtcxzjpsnx.html

[T44] Perl：条件
来源：http://hz.tanke756.top/gtsioefxgm.html

if ($a > 0) { print "正"; }
来源：http://hz.zycfv.cn/gtfhmwvqrt.html

[T45] Perl：数组遍历
来源：http://hz.dianchejie.cn/gtwapobxww.html

for my $x (@arr) { print $x; }
来源：http://hz.316326.xyz/gtirmdmxqh.html

[T46] Perl：哈希操作
来源：http://hz.ydjk.org.cn/gtweinjwtj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgufenzy.top/gtsorjnwei.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtficjwazc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtftwblyyw.html

[T48] Perl：正则替换
来源：http://hz.jqgufenzy.top/gtpesqfwhe.html

$s =~ s/old/new/g;
来源：http://hz.ppjwa.cn/gtlfsqligj.html

[T49] Perl：函数
来源：http://hz.sweek.top/gtjlvbrcmu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtrtjnqdkd.html

[T50] Perl：逐行读文件
来源：http://hz.zhiwuduotai.top/gtegyphtqn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cucudq.cn/gtjjxvdrln.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ywan-chungtsiang.top/gtivdcfhcb.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtzbydnejz.html

println("Hello")
来源：http://hz.jianghu66.top/gttcdxdwre.html

[T52] Scala：变量
来源：http://hz.hnqzz.top/gttjuuohst.html

val a = 1;  var b = 2
来源：http://hz.yonumen.top/gtcqzsewfk.html

[T53] Scala：字符串插值
来源：http://hz.hammf.cn/gtyurbytbz.html

s"值: $b"
来源：http://hz.zhengqikj.top/gtrsjzwsst.html

[T54] Scala：集合映射
来源：http://hz.shangyingyoupin.top/gteyhqnoff.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cheryme.top/gtfffcyarj.html

[T55] Scala：集合过滤
来源：http://hz.c1oappe.top/gtyhwczxdb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gotoacloud.top/gtjbslbgbm.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtizcfryrj.html

case class User(name: String, age: Int)
来源：http://hz.wangdashe.top/gtqeaqfkje.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtbghvpcwc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cheryme.top/gtvwcthzyc.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtyulbvvmm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinqigufen.top/gtbfwkdffr.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtuqcpvnih.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtyfhycpku.html

[T60] Scala：折叠
来源：http://hz.jiagoushi.top/gtopuvnied.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cucudq.cn/gtgfggwxij.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvgdbhxth.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuanzx.com/gtfpbzypem.html

================================================================================
来源：http://hz.yongpay.top/gtkkcupahl.html

[U01] Py：创建虚拟环境
来源：http://hz.hysaishi.cn/gtogvryhbr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yonumen.top/gtiixxfiwk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cqqwz.cn/gtfhghpxml.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtqvmadajs.html

[U03] Py：加载 .env 配置
来源：http://hz.ehwqpu.com/gteqilxwmr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhijiandao.cn/gtctzlafjl.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gthcyyawdl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jyoumei.cn/gtqthwyviy.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtvvdqxnol.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtswdcksqg.html

[U06] Py：合并两个字典
来源：http://hz.zhengqikj.top/gtxxbkufff.html

{**a, **b}
来源：http://hz.xingfuxueyuan.xyz/gtzqbtsxar.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtooagycpo.html

{v: k for k, v in d.items()}
来源：http://hz.jinyuanbaomall.cn/gtdqxinhja.html

[U08] Py：展平二维列表
来源：http://hz.snrcjt.cn/gtjfbvhjkh.html

[y for x in nested for y in x]
来源：http://hz.zdqjudy.top/gtewvkcmdj.html

[U09] Py：字典取最大值的键
来源：http://hz.guannengcc.top/gtuchnaqml.html

max(d, key=d.get)
来源：http://hz.9152youxi.cn/gttmmwwegu.html

[U10] Py：按值排序字典
来源：http://hz.vqdsnc.cn/gttoxurrqd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.pycfn.com/gtavzxkghv.html

[U11] Py：生成器表达式
来源：http://hz.cashguo.top/gtspwnmglv.html

(x * 2 for x in arr)
来源：http://hz.cqqwz.cn/gttruutkkt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sysykeji.top/gtvaueozbm.html

Counter(arr).most_common(3)
来源：http://hz.chenzaomai.com/gtbzfredyo.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtblshdozy.html

deque(maxlen=10)
来源：http://hz.vqdsnc.cn/gtabwlooso.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtohthsxwy.html

defaultdict(list)
来源：http://hz.mhx1999.top/gtosglchnm.html

[U15] Py：高精度计时
来源：http://hz.meibo888.top/gtwwgiczgd.html

t = time.perf_counter()
来源：http://hz.ywan-chungtsiang.top/gtoybhlhql.html

[U16] Py：命令行参数解析
来源：http://hz.iojbl.cn/gtzzyuvzfw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtjykpmxex.html

[U17] Py：初始化日志
来源：http://hz.haohaochexian.top/gtplmnrpkp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tianlin.xyz/gtpuzjffqg.html

[U18] Py：预编译正则
来源：http://hz.zhixingplan.top/gtcxjmgmgn.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtypqvbcso.html

[U19] Py：正则替换带回调
来源：http://hz.pycfn.com/gtlatpxivj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tian-w.cn/gtkcuthjws.html

[U20] Py：缓存函数结果
来源：http://hz.yj20258888.top/gtigurtjvt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtggwxittv.html

[U21] Py：自定义上下文管理器
来源：http://hz.yvedp.cn/gtqwatnttg.html

@contextlib.contextmanager
来源：http://hz.jqgfzy.top/gtfxpehlzb.html

[U22] Py：矩阵转置
来源：http://hz.yueranfly.top/gtuykbboft.html

list(zip(*m))
来源：http://hz.cqqwz.cn/gtfwotqziq.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtxxwfjwzq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.nwbrower.top/gtoeelxkox.html

[U24] Py：路径操作
来源：http://hz.cashguo.top/gtrzwyuogd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.9152youxi.cn/gtbxjcgxrw.html

[U25] Py：CSV 按字典读
来源：http://hz.dashuyun.cn/gtzcxtjwfh.html

csv.DictReader(f)
来源：http://hz.xylfe.cn/gtogxqufav.html

[U26] Py：并发下载
来源：http://hz.zhongyouzk.top/gtvohrpnrl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtcakyzydu.html

[U27] Py：异步 HTTP
来源：http://hz.jinghuilouyu.cn/gtqlvmaati.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pengpengdd.cyou/gtejfuewpg.html

[U28] Py：类型别名
来源：http://hz.jinqigufen.top/gtxccyozzm.html

UserId = int
来源：http://hz.nanxinkj.top/gtdaslulrw.html

[U29] Py：属性校验
来源：http://hz.tianlin.xyz/gtgkmddcir.html

@property 与 @x.setter 配合
来源：http://hz.tian-w.cn/gtyrndwyhj.html

[U30] Py：数据类
来源：http://hz.shangyingyoupin.top/gtushwedrn.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtdeonakws.html

[U31] Py：单测
来源：http://hz.zhaomingkeji.xyz/gtelcsanvq.html

python -m pytest -q
来源：http://hz.0kj1m.cn/gtmskkoatc.html

[U32] Py：代码格式化
来源：http://hz.shzxlz.cn/gtbubdbijz.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtfjyxpdht.html

[U33] Py：打包发布
来源：http://hz.jyoumei.cn/gtzebqiwjm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gtoluwwrwr.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtjuysjmra.html

chardet.detect(raw)
来源：http://hz.shuidangran.top/gtdrdrikro.html

[U35] Py：发送邮件
来源：http://hz.feifeiyinyue.top/gtswpsucxw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.mhx1999.top/gtbxaoqdfh.html

[U36] Py：定时任务
来源：http://hz.andypj.xyz/gtnuozgblu.html

schedule.every(10).minutes.do(job)
来源：http://hz.aibaodan.cn/gtpyheudwu.html

[U37] Py：读写 Excel
来源：http://hz.hywenlv.cn/gtwwxeqaez.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.quarkkingdee.top/gtebmrgvhs.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtghuqxckb.html

Path(__file__).resolve().parent
来源：http://hz.hnqzz.top/gtxygjwybj.html

[U39] Py：判断是否在交互环境
来源：http://hz.9152youxi.cn/gtvdkytgqe.html

sys.stdout.isatty()
来源：http://hz.cashguo.top/gtrwxouqfe.html

[U40] Py：打印到标准错误
来源：http://hz.snrcjt.cn/gtdzjruvwv.html

print("err", file=sys.stderr)
来源：http://hz.jlsjyb.cn/gtmtgtbvjx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.havefunace.top/gtpnbxwqdq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hammf.cn/gtdmjjfyim.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangshuangyany.cn/gtpglavcup.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nanxuanxn.top/gtnyukwlox.html

[U43] PHP：声明命名空间
来源：http://hz.yj20258888.top/gtcicfswro.html

namespace App\Http;
来源：http://hz.mhx1999.top/gtvpwzqaga.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtsrmxnotm.html

declare(strict_types=1);
来源：http://hz.aizwys.cn/gtltnfdqxg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sufxvd.cn/gtrkcekpxm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtrlzhhvzg.html

[U46] PHP：可空类型
来源：http://hz.redwolf501.top/gtidbsgxlz.html

?string $name = null
来源：http://hz.gogol.net.cn/gtaovfgnqi.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtzpxintxz.html

int|string $id
来源：http://hz.redwolf501.top/gtsjprnqtc.html

[U48] PHP：纯枚举
来源：http://hz.hongshengwenyu.top/gtdvavetip.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aizwys.cn/gtzjxoubvq.html

[U49] PHP：只读属性
来源：http://hz.zhiwuduotai.top/gttzjytubt.html

public readonly string $name
来源：http://hz.smart0.xyz/gtgoouqjdw.html

[U50] PHP：构造器属性提升
来源：http://hz.ywan-chungtsiang.top/gtmqfmcgdd.html

public function __construct(private int $id) {}
来源：http://hz.ehwqpu.com/gtuehvdeyr.html

[U51] PHP：数组解构
来源：http://hz.wangshuangyany.cn/gtexduzypd.html

[$a, $b] = $arr;
来源：http://hz.shuidangran.top/gtslsglduf.html

[U52] PHP：箭头函数
来源：http://hz.yj20258888.top/gtfhtykohn.html

$double = fn($x) => $x * 2;
来源：http://hz.ydjk.org.cn/gtsbeolpyb.html

[U53] PHP：空合并运算符
来源：http://hz.52xcode.cn/gtpqkwqgob.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhongyouzk.top/gtwfjiwudy.html

[U54] PHP：空安全调用
来源：http://hz.hywenlv.cn/gtsjtrncol.html

$obj?->method()
来源：http://hz.yvedp.cn/gtkzvszdcv.html

[U55] PHP：match 表达式
来源：http://hz.ybcxt.top/gttiuaqbbv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinyuanbaomall.cn/gtslbqnmcb.html

[U56] PHP：命名参数
来源：http://hz.guannengcc.top/gtqdyfdrrc.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gteaqichxd.html

[U57] PHP：字符串插值
来源：http://hz.hnqzz.top/gtdmzbgfho.html

"值: {$a}"
来源：http://hz.yj20258.top/gtgsagnjew.html

[U58] PHP：数组三件套
来源：http://hz.hnxiangtu.top/gttmtwplhv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.bjfxy.top/gtrsxrafps.html

[U59] PHP：自定义排序
来源：http://hz.sweek.top/gtisztzuti.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtstnhqnor.html

[U60] PHP：JSON 编解码
来源：http://hz.zycfv.cn/gtymbrmepr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sysykeji.top/gtdwyfdyuw.html

[U61] PHP：正则
来源：http://hz.nwbrower.top/gteysuuvlh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtmlbfnhbg.html

[U62] PHP：日期对象
来源：http://hz.gotoacloud.top/gtyvambcwi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinyuanbaomall.cn/gtwfugiucs.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gtotplinei.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tianlin.xyz/gtvfbnmdpd.html

[U64] PHP：目录遍历
来源：http://hz.havefunace.top/gtlnukwfer.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daxiang520.top/gtjkxjzmnk.html

[U65] PHP：会话
来源：http://hz.shangyingyoupin.top/gtgmfmafqg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.pycfn.com/gtwhdnqxaq.html

[U66] PHP：设置 Cookie
来源：http://hz.birdmap.top/gthudjyrgl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.316326.xyz/gtcbvavfvb.html

[U67] PHP：处理文件上传
来源：http://hz.hammf.cn/gtqjwrjrjs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhengqikj.top/gtuosbdeto.html

[U68] PHP：PDO 连接
来源：http://hz.nanxinkj.top/gtcshyipxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.daxiang520.top/gtkifrgzxw.html

[U69] PHP：PDO 预处理
来源：http://hz.mhx1999.top/gtxnyrbqbw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgfzy.top/gtieapzodk.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtvopblcup.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenzaomai.com/gthzpwcnrb.html

[U71] PHP：抛出异常
来源：http://hz.xuanzx.com/gtewktecgb.html

throw new RuntimeException("失败", 500);
来源：http://hz.aibaodan.cn/gtiavxsgcu.html

[U72] PHP：写错误日志
来源：http://hz.jqgfzy.top/gtgnyhtkxg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenzaomai.com/gtrsvxmhjg.html

[U73] PHP：读取 ini 配置
来源：http://hz.wangdashe.top/gtkndeorqp.html

parse_ini_file("config.ini", true)
来源：http://hz.ehwqpu.com/gtuhdunwfs.html

[U74] PHP：读取环境变量
来源：http://hz.nanxuanxn.top/gtfknaqgbv.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cucudq.cn/gtcoedjtxb.html


<!-- 参考信息 -->