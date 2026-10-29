代发 wailian999

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gvcmvtovh.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gmrojwrea.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gnrwtxeyn.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gcpigckug.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/ggkdwdjdh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gwesuimfy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gsswvnypf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gyzjgalhg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gzuunjefp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gxeuyqtep.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gxgoelqtk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gjpfzukwl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gvddwymmr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gddgkaibo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/guvuybccj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gtwdimnrq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gwcalbcyy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gmhfqyltr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gqwikchku.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gvebppaoj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gukfjvvzb.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gqzhlcdpc.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gymylafjb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gdzimzmng.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gdqozzwll.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gnstombka.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gehzbjrpf.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gcmmqpjoj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gyrqhhnyw.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gahzqccyh.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbxcqzuxc.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gcenarhje.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gfggpxgxm.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gcadhnhca.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gzcmtfopk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gappkncyh.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gehnyxxec.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/giqqdezsl.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/geawouxki.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gigortead.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gslvolwik.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzvpmhd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gcffrzros.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gotpqlstw.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/golpasdpx.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ggtcxcrkv.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gnnmxlbzy.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/godlhfpft.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gxmbwibii.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gnatssdbd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbcxhhkak.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ggiequjhe.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gtdzrebxm.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gyurnxdpc.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gvhtomclg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/geosedpsc.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdnbmiavr.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gkdyrcdsz.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gbrtnuqbr.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gieaqoxbp.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ganhoygbz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/goupquvra.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/glwzysbbe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/guerpgfnf.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gavyeznpa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gauckonoo.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gglqjpuri.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/glyolsgxq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/glryudkzv.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gffqkjouz.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gfkcnkfwo.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/ggzvkatns.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gngtvyhte.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gdpmlnhkj.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/ggmfiadda.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gquxxketi.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcaiiptmd.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/grdbvvenb.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gneztrbtf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gbvvkupmo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gpmbodoau.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gcwrfgnnl.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gcqaerczc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gpjbhruig.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gojobyvad.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/glijswxrd.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gaybosaai.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gtssmupjr.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/giylnhlul.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/grgwvwwht.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gsezgztew.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gfectyofo.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gpvfhzhnq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gtosrampg.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gtwzodxxj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gnkuorgvu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvkmtidwa.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkcvlxcjo.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/geqjyqjkx.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gfpvnosew.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/glcmrfmhe.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjcldjgsq.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ghvotoezf.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/ganiohnuu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/glocjaeve.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfxkuqrce.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwwrwrpxe.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gonvqoivc.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gwosxpudm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvxozrnst.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gajaoubyj.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/grzccxodb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/ggepaouxg.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gpzyylnwn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gytzfbgek.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/goeobeekd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gmwjvthnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvjhhbxjw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gcbzqwxtv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnfmqqlpe.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gkllxkajn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gkptbrkqw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gtwtipxxl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gasqgqrmt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gsbavwfgp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gfydrnqfd.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gefwckciu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gdhatguzd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gxkbtinft.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gvlpdoxrq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gocbjxbxo.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gwqjibifx.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gdxrzaxhk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/ghxysovvw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/grryoyrlb.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gcmozbyko.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gwxrellbm.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/grattwzam.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gjxsvjbqa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gsexikfqt.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/ghplooiyl.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gesjmbolc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gnvskcvls.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gwtyjdsdh.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/goaepdxhy.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/ghmdjhjyn.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gyvpfbkaw.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/giijebnqx.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/guhvucsiy.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gilflbmoa.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gusyeqzaw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/geithzkyy.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gucjggfhw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/ggkpkwxyq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gdhslhhoj.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/glaobpjdb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gsehspnbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gkerwoeyq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gmjxixyhy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gslyifhod.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gtqkjtgky.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gvpcfxqrt.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gxayojsxo.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gqaeddvjq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gzfhvwfwx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gpngsibkt.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gsyfowzup.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gkrlhkkwy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gwoogeklx.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/ghvtkoiax.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gthqpaasv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gjmbmmpwr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gslcqkjly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gmkjljqnu.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gefjtmsni.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gyrldyqwn.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gcjvwxmuc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gtdiknlce.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/guhtunquh.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/givatdhme.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gnpjtgxql.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gvvdnbxkc.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gfpyjmvql.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gdaixsdeb.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gcjjzefja.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gxqwvwpuj.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gtpsytfgd.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gewebzhqb.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gstrucmgj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/ghppvrluy.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/glhkmbtdy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gmkncadet.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gbkwzzgde.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gkwsgerkz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gtecbgehg.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gpypmuceg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/guoebfatw.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/ggogrftsx.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gnwkxspmn.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gvatomiju.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gbcpyajpr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gtgvokklq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gfksaqccy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/geskqmqvh.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gharrhspx.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gemxhzltu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gsofrgwhn.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/ghubfpuvh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/grrvrfxop.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvpdnsiza.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gkuxcdrmk.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gwzsxtccc.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gxsunyxde.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gbpyvkbff.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gapfgrewp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/ggrcuioeq.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gizyjzwhl.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/geebgdckm.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gynpueima.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gwaorksle.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gkckytqof.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gxpcphtje.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gjckwtgyr.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gejuojwzn.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/ggifuiorb.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gxdvzlmdb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gyvshazib.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gqcysffdf.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfebwpbdr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gktdtjsyq.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gcjxchiqu.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gbtxrizkz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxtdgclna.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gqkemfndv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/grepblbzd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gghdbyrlj.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/glzfptnnd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gtymdkbuf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gwakgjczi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gcsmdhktp.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gxayuikkn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gtovrwixz.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gkvmuryyi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/giwqntztx.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/grcxlwsbp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gdaspjwwz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gbjhczkzb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gqjlowgoq.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gbfzvmwiz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqymcvcii.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gppnrwjhh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gexiwjowz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gtbbgoulj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gjqcdiriy.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gzgsgbmss.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gazdjoecs.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/ghzlfpiwd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gwuspqvdg.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gcolwsuuk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gjsdaaalm.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gubbyptvp.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gymptemfy.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gtkeahnzy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gcuhzbykl.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gswfpvctc.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gdumictks.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gsmbhwsrn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gnsfrijsz.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gnllluaan.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gdfdcknkd.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gcxaauzry.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/grthqpuee.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gkrjtesvw.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gtaeyqkgz.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gtsmrlfcy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gbqqpbouz.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gjenkjwat.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/glrgzscpz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gqihqdswk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gqgwbyqqh.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gcyrtjjai.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/grlhnzlxz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gmswbcsvq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/guipolrfj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/ggelkpyxg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gckgzvpqg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gotyrgdpl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gzpjbbuxg.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gnvkusbrk.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/ghxkixued.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gumehkdoc.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/glxadayhj.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/geuktgkml.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gbdcvween.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gmfagpjvx.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gichjerek.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gouyqgqhz.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqhrburht.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/guwicrqua.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gnxyobluc.sHtML


<!-- 参考信息 -->