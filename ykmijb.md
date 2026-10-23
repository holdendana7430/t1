代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mvcwptdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3figcbluf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nbyiqova.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plhqhsht.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zxbojvuj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xmkhwyil.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhlphefu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ksuarrkj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zkqqvplj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kpstdzbz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tfodaahb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ttrhbwvj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mlvccgah.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pulgpkhr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pcrqneph.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jphwewro.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3etkedths.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dqazzmtp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mrdjulxz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zowjwawj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3erlxxowp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gfizmdpc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3boudaxlm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eznepwyn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3texkuunl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zaolatwu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vzsjjohk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmsdtnao.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ertaamuo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgmbqgn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pxhwagks.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvwwmtf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rpimogci.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3chpoyhpk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qttejjwj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3utbgjqvw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zjyvnmae.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hhrcfsvq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zeylqkjt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ftfztfko.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ddktmxwj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nibsyprz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dxbshsho.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tyqpstxe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uefghzec.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fwstnjqk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3initohmr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wurlafon.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqsonkle.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ippaqerc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3voeogfff.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iellqrla.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sxsnpmjr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bbzidfnf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wkzhvcpo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bbhrwfkp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dlyeaovk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gedyzpio.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lqopejrd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdujgob.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3coanxakg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nspejfna.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kzjyuigo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dgzwbfqr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgmzxfay.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xwxtniiy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3achibfcz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nvkkwbmy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lapavokt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tbfcsagd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fgwtwvpm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xwwtynvv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qqjhbzfl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bwdkrunn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ltrhfcjw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xyvrtbfr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xzbqsxtc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yylqjigb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3umbgbjtc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zxtpzjdb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hrftbtfm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3abkfwgmv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mhgemcbk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yjiybaai.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xbdosbxu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dkrpycgu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3luftusio.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fcvfcpcq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3joktipsk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dsymruwv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vpforaye.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgemvtgr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qfwrcmgi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmkntrtm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ugpevsbq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3twzduimm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3aivhjlst.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gueyfhcm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yarywxbx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rwrigrcd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3beqlghwe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3opqnoknb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ijnczawa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jnjrbdot.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rkycnqfn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvzewmnn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rlukjleb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qqztfmyz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ztfixhtg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wkckxtze.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3irrssfug.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qdyfpiff.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmpntwv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zimdeoto.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xmttvnuc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tplhrucp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vbnejkiw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tbuekchx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nzkfdaip.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qbvddjpy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wheooncr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3uauzyjic.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3khrwzqmz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ndlryswt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tfhkwkvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yidstucq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3slwmppsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axqzrzmt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hluctznw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3eluyaiff.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3fvwxkpmc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cqcoqunu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wsdjwewl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dohmovda.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wvdnkezb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3btfgwbov.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jkgtddxp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lbguzhpz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lldbpxxj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3voobtjdp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cujqdjgd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3iafsojsg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lvshaxkl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hanhgkui.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xobuszdo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vlkualgh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yzivvhmv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3krcwgbpq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3umrqqmzo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3svnpmxcc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dwfnkbxp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vlnzsrue.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ztaogpcw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pmrxtgkh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gaxncnnf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3oslrsjdi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wyvzdpwe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3glifohdp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jtdtylwk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3llnofovs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3opbwelug.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3asgfgxkq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3icjipcjm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mutssqyu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yfnkltrp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sarffxhj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3fvcvtwiy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rajlktrw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zfomydkg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nxitjwup.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kjskduxn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fpninqaw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tbplqyzb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3iqebrhta.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cbzhjhfy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aeazsjoj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3odsiolju.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vxkgabyh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ojqujvpu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3oqkohoxt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aeeilwgb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dfofosae.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ozbrsqjw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wshvibpq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nkmmkokf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qsrqtbii.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nxgjtlgr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xoswwrea.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mqnvqerj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3coikorvf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lvmiunsh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xvcmxedk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3crugdtjc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oqyztcra.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3oskqfhts.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qldrsbmn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3llrpwgid.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3txvgzcue.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wekbodlp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3lehsgcnl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lpuvjxtf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xphpvpvl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eenpuoar.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3maztseja.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3gmzldtou.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pbrlelkq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dlyqpura.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqchtpzg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tgdygoyl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrrehl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3eqqyaesc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rbomlwxd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jslihazx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3chlhzfes.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3viiizsvc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dojfaiwy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3cifhbymd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwqapafs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lfomysqm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vzwavluh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqqpshzo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uvayehrl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xbmduywj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkhmnkbc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jkrelier.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3pphuymgw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ouhcsipw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uvtpdfgw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sfzjquom.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hkbznvgm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3thrymnaj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hnbbkxwt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tkttqoag.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3axmkqsrb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3txqmgzdu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ucsveehd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rapfhrtw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qcxxrsqy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3imvvshfn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3czwnknqa.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wmwikdvm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3peqhqwwr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jmqcizbq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jykuunpa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3xhhclevi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wzpbonwr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3soedguzr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tvjynaiu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3brqljqfh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hqzpsjny.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mpagatiw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qlduqxmn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jolwxwpa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3spmvboqi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gowjzmnb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hnxyjwvb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pawkmzzg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nzufxwqy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hdqnllbw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rophujuo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wovscncc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lhvjidij.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yoodtvqo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wvvwgzdf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lidrkcrt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhdxpnwd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qvhaakyh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lpyxdvph.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xrmpxpiq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bcntslew.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3latqrtkv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ahcblmxn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lnvgtoyv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcduqgm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zheurmhy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3muxqgklw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3leqpgbwk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dpazvntk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qiqhzexr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3unzgetag.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hxszxndb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3srotkkmk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gznpyszy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zfrwgszl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zdjwfeww.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ghxhsyto.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tbampywt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dxiyiwxk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rgqlvmeg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rkgghihf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gwawyvtm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qjlbqtcp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hgkdnsiz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3anymcgce.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eauvizxp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kdsqohxf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3adlkpqru.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tballlqh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3awmkqikj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xzxeeadv.html


<!-- 参考信息 -->