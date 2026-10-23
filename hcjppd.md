代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zlgaxdnt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wlcnxdxo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3frfrzdve.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ivtktcxh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3isebieln.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vgohznwo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vftfgtjj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ufoeuqya.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3aquzluyv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dajhvhpg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bljkwnxh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yaqwoojx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pvnivzng.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lwgjuejv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gqtxuiwv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzklclyd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lhjooxep.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3umdyrmej.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ndmuxfry.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uajvwfro.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dvzfhtxs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jdtiravz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yuunedyz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vjftsgjr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ikeukqhj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cgjsvttk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3baisssua.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3skbhrhcp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iqcimsyh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qjnkpwud.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bmxijpkx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sxektpfm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3idnwlyxa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vywpulvk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uzfimxsm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bxxgqiej.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmkkamay.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxakyrl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bjdwoxcl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ruhodwyg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3zgdjcvmn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3eegmaybm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gqdpalaf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dmvlafjt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3djvjxems.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkgards.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uylxgtdx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3azgfgwty.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qlcmyplf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cqvfgnyw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hewtlpmp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fssivpyc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hzboafnu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qspzzjjc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nxfqpzeu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3iqbxdhuu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iegjlqsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3swxfuonw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rcrowbtr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uvhulwyx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yhpezbdt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nelqrjqf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhyxtsbe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qxsbwtch.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qrsrhgnr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fctnxpzy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dfdqtmpg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ogtsiezy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gpbrclrn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gmdlhtjz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vjnchecf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jycwoqsz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ydxezrqa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ggrilhwz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ypoihvtc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3culjcljk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kzwbmsgs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mrtxrftu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nmchyzch.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jcryatna.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lucdmjuz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xquafjuq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yztqnkwp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3afmeowzf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tewjqojl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3shnyarqi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlkeomoo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lockmuea.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kclzrssh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxmedgxd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3edppagaz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gtvepndx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pkhepqqs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ncbckgxj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nawfyvix.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ktacddgy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pcqiaxwi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3daxqteyv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lxlsezsu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gtgcmhti.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qxgqobvi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlrewatf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmzppvob.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3diukxrey.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3smvsrhun.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ktzgrcse.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3edpzjmid.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lifwhyby.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mgpfbwnw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oivcfxuu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dktylwgx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ldszgavk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gvyzvqlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rytgyfjc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rsoessln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqhxfeyh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jccorwgi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zugsxzaj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bvaqegnl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tkdttjvk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pnhvlodj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fjakycpw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tznbbyzz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qrtbfagf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3expxwguc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3usorjsez.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ziibrbww.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jyagpocc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3thbxemzl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kvthurjj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bwlygfqp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3oywfaukw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3oknxdhev.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gdwtrlok.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3oizryivy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xxqzztwj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3viyehlnd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3chxvrilo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tmkzkznj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zedtznam.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cgysanpr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vunsrobe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bqxapuhd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hjdgoqhx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dkvnnelv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3diesqkra.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aqvjdasb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jeiabypm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gmupwwgh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hsthzmij.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tyuotnwm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yviaruqd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hyxgvygs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgsujfn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rrvouxtv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3itkjgzgy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ufhkagmf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3azthclfr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dggggddq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xgvhfioo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kcdbktbi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ffscwjgx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ftxqsorb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uvpyonmk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ljoozlvj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vbuuksfz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qgakcifz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gifxzdjx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qirmszcb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wnrwmuad.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yzubjbab.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3runmcjth.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3veiutxto.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lvanswlq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xqnglyen.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pppuglae.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kstlftnc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wjlfeziy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vscekmok.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sftwvbgb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mytrzbti.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hmualzhs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wmzssebm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wvimcjzm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3liczspgn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wvjtlqbn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cllpiovv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uryhqdom.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ztyequwb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3crwkfmfu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cxxlymhc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jkvkbhyj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3oquaoqhy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kabypvso.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ztgdivjz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwtsmtr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wquclxjb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3iljeixnl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3sbnkratk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pelptywr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cotqainl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qkbptdyz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uxdecmum.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zejgxale.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hezhtfmh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kayatigr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3shvxjkxf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mbdvslwc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xsrffwfd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tmoxtoll.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jrwvlczq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqbxnrhx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3yieqbany.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fquwunez.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tlabszvo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nhuhvjjj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ttymdwbl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nidxbdpf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jvyjzuyd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uvslpiul.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hojwdpce.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gxwywirw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3llcxmzky.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3kneackdj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fqbovhna.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qzitdgpf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3opfyyvld.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xxajkuzv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ywtgtvaj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wxlmhqlx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3haqlvrum.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dgvfaoyx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dglrtcjq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3taxbqaym.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3forjjvki.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dmnhkgpu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gpkimdfp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgrasaab.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xuvytiuj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tbzjvrfw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ixcilpes.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3kaseslgy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3izeamjbh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wftsgekb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cdoxxemx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pkvpqmrm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dctptqct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nlvjrbgd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3iqbzlzku.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3chzkyslt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ssbmldea.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dmuwoxvx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3dvycnyve.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ylrtwsij.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3azpyrmrx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mlydlkgi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gxzukhdj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tdvrjpcn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jtaqorpz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xfjhxjwo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pdptqqth.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nmzfqotb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3elphkwvp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3smxhjoet.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vrfqfvxx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3uhzazhtj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lweihqeu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mqdlsogp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3egwgagiw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zrfdmofk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3sfnqxpuh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bqvwdcvm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cgsgpzyy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eibbmrwm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3reutzlph.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qygbwhxj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3unrkzxzl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zualtydc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fstbjosb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3crlwxhte.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3imkuhbec.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mupggppw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3emodcedl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3trdeflmp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fuzlnjdz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3nhoohwnp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lvgtfouv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kpsxomib.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uqnudyzb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vrskoxyn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jejtgkfn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3eogqyrnp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gwxlkmsi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ognbtlph.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3azwyotji.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3abcxphdp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ksmqffqh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fptoybzm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oaezhxpz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jryokwzg.html


<!-- 参考信息 -->