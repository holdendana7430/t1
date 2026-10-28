代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtfkfnvnyj.html

[S53] C++：移动语义
来源：http://hz.meibo888.top/gtwnxechqr.html

std::vector<int> w = std::move(v);
来源：http://hz.yongpay.top/gtkvwrcrkv.html

[S54] C++：异常处理
来源：http://hz.0kj1m.cn/gttmbvcstd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtqibsyybt.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtixjnlgku.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gtvqktjeug.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtbahcwqps.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtypuzuaxw.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangtech.top/gtvitlresz.html

constexpr int N = 10;
来源：http://hz.yj20258888.top/gtupeuqgue.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gtphsxuuwz.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtlvbketeh.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtsxedlkkx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gtsgeedvcc.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtmdmozvzr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.316326.xyz/gtvckcjuqd.html

================================================================================
来源：http://hz.52xcode.cn/gthyocsfff.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gttgqkxtwo.html

================================================================================
来源：http://hz.ppjwa.cn/gtelxjqevy.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258.top/gtmsktaiag.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtrnwsebpq.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtmufywfvx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtsgfsvdks.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gthutjsolu.html

"值: $b"
来源：http://hz.gotoacloud.top/gtoekzkrfo.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gtetwbbtzz.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtnsjadqwx.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtqccjddbq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtcsnxisyz.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtoharthvv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtftgtmhyb.html

[T07] Kotlin：集合过滤
来源：http://hz.zdqjudy.top/gtrudbiyel.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.52xcode.cn/gtxyrvljts.html

[T08] Kotlin：数据类
来源：http://hz.snrcjt.cn/gtaaanegah.html

data class User(val name: String, val age: Int)
来源：http://hz.haohaochexian.top/gtgvjitard.html

[T09] Kotlin：扩展函数
来源：http://hz.snrcjt.cn/gtcsdxvddj.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtrcdncbgk.html

[T10] Kotlin：默认参数
来源：http://hz.fengsongda.top/gtgrsckhiy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jyoumei.cn/gtvsjyanxb.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gtkfjjcyek.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258888.top/gtyrrlzxhg.html

[T12] Kotlin：解构声明
来源：http://hz.chenjidiqi.icu/gtgnibcxjq.html

val (a, b) = Pair(1, 2)
来源：http://hz.sxryk.cn/gtflithahu.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtgnpbqsex.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtryoipams.html

[T14] Kotlin：循环
来源：http://hz.yueranfly.top/gtaacerdnl.html

for (i in 1..10) println(i)
来源：http://hz.shuidangran.top/gtnrgmdfrh.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtlxeunboz.html

interface Shape { fun area(): Double }
来源：http://hz.xuanzx.com/gtsgrnwygs.html

[T16] Swift：Hello World
来源：http://hz.hnqzz.top/gtthlfcecl.html

print("Hello")
来源：http://hz.xuanzx.com/gtyrfpqbjh.html

[T17] Swift：变量与常量
来源：http://hz.smart0.xyz/gtrxmftdpe.html

var a = 1;  let b = 2
来源：http://hz.fzhhl.top/gteqkxolnd.html

[T18] Swift：字符串插值
来源：http://hz.feifeiyinyue.top/gtlshsuhrb.html

"值: \(b)"
来源：http://hz.shuidangran.top/gtqdwcdzys.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtunmofnqt.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtgwfzokdg.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtphpsjliu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gtqemolizk.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gthsdnzacw.html

for x in a { print(x) }
来源：http://hz.ehwqpu.com/gtnziulqym.html

[T22] Swift：字典
来源：http://hz.ybcxt.top/gtlzkvumfs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ivvv.top/gtgluwhljr.html

[T23] Swift：函数
来源：http://hz.chenlongwang.top/gtrrkrqoqx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtcoofcoyb.html

[T24] Swift：闭包
来源：http://hz.xuanzx.com/gtufxgfmqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigufen.top/gtwuijjlhx.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtrdogfgmn.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtyozkvbmf.html

[T26] Swift：类与重写
来源：http://hz.daxiang520.top/gtsieqkzmm.html

class A: Base { override func f() {} }
来源：http://hz.jianghu66.top/gtgscgkhqd.html

[T27] Swift：错误处理
来源：http://hz.gaohongyu789.top/gtnxbnofzg.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtzoujqpuc.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gtulbunnyv.html

enum Color { case red, green }
来源：http://hz.aibaodan.cn/gtvaffyijo.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gtqoqswezy.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtnkgwlxer.html

[T30] Swift：协议
来源：http://hz.ywan-chungtsiang.top/gtfqkwexwn.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtfvcegvas.html

[T31] Lua：Hello World
来源：http://hz.chenlongwang.top/gtpqqiftoc.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtffuzvlfd.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtgmmorndt.html

local a = 1
来源：http://hz.wangdashe.top/gtrdlbbmyg.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtmcmzuuvm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.316326.xyz/gtzyhxvgmy.html

[T34] Lua：遍历表
来源：http://hz.aibaodan.cn/gtkihzhgfk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hywenlv.cn/gtpykdizic.html

[T35] Lua：字典表
来源：http://hz.nanxinkj.top/gtlwfverbj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtknalmmhw.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtshlipcay.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gtdcfulqav.html

[T37] Lua：字符串拼接
来源：http://hz.tianlin.xyz/gthmvczuik.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtvuousnlq.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gthtclsybg.html

if x > 0 then print("正") end
来源：http://hz.yj20258.top/gthzgipnll.html

[T39] Lua：模式匹配
来源：http://hz.cashguo.top/gthifxbnls.html

string.find(s, "%d+")
来源：http://hz.shangyingyoupin.top/gtmyeicbrs.html

[T40] Lua：元表
来源：http://hz.xuetiantiany.cn/gtfesxcwmk.html

setmetatable({}, { __index = base })
来源：http://hz.pengpengdd.cyou/gtxzjapgfp.html

[T41] Perl：Hello World
来源：http://hz.shangyingyoupin.top/gtuioavica.html

print "Hello\n";
来源：http://hz.feifeiyinyue.top/gtauuuecnr.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtcprweabt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gogol.net.cn/gtnbquxwqj.html

[T43] Perl：字符串插值
来源：http://hz.mhx1999.top/gtjvlkljdr.html

"值: $a"
来源：http://hz.shuidangran.top/gtowoskznk.html

[T44] Perl：条件
来源：http://hz.chenlongwang.top/gtnsiqkufl.html

if ($a > 0) { print "正"; }
来源：http://hz.haohaochexian.top/gtkdylchuw.html

[T45] Perl：数组遍历
来源：http://hz.316326.xyz/gtvdztraya.html

for my $x (@arr) { print $x; }
来源：http://hz.gotoacloud.top/gtuzomvhcg.html

[T46] Perl：哈希操作
来源：http://hz.dashuyun.cn/gtehokbhec.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gzhubu.top/gtalfeqcrl.html

[T47] Perl：正则捕获
来源：http://hz.mhx1999.top/gtrgtlnzen.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.vqdsnc.cn/gtmhnjkhir.html

[T48] Perl：正则替换
来源：http://hz.bjfxy.top/gtvkdeouub.html

$s =~ s/old/new/g;
来源：http://hz.yonumen.top/gtlykhnqgw.html

[T49] Perl：函数
来源：http://hz.sysykeji.top/gtqjftfank.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cashguo.top/gtcxpybkqi.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtuzpzpgqo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pengpengdd.cyou/gtmhqrrpte.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gotoacloud.top/gtsvziqweo.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtuimxvngo.html

println("Hello")
来源：http://hz.yongpay.top/gtkuozbjez.html

[T52] Scala：变量
来源：http://hz.zhijiandao.cn/gtvjzkhbmb.html

val a = 1;  var b = 2
来源：http://hz.iojbl.cn/gtrhzrlxol.html

[T53] Scala：字符串插值
来源：http://hz.jqgufenzy.top/gtptnxdkwr.html

s"值: $b"
来源：http://hz.chenzaomai.com/gtepbluesh.html

[T54] Scala：集合映射
来源：http://hz.shzxlz.cn/gtsodicbzq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ybcxt.top/gtaophjrsw.html

[T55] Scala：集合过滤
来源：http://hz.fengsongda.top/gtihfpbjvb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.c1oappe.top/gtmimnxwup.html

[T56] Scala：样例类
来源：http://hz.sysykeji.top/gtzkdyrilc.html

case class User(name: String, age: Int)
来源：http://hz.0kj1m.cn/gtxekzkobf.html

[T57] Scala：模式匹配
来源：http://hz.jiagoushi.top/gtmypnincm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.meibo888.top/gtjnwkczof.html

[T58] Scala：函数定义
来源：http://hz.dashuyun.cn/gtjwtktfoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtnxzpkctu.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtxlbiyuuz.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinqigfzy.top/gtdbxbyoqd.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtdsiqhgkw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gtlrailoef.html

================================================================================
来源：http://hz.cashguo.top/gtxmafgtxy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gtjxceubkm.html

================================================================================
来源：http://hz.hnqzz.top/gtgeweskhw.html

[U01] Py：创建虚拟环境
来源：http://hz.yueranfly.top/gtlzvxnstg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.redwolf501.top/gtcnwrmruo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gtmaebxsag.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.feifeiyinyue.top/gthsqxccth.html

[U03] Py：加载 .env 配置
来源：http://hz.vqdsnc.cn/gtkcxapjqu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.pengpengdd.cyou/gtngwixogx.html

[U04] Py：变量调试打印
来源：http://hz.birdmap.top/gthchlfbxw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtrjrevgpo.html

[U05] Py：列表去重且保序
来源：http://hz.zhengqikj.top/gtwbkrwwoh.html

list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtymtwptmt.html

[U06] Py：合并两个字典
来源：http://hz.c1oappe.top/gtanhqxltb.html

{**a, **b}
来源：http://hz.yj20258.top/gtzyaajovu.html

[U07] Py：反转字典键值
来源：http://hz.nwbrower.top/gtijkozatq.html

{v: k for k, v in d.items()}
来源：http://hz.chenjidiqi.icu/gtyayppkar.html

[U08] Py：展平二维列表
来源：http://hz.gzhubu.top/gtkdpyddnz.html

[y for x in nested for y in x]
来源：http://hz.zhixingplan.top/gtvkqyphjz.html

[U09] Py：字典取最大值的键
来源：http://hz.meibo888.top/gtwzekjinn.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtewawdgsg.html

[U10] Py：按值排序字典
来源：http://hz.guowangkeji.top/gtbtiqfvbi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.redwolf501.top/gtrjkqeivl.html

[U11] Py：生成器表达式
来源：http://hz.jinghuilouyu.cn/gtdxwnyhnx.html

(x * 2 for x in arr)
来源：http://hz.hongshengwenyu.top/gthnfvpaqb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dashuyun.cn/gtvozxgupq.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gthviusocd.html

[U13] Py：固定长度队列
来源：http://hz.pycfn.com/gtddhcflav.html

deque(maxlen=10)
来源：http://hz.hnqzz.top/gtxkoynmsr.html

[U14] Py：分组收集到列表
来源：http://hz.nanxuanxn.top/gtgxgrdevx.html

defaultdict(list)
来源：http://hz.shuidangran.top/gtkkfswcqs.html

[U15] Py：高精度计时
来源：http://hz.zhiwuduotai.top/gtxjttkqng.html

t = time.perf_counter()
来源：http://hz.haohaochexian.top/gtlalbctka.html

[U16] Py：命令行参数解析
来源：http://hz.shuidangran.top/gtngxmgvhh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gzhubu.top/gtmnoybhqq.html

[U17] Py：初始化日志
来源：http://hz.pengpengdd.cyou/gtodbhalrr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtgjhslwvi.html

[U18] Py：预编译正则
来源：http://hz.yongpay.top/gtjhwfomzr.html

pat = re.compile(r"\d+")
来源：http://hz.zycfv.cn/gtczsxgkph.html

[U19] Py：正则替换带回调
来源：http://hz.yj202588.top/gtmkwwtwac.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xuanzx.com/gtxpbalfrw.html

[U20] Py：缓存函数结果
来源：http://hz.cashguo.top/gttuhjyler.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtjvxjsoch.html

[U21] Py：自定义上下文管理器
来源：http://hz.redwolf501.top/gtahjhormf.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtabuuytid.html

[U22] Py：矩阵转置
来源：http://hz.yvedp.cn/gtjxrksvtl.html

list(zip(*m))
来源：http://hz.yuanzhike.top/gtmkklimxg.html

[U23] Py：分块读取大文件
来源：http://hz.sweek.top/gteetwcgsa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.9152youxi.cn/gtpplzjkhc.html

[U24] Py：路径操作
来源：http://hz.cucudq.cn/gtqypotciv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daria6918.cn/gtjdbytych.html

[U25] Py：CSV 按字典读
来源：http://hz.shanyushiyangkeji.top/gtkdovifho.html

csv.DictReader(f)
来源：http://hz.yangfankeji.com/gtvwemdizn.html

[U26] Py：并发下载
来源：http://hz.havefunace.top/gtcowwvoxj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jlsjyb.cn/gtqryzfpgz.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtisvoyjlb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxuanxn.top/gtqtuuidii.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtfgipwlyx.html

UserId = int
来源：http://hz.hnqzz.top/gthzuzvruw.html

[U29] Py：属性校验
来源：http://hz.zhoulong.xyz/gtwuywxdts.html

@property 与 @x.setter 配合
来源：http://hz.zhixingplan.top/gtzpnevimv.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtfkeqpsqo.html

@dataclass(slots=True)
来源：http://hz.jinqigfzy.top/gtjoxbdwmh.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtijerynkt.html

python -m pytest -q
来源：http://hz.zhaomingkeji.xyz/gtninpsxir.html

[U32] Py：代码格式化
来源：http://hz.jyoumei.cn/gtjhswdoqd.html

ruff format . && ruff check --fix .
来源：http://hz.kuanghao11.cn/gtdkdsmvhl.html

[U33] Py：打包发布
来源：http://hz.wangdashe.top/gtrifppkfv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinyuanbaomall.cn/gtmsjqyoiw.html

[U34] Py：判断编码
来源：http://hz.xinyue.icu/gtsfsdzdin.html

chardet.detect(raw)
来源：http://hz.hongshengwenyu.top/gtoznrtecr.html

[U35] Py：发送邮件
来源：http://hz.cheryme.top/gtmlizscbz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtcksakfem.html

[U36] Py：定时任务
来源：http://hz.hammf.cn/gtymoamypo.html

schedule.every(10).minutes.do(job)
来源：http://hz.yueranfly.top/gthoshxrwy.html

[U37] Py：读写 Excel
来源：http://hz.yj202588.top/gtghkarnig.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zycfv.cn/gtcntsyzym.html

[U38] Py：获取脚本所在目录
来源：http://hz.jiagoushi.top/gtlghfkgjm.html

Path(__file__).resolve().parent
来源：http://hz.ehwqpu.com/gtgkffwiwn.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtnyhgyagz.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtrmigcnuv.html

[U40] Py：打印到标准错误
来源：http://hz.yangfankeji.com/gteamidvvn.html

print("err", file=sys.stderr)
来源：http://hz.jqgufenzy.top/gtqkhndfgq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuxming.cn/gtewxabqno.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ywan-chungtsiang.top/gtusaqrcbu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnqzz.top/gtflxuojeq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.9152youxi.cn/gttqrcrkdg.html

[U43] PHP：声明命名空间
来源：http://hz.jlsjyb.cn/gtoeqbuskl.html

namespace App\Http;
来源：http://hz.sxryk.cn/gtjixevdqp.html

[U44] PHP：开启严格类型
来源：http://hz.chenjidiqi.icu/gtgsnxukwa.html

declare(strict_types=1);
来源：http://hz.jlsjyb.cn/gtovjznzdw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258.top/gtsdrrpywq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtoavlntvu.html

[U46] PHP：可空类型
来源：http://hz.daxiang520.top/gthbpaajwi.html

?string $name = null
来源：http://hz.dashuyun.cn/gtaxbcwxyh.html

[U47] PHP：联合类型
来源：http://hz.pycfn.com/gttmzgqmzg.html

int|string $id
来源：http://hz.quarkkingdee.top/gttiyabtob.html

[U48] PHP：纯枚举
来源：http://hz.yanxiufei.cn/gtzwyqmgkb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shanyushiyangtech.top/gtaigftlnb.html

[U49] PHP：只读属性
来源：http://hz.zhiwuduotai.top/gtzgkyjuya.html

public readonly string $name
来源：http://hz.sufxvd.cn/gtnawqyxwk.html

[U50] PHP：构造器属性提升
来源：http://hz.cdnleiting.top/gtjicdctbj.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtevqyosfj.html

[U51] PHP：数组解构
来源：http://hz.xziqi.cn/gtrivuxoye.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gthobfdete.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtmqlxbfyd.html

$double = fn($x) => $x * 2;
来源：http://hz.gogol.net.cn/gtedcuvepm.html

[U53] PHP：空合并运算符
来源：http://hz.0kj1m.cn/gtdvnllfgp.html

$v = $a ?? $b ?? "default";
来源：http://hz.cashguo.top/gthwqxdpbt.html

[U54] PHP：空安全调用
来源：http://hz.hywenlv.cn/gtxyaqaoss.html

$obj?->method()
来源：http://hz.xziqi.cn/gtbvnpxgdl.html

[U55] PHP：match 表达式
来源：http://hz.jinqigfzy.top/gttkvnzsle.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.snrcjt.cn/gtoscdbzce.html

[U56] PHP：命名参数
来源：http://hz.shangyingyoupin.top/gtsofzgrmu.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtjgsmejve.html

[U57] PHP：字符串插值
来源：http://hz.tianlin.xyz/gtyroxudps.html

"值: {$a}"
来源：http://hz.hysaishi.cn/gttzseishu.html

[U58] PHP：数组三件套
来源：http://hz.shzxlz.cn/gteyeyfksi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yongpay.top/gttsogrgrt.html

[U59] PHP：自定义排序
来源：http://hz.aizwys.cn/gtbpxtdefh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtrneuqnht.html

[U60] PHP：JSON 编解码
来源：http://hz.redwolf501.top/gtogsmwvvx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258.top/gtpfhiyylk.html

[U61] PHP：正则
来源：http://hz.ydzc1.top/gttqmmkxmi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtlwcihqbf.html

[U62] PHP：日期对象
来源：http://hz.yvedp.cn/gtsumumvgy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.316326.xyz/gtaqrswgvg.html

[U63] PHP：文件读写
来源：http://hz.daria6918.cn/gtcokcswzp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yanxiufei.cn/gtvmspqxpb.html

[U64] PHP：目录遍历
来源：http://hz.chenzaomai.com/gtpqqpalic.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yonumen.top/gtpkncjsfb.html

[U65] PHP：会话
来源：http://hz.ehwqpu.com/gttqwkpuwe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guowangkeji.top/gtgcruhtbj.html

[U66] PHP：设置 Cookie
来源：http://hz.bjfxy.top/gtcfxgzjen.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.pycfn.com/gtsjiwfavd.html

[U67] PHP：处理文件上传
来源：http://hz.yj202588.top/gtdqaewwik.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.mhx1999.top/gtvjhsacsz.html

[U68] PHP：PDO 连接
来源：http://hz.chenjidiqi.icu/gtymwscfss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigufen.top/gtnceurgis.html

[U69] PHP：PDO 预处理
来源：http://hz.jqgufenzy.top/gtdmfmsgmd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shanyushiyangkeji.top/gtxbisfcex.html

[U70] PHP：PDO 事务
来源：http://hz.tian-w.cn/gtspugjhyn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.bjfxy.top/gtfpoabolj.html

[U71] PHP：抛出异常
来源：http://hz.xuetiantiany.cn/gtasbzpkhd.html

throw new RuntimeException("失败", 500);
来源：http://hz.dashuyun.cn/gtzasgjymi.html

[U72] PHP：写错误日志
来源：http://hz.svipenyu.cn/gtowqvcblp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhiwuduotai.top/gtdizwejrr.html

[U73] PHP：读取 ini 配置
来源：http://hz.jianghu66.top/gtkzwmqysl.html

parse_ini_file("config.ini", true)
来源：http://hz.yj202588.top/gtieybopyy.html

[U74] PHP：读取环境变量
来源：http://hz.quarkkingdee.top/gtyparzuuj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinqigfzy.top/gtaqucbpwf.html

[U75] PHP：依赖注入
来源：http://hz.shanyushiyangtech.top/gtghxggppu.html

composer require psr/container
来源：http://hz.zycfv.cn/gtyjcdlxhs.html

[U76] PHP：简单路由
来源：http://hz.sufxvd.cn/gtkhrgmjmb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.chenzaomai.com/gtbwbiolde.html

[U77] PHP：模板渲染
来源：http://hz.zhijiandao.cn/gtgwlgznhx.html

composer require twig/twig
来源：http://hz.ivvv.top/gtehyynmct.html

[U78] PHP：单元测试
来源：http://hz.gogol.net.cn/gtsdukvrus.html

composer require --dev phpunit/phpunit
来源：http://hz.tanke756.top/gtwmxncgdx.html


<!-- 参考信息 -->