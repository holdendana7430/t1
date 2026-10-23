代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxiuqa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sgbxcmqn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bzqplfek.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3emhyjukx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3szoanfdl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cxjlafbn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wsuxxbua.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hvrkcarp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wcblhros.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qhmwzgbc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tseqrthz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqwtciv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yqjlijhf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqjdvlfp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wbrhakvy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nakwxtvp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jhjurhag.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mpywysje.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kyyaptlp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qbrvqscy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ygbifpph.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwhjjdm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mwgtbcpd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tcbksblc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jnoxnivb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzpmhwbh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uqmqjvmu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wzjhzbwu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eaqjpjai.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sqykajvi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vooxxlag.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lfaflajw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bhhcaylr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ehnenjjw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yynqjiqv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3oavrylxd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3deelxseo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kjbobayt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hnwbmmdy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qpidouix.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ocvpoxsc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qcsvfcul.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tpubskdb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pzavwimv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gepagzaw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ruetejqk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wnvxovlw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rwfuzzxp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lbhigdud.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3quzzjsec.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mbfsfbaf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3utbwtxbi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3eoprtnmd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kyytsyqv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uetototj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wceesstr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qbfkilag.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kfexlkmb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3dxgtpdxq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3drnhfamn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ksujahuq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3asfwsjfp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ahjxfimg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlifogkq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fssojqyi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xdhehlvn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qrxnpeon.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ecqifppd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3azqwkcxb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xhbnfkpz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3thinjhmx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cbpcppcr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3evfogxrg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rgewxyvi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3djschtcf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3faqsohcb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3porffuuc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zwuwwztk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mjamvqla.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3howaefai.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgqdqbup.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hbdrxwjv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrpfwbma.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hmysobfz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rwjanctv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hqdzagfs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vuocubgm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fgrygpod.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bgvmohai.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylhnawli.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cbphkuzt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vqeqfvny.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xiohwbkn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywimnxxj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3llxbsrsy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zucfrfvq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3oyxqjjzo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3odtuoejl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3icssurkz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3eknqmham.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ktkqvykb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hoeurnjd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkcwjrmb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kzdxmnfh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vgagruch.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ppgdnnhq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bmwgxfjb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qkdgelha.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmjzsoz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iawvpmat.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uphebaah.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tnydxgnc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cneuvcpo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cbuuntck.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhtbqpan.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wchmpqha.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3oqrgzxym.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jsmphpjj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3blriopsc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wpdiknci.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xtolhtly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xphbwdij.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ofzttkde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzcbwuty.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3umkuyvoq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3twhahebb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qahfcmtw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lvyzbxrg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qojdzimf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zmpygxxs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3klejnjfm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3oebmeunq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kuqpilrx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3efrvjnan.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uislzoux.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jamuyhfr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nolczrke.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3symmgyjg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnemvvnn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3aizpivsk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3flaiavbb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qqzbosvh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cjberohu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uqlanxyz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ofhtprno.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ygzzslhp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nwhdjkld.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vkeimcsh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wnglzcgm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mhbuynai.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yrxvvfmz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dbyqqomj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cytrhkfy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ohyetqlg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qplvbmkm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ptbypvud.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qhfdoxbh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3eyjutnsh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qgywkxxt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3efcihrtf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3saozawje.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoqzaeyw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jrudxjfe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3duhfdenk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qbmjtxqf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sykbdvxh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3scemazsn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3echpwcbn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwwolfmu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lqhxfpny.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yqhailhf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dbquegvs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dxzqyqfn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsfngvl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rmorlfjw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xbdfqdkz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cfbecrue.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nbdagvoh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lfulyxko.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zdcjwjxg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ewhopcyh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kleiwudb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mmiagwzi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrpqyay.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3krsydiex.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gpeuzthx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3makcqrch.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hrndtrvz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gomleudg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nfypitnz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cmdwladf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vosgrqrn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cpgdjcwt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zkxjyckj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vhsmubap.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oxnbsrzw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3defqvwyf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nopftvpo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gsodfdpv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uokxsawm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rlfaxusy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3luxzvmcj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3shhoynip.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhmdxga.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zdtozvyq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pusecosa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3iknbofhc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tbalcytr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ssficddl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3uijrxgxs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3imnlkvuu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3chsnvljs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jtgsrcpp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dehacnbq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qapkwhue.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fynqbiyg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nykatkau.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vgqsjvha.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wjxtfnek.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3siwisurm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ymckyltq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jnbpbtjk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pzvwkufd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jyhytmdg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oifgopvg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ymirhcxo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3erqpjdwr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jzzuxvcx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bnlluxgc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zcspjaoj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lkaqufvq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uywueqys.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wtjfxvov.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jgcjyzhx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhlhhtya.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjbabbg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xmnupnoj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qvrtvfor.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kbwxekkp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wxjdoaca.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3opsufbcs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3glgogvxv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wmpwawcn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nqvjywag.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3arqgaojl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fjmudkze.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yobtqiiv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3agzxdewj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mmegkrnu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nvcycmoe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hjcnmnxb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fjxqvqhs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wfsylivu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3netodosg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3sezigzyr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3iqyobavy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ozzycibx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qbyzdvca.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pvluzlxf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ryulrbsw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ccxbugdy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dhnkvbqo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jytutnwo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uydtvqng.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tpxpehsh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bikibnsc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3etdzcbqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3cyeworug.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3iikkzecy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3cwsrumlo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqciig.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3frggdwlk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ljmiyjwx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3aeuxewbx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jpzwazhf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dqafxpcm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ubuhlrss.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tpwgwqnz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xldxitkg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bftguafy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wlklzkor.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hyjnlouu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rxfvsgxj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zojaodxa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wadyshkb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3acjairgf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vgwlogee.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gzzfrzdy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rvsouhyp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jpooyuji.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nswvxjla.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cpoawjan.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ffvetugz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3psazdpgl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bfwtufjg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wpxketzw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ctzvybzo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lbynlydm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fesbqqpk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vrcftqyx.html


<!-- 参考信息 -->