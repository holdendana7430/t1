代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rdlhgjxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpspclua.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mkjjdgml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beerxrue.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dvjhsmfb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qdwqdrjd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lesudxha.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xrpkedtw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zobdjaiy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3naeyffhp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bmpwolha.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kzqgkgsk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hhwpotwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jqhkgjne.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lyelgygd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cqnfvmbp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vrrtiquf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rfnneufg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rlpyrtpe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jzfjjcmr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ohfjyqlm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3reokmoxp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ylbixpze.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3clcgfuov.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xuyhwrko.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wvmysivj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wuyvkpac.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drdfsbak.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iddomsrb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuknjfhq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ccohduhe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mdeafaka.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qdhuslpn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqexfrs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cucmuorw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pabacmsm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ladxbfus.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pbdtmufn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eaqppocc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uyokdxmq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ghufxtvg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fgibtcel.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mcabirey.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmhsuono.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3npqvrgzc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jtrryfzo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ugjeqmda.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jymysgsn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3njpnsuwo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwtnqrc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3osakxdhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3crarzsee.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3knubdyop.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3eeswtkez.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qfbbdent.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hfzeajso.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zllsltxq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3elyefngj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zmcroqoi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ajgalzmv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pbydvxrl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lfwwuosl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ofvpefqg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqnltyl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hzfreehz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sepzadtg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vbfjuynb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3eoergvcs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hgdeywyo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3glxggpao.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3flnuypbz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rnpguvjc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3odwllcsy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3aplnmvgn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyvgapfh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hdtlxlwe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cuwjnuhz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iptqailu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wscxcaun.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eetgkrmx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3huhtlrab.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nzudajqz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lmozytzi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pldhdoln.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdsrkuix.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ldeelheh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oreegibn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hgmvpfdf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3penvdoym.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mvbnsmkf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wibeujcl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cwdovkrb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eyrjcbwj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3oakykxgt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3lulqngap.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swxdndde.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kjtbqzca.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lpmpdbwu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3koonvraq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mnkkeokr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpojnahm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rsmjnbhl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3noaapswq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hnoialxu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nwbwjofc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ehvemtrq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ppldhuhj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3treataxp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wheesmrj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3loxjjzhi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xteitokz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3idgutqqj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pehhjhdr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kvmscewe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3psuimwsk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dhxjsdmj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3irecourz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rwrnmafx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nplizmke.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvxzdbck.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uomsfesj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fhlbhuqk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qfppkosm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pqkxddke.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3odeilgkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shlzzjkp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pvzuhvtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oocbhtnu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3etooizig.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xgxqbtpv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iltuiflv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vsybleoz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bvgwytwo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kmtwtcqf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xiartxyd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yenjrbzu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3svqxaact.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hzogbmry.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vbblphvd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nbzsxxyt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3twapobbs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3aefcbzwv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ddlxmquv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3akioqfjc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vxinubqg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3keaoosxc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jmcogbyi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3avqjuvdc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3akqljbte.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxzfywe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fjbxapvc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbkkbbh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nncfamwn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmtqxkw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ncctwlwb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kddwdthq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3htdqmlcd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wcvvtgkb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mtshvwqb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sfwcqaas.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fqfzzffd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3oofwkbef.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vowgwoeb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rivlmhkr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yaegiwug.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gylbpbna.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3aambhjyk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3eafjkblz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3svznmjns.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ahhvjnyy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ammtehtp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ezdoovnq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hgatgxlo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tkjgrume.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zjibhqlr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dofehvhf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3raxzgnye.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vnmsalpb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3yfjnnfwf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wogwlgde.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3osazwkwl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ksbkafzc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dygjgdyg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3haobyvbh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bthnupvd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nvsoejhq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rzvpqtfv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kqmkkeqz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nuhidujb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ejtpvkap.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pisyxkvn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3egxbjjyv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3iezkifbv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nmxeekmb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hnhcqolz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fpalrcnd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3iqwnyitt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jrwdbxyk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jsqresop.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wnrzjrzq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wfgbivbn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3eggiramc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nmlpzmkw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qldzbita.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3iwqdgdxq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rohwsuls.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3idmehwdl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdjqcxc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jhbtseih.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tolyxtwc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hirjamne.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lplcmazc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pdvwtezo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wuosrgdi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bjgifoik.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mnaaejiw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kzozearn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcegayie.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3brpwbecq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bimtnzhs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kdjsrmtl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ygdluafh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mlhfaxys.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldmrohpm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ayiurwzr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3owefweyl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qkcvrneu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lshtrxrl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bnkvtzpa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3idswpvaf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggfgocyr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ztpkumjf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3rppjbmkf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ihvwjrec.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gbnjcivn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nkrfqhqj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3apbgejmi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nsdrjfnj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ndwpyoux.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3otszczsj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yrqzjxpu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvkftrfw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tdqacsyo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtbqyqbe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3olcirahs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tvoebcxp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3eahtqscw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wzmxnldp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jfnfhubs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ythhrxvt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bddvpven.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rwqyqpwa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ivnzesse.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mtdcvwtx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kidsfgqv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ojkizxln.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sobyzmql.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aqbyiqwx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gkvudfcc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xzkqjhsv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vxgibqiy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gdqfevwm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tuxtygnr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3sxzgqcxp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zpcwlktt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mzmadndd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zkwpsrjc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kbxciaja.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jwswcabp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lxootemr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3odakgylb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lgmedekh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uxwuvhek.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcotqlw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkepeszn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3aknugixd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3eeetpryt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3crayacuz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3oxihgkox.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dycukjjl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vcfbwtxy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pioikidk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mhsxavuf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3feaigifz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rsrauedi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bclzeyer.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ahvajvvy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3poxrfqwv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xrxkfnwa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gpufvbvj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zjtfrhwt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mftinruh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vdtpcntv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wquyuanf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zvyvfepm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jmucfnxm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uhrakyty.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3leadqher.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yxexvjdy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3npgxglpk.html


<!-- 参考信息 -->