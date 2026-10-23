代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ilpusuqg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pnapgktd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sgdawnvr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jtdufyyt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kuvivlpl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3smlemuht.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3owrsvgpj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vgexrqxe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yozbawvh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mkdmifoz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mnvytwot.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3awzoxohd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cbpnazlk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwonmiwn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ssdngxut.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lsgtzuic.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxfovahr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3iutxxmkf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ryqkgznw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rjujlqry.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3imxjpqcc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ipqyjppq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jnlbkrlr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgyxwqe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bibpjxmk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrtsemi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gdjyheat.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vdgxhqak.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uakyfjzs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jbnxheui.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kpprnvzx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gvepzmlg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xljfwudp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lmmflqgs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qfjggkpy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ritrnpmz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ijamlzen.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wmdwsazx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zbocagjx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3aypysaot.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fifcpptq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3artyvjpb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3epcpakfx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kjprqzvw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xtvvacbi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ckawetnj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xolgckdz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azklylnm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hgrqorxy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vsfyszrk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vemefcga.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tzikxpdv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rhpuokot.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lbihckmn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lefkepra.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bpqomzrj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3swmukhih.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bxpphudq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3asmfbvbj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kqezmmgu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kymmwklz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fqlcuolq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qtcopynj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3inrbdxez.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wlpmofdh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pimbqiwk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yzdoffhc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ckxhwllh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ogjpwztb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3thrmdtcz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cmfqmznd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3otyxwwig.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fceugvtp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hlryrgap.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zrbbbaaj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3smsxmjwk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zvlbmnkl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ffeufqim.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hifqkpfu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gdjbiuee.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jificdun.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xqerziqn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cglpheok.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dwzjvpua.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3euezuppk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fxogcvrd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ctibfxgw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bquldzep.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gzcdsmej.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqxugtav.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dizibsea.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqyzpgem.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ysknegir.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3siulizkf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mddgrqfw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tzqtgquy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngkezywc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mzndzfwe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmgbzung.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kpxcytpg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpcrqry.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lrrsuuen.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ogsjvmwr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sgoyblnu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xelphitp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gyrwtypb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kxlxrrwz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3keszsjsm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzrmnsv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mgkwdajl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wucuozcj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tqgkhdqr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxvqxtn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fewgdlcz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dwpgwkhk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fekxwnti.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qecthvgr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qdpbeiia.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3enhlsuhy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ogkgvwzl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dejektxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqxqifab.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rixydfoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njrdqjno.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3flxkurhh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3azbsxqlm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dtnglgeu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ymhaeknm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tjnjkecq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gomqoydu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3inmeqjhk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3styacume.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gqqfwluk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yqpomthi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3asfjluhh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3utfxslih.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zbllnfdo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vbxmzehf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kalyfxkg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zkgnoeuj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3aneichyz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jhbdojpj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mgwabbbs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cbbdjaac.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kpolaoln.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ktpqived.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3looezxrv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ptrpvqow.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3alcjfwsc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wxyxpzmq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3drwxeihc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nndlktaf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pxtlaedx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nkcdhydq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jcdiqppq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mwrotkfa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eabqrlll.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ketslqsm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qvvgdrwz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kygodghc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ddlupido.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3foytjbbw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3psxayaua.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mdtnxvcz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3syfjwwcu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tvsmkhne.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bwtqpzcr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nkzxwwtc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yllnojzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3azlceolf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3viujzwcf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mcauwjmk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ibwvpiec.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3suzenwtw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vtugeqpm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3snvkgdjd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tyzttyhy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3thldnnjh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bstdspdn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gsvpvzqi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3igaqemoo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bawgaepc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jclqqfzs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3shvdvjen.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3daspscvr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cxbxnnee.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rnpxlivh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zfodafjq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rdputvyd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3yejfeush.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qcqdpbpu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qtkspdno.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fvsexwvj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kpmkcpqg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vtycymgp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mocgqkrl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xyzffacg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3aridotct.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3axhvxkph.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tfkjteda.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fwomnnya.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zgdiwnkq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gjjwxirp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbpozemd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gmnhfbmk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gbpxidqm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3icdozqsj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfsawxl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qxejxgkd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3cfzbxdhh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dkuyukvq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3aygdgaok.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxztabgi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jnqfpkpx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3oyulcvll.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yglndygg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hetiqqxk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3fwcolswf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3uoicdczp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lchcguba.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3swmdmbwf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uuztynyo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zgyjowiz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obffcopi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3erxkirzl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ztpgodat.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3docvnjgn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xcelsqys.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3budjrvxt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3iuwbirhw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bbixpywn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lprrhorl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3unytfabm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aiawokyv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3epyyyvty.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3omoygkaz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oooomshi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fowjqtim.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rqcfresy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uatlhyob.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhhrkwes.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fckcoxgl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bevclyrs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vndraegn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lhvutmim.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wsadjten.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ztvuxcfw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ehpgzawy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wnwhcocp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zuuazmam.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3nhkmzpmw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xrfftqes.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jbstyfiy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hhbcckud.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xuzhphzb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkxpuyk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3umdpdwyl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3roevjojx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zgcsdlog.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kezstwqf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zayuenha.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qlstlepa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xhgxljlr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3moyuqbph.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3znpyduuc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3sjwhiroa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3yztnkyok.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mdahjdnt.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uaublqyb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jnapkszf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ipfebqbg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wsmklgxa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bdkqztbr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3npjwjexc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mchjzyae.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxqmnqa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gmzfnief.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3eoeadjqy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bxyxrqra.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qeorfydb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lxhlkvmc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eezupfkp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gvbeketq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lbgjrpfp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3fjlzzkox.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jxlcmmjf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kwbolxzv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3htrvkzfc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tgtbezhj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3eqhpkxip.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gyymazff.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jfohrlpg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yogycuvi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3thtvervy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vtomuvpk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wutsaezi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wldvwpjl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3scriqsqv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jtxiadjy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hxlqtljb.html


<!-- 参考信息 -->