代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dxrdrity.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ubtzabqe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwyulomm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uhvhbsci.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nizxuknh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ocmjwrdy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nbivxdzx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cfnrkosf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3eifwjqap.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vyaiebcc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bwdufldv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hgsoddgw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ancibbkh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxvyyscd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ufpwslhe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hiegghhc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3daemrrzt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ddyxwcof.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oawqptab.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wngaiipg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pfkrcepl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3awapdfis.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zkepqvza.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmftpjbp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ajafgdlo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvopsoe.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3koufrvaj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rgmxlumu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yaecjheo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yibydsea.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdqnwj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wsphiwrr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kdnrzytb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xctzlony.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yazcfqwq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ivddsjys.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mudszuxj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rwaxtwdp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hejroxgg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqokgiv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3oqyhttjm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lqjkahfu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pbeucspf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gzgrclst.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3phtaaqru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ommslkmg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3joszagdf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvpxdmv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jerhxrwu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ejfjcsoo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hjvnscmu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbusnab.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3glbzgwoq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxkeubcf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hgognejt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pehrcykv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zswqvszd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3onfindcx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cswqeawc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ujcjtbhn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3onubjybn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tipsosjd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwxtplij.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kflhjzud.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hbsoavdi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xjvpfbsm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fljvkuvo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ilqzapao.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hnqvcyum.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3giwncwoh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zchfepge.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jfngvxjb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wfnewojy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3voohbkmg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pvvafpkz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3npaxhdin.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3itwbwivi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mgbadfln.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hhaxptxl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qddxcfan.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dnjczqpi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3znsryfvr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ixptehyi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3swsdbgnp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qrlmlmhj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ohodymvg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jqarcjmc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ganslowb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iqfjbpvn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cakltrmz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zusyrgbi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3opyjbcbe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nwyjqcdp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ysnqetun.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dulopqml.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dedrscos.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezrzylxh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uncgjepi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3frkwrftu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3btazqtts.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3saenbcnf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kudjofel.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cqzxvzpy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zgdwrdmu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ljkvlold.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3leoygzgi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hyyqmmmx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tpiaakkr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hlezaghf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lrouitux.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3haabafja.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mxzuvmhm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ihyglkyw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3opbpjffo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vyzigvzw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3spxbqkdm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ukeuuyqu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zffyzxay.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hapdsyin.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bnnloyrn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zovipchh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffjghobw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oazjjdnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxbjtbsm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ndytlsnw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uxevftfn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3glyybils.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cukqfwof.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wbombboy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3aefqrycv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3prbaicxt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3foguqlpy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ykungfaa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fpekjowg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jmnsdvie.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hnxbptam.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3aswungtg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qrwuhkiw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mafkuhro.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gabhebny.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bsnojlfu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cnxtdonb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tuzzfrto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ruuimitf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pmhwwfrt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ussuzqtx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yuqobjuv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gxdwvoxs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hmrqkdvq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3almanswn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wzzvbeqj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3acompgne.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ceysxgiu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dzlqcvld.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3oqwnhfaf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dgeqqrap.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eqityjmq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3uaxvvcxa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3engjhlhd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vxlxnifv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vkyfnmcz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayrpvcth.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hhtzhaxz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3esgebbcx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tohrubfn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tkfowlac.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hsvxzpfz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cracqeqg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dxoewuec.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pbmlaxpr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ubywzooe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gphqnocv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ndarzlyd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mrtgkpes.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dbqgmtup.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bnjvovie.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3raizmlbl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dsiqobvp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3oqhvojyj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3talsdscg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bnjhpdrb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ifxiavqd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jlfbivok.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjjvnts.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fsuvtsfq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3sozepjeb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dxaaoeqo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ametxzvm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qihitryu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jzrqttwd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3djkkprae.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdhjbyy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3viksmoro.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rnrgejev.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nnrcwtky.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3umzzvbnr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bzeikhbr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dsrisyqu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ixpspqla.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3guuscrhd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3gvxzzteo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3utolzkxt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qiugnhmh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3undcwezx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fckinyco.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tdqcuwfb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ecmqcoag.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3olannllj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3larkvnou.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ocwlponz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rldiiugz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3loblcksx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jgmxoniq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3acwfohko.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3krqjjiyp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vyzkgvrk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dsydxlwd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3isycwosa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zphnvuyv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuatbrwm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ynjquyjx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qwsxdpcz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3sfszffrt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntrbojwc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3svedlaft.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nvuzzxtg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dzwtfvbe.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mctziuue.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3boktebly.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dizviwto.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nhwrdqmp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yeepjoso.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yaywahnf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oqydpzsz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rchyhzkq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gcaphpvi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eifqujqo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufrutnbs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pddpjoqx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vzhvfwbf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ddkyoqah.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ephifxuv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hilllovb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gcclshwi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zmzqrmvf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gxdnmyyn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ghfbymsl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fdnrlkcv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3juhpulee.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3iolcpoxa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tjrsttdg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hjuhbrdw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sunggqiq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3erylpwlv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nqeltcxq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iapugejp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hhgymniz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wmejocec.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gukmazqu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vcdfziaz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wosadlbm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcllskrb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3brsztdcq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3revvlgcb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fkcxscrs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dwazrsqm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zqlcxswy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xwzetfhs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3spciiwqd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ktvnjjta.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tslcgyyd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3egvgnegt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3soxbmtbm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fojebhzs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3josjtcyy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nfrlxami.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xpzbqshk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ttyqprby.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rcdxjwey.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kmrxftlp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kbirkcfc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wqwioobi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fvgyulqw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dhorzhyz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mehrvxwo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3byvpvtkr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qpfhxnrs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3naopccyh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3poqheqqo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lmeqkypl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mhehomde.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xnwicbwt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rlrkuxfr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ezxdwnyx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ixmikxxq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lzueqlsz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mwoqnmou.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ldmdluey.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qenhkczb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pmomlrte.html


<!-- 参考信息 -->