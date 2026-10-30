代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gsxhanuxs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gqyefeejy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gwyuxnupi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gyylhqtaw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gdeerdcce.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gudztfehr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gzndwlqhw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/ghzxhuwuc.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gxhquhjzv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gtvroimkc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gxvywvixf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gijgzhlwu.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gjztbrtpn.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gviwzatya.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gotvhuyho.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gzpalplkb.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gcqlnbskq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gepnrinam.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdvconfrs.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gpdbiunqp.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gtmrkwjfh.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/goyrepfqh.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyfzqnezm.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/glefnqwmu.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gaoxymdhv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gviznhyxs.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gvxtvofxe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gnyeqbbai.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/ghrdsihlz.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gnjmbyixg.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/ggaittzqx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gngrsgksq.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gftxggjwu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gfesuqbld.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gagvntwzb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gzbhpvreu.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gridxmqgf.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gxcxjdyif.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gjtbktagy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gikhdwbyj.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/grshopiik.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gaktddwrq.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gdrvixaaw.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gyunpbbeq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gynlyvwbb.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gfxmbzqyb.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/grrrehjuz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gffjggzhq.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyjkjdzjf.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grwtxrclq.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gyarfrpvf.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gzzafppfw.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/goryjrawj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gydhnqpjt.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gthfakzdp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gnhnzwkcm.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/ghulykpol.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gkpzjgbzf.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gkdqwsfhb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwgjaqk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/grkykipsu.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gvxkuzdqx.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gawigknbk.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gwmnvvkhr.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ggiqkcaad.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gfgewijxr.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gtkcdqfif.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gpsertobv.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpappbmiz.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gfzogcigk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gbrctxjhb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gwtcdwhwq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gjajvumzo.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gcvqumgrd.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gaxfhozqz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/goqlrmvbc.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gdexolctn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmnvyphi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gkjfrorju.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/geeghknje.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/ghwubzmuk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gqwkmcawa.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/ggcfccemy.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gozprabls.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/glcqqajyo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gpbwxsrjy.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjwkwoi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gepgdmmzt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/govqgcaxs.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzhtnytwb.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gbwvdwkpj.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gqpmvgasa.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gsonihiyn.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gqvccxnev.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gifyolbmk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/ghxlcfclt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gvlzifxdd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gtyacpzcs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gafrnxcqp.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gdacyoczw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpsnrxqj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gwthkycgl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gponjxlry.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gxnblgbdi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gfppguvii.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gfclsapwc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gxhubbeba.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gvpkwihca.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/ghcbzrzpa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gczsvedke.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gfckpnlip.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmxjcblhe.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gtjmjtwsk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gnptzhxzi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/garxikqfn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gnhytnhqm.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gewvhglix.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gtanptcun.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gtcpbsxyq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/ggwlqjqmb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gcijyhyya.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gefmejuci.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/ghqcmmmpn.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/glfurctpj.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gpmvpdvxm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/grtotyqir.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gvkfterrm.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gavkatsxl.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/glzqmfwlc.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gdayugfqr.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gcstpanxg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gthwzsdcn.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gopwbhnyf.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gtblxqqpl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/giydenbpt.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gicoqevfz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gswzskmyj.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gwcjckcmu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gbpqwejab.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gldubqqsq.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gphvubend.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gpaexprzt.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gqqturdbl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gsassurjg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gmugiowmt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gixquutmj.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gxpnnecvi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gudsyakum.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gpluhddmc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gvgewmqwy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gviktpebf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gadjwxpro.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gifwgpoxa.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gcxboxnoq.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gajzgyrej.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gklxggtuq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gqfxbmxvw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyarohm.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/glmgasylf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gfqyklfne.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gdtckersd.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gyqhmveip.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gbjyfklhm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gtywkvevz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gbtoljemn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gjbwfqygg.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/girrcvcqs.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/goxzfbxjw.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gtmvmvnqo.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gmpgxogcb.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gnhiiotew.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gncwsrwjg.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/grtyaksdr.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gnczxtjoy.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdzjbzylc.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gdborbkvi.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/ggmxkbpxv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gdzxfosqg.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gkgfaaxwk.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gkxeyoclu.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/grfgbaoze.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gwmzsduit.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gmnkwneas.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gnpagojop.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gvfnbkgpz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ghpcccdth.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gyekazmhx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gpyodltaq.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gddsysiql.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gqpjtimgt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gbusrahia.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gsdivgkmm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gpxdvtzgm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gnmfiaovs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gcqftfmis.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/giklvemwe.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gsxaqkhos.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gxsinjbla.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gepzegbua.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gnifibpeb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gydzoblmr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/guqpfcago.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gecajqsxn.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gediiwsiu.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/grtcwljfk.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/geqvpffbq.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/govnyoxcp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gqosgtvem.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/ggjytpbjv.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gqfbvoknk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gkfathcxm.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gyfiklvmv.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gfmfcuymu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqqquyon.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gdxmrnrnc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gdxgdggxd.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gkrkkmkas.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gmmukvysv.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/ggekqvnod.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/ggijgywfm.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gftuqfdfx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gmnileybd.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gfwnyupfa.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/grwpdfyif.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gflyrneox.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/goramaztz.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gmxykacxv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gjbtsuhfh.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gskmuzjed.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gkdwsevqn.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gimqcwftv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/govbbhyhi.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gxefroiub.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/grpfplzaf.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/geyadgtqs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gvxwxrtpi.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gqgjjenjg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gjacnfvqf.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gcvgavzvv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/grarpqayk.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gvagckusr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkbwliaov.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gycsitchs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqvowuna.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gqelmkqqn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gcgyuzcgq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/ggipyaytf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gcemfhjcy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gxvdqypzy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gwkqryypr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gmhvcmtim.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gdgcjvdmw.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gwxqbtmae.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gvoyryihf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gckzamnma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gqqjcottm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gutcyjmkn.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gczukvxmq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/goffihane.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gkdesuqqf.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gqljnpssj.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/geenzmtbu.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gccptgzli.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gbcjgdewn.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gybpesrme.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gnuiafcbb.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gstcoutha.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/grvatpsga.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gjrwxdfut.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gphnapmsk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gdocuojnj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gvyeizaov.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/ggjfscgts.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/glyqxbeqp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gzugvcecg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gufftyqzl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/ghnahldwi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gmihymvxe.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gjpntkgai.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gxkpdrrou.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/glqtpjmls.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gajstbmtx.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gqdxddowj.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gepqbgejw.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gvgkawtxa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gbiqflfmb.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gkptmunzj.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gxoevjeyd.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxpkejkhq.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gmisjriik.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gaygehlbi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gyijovjip.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gszsshbgd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gpwhrmfze.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gzvaoegkd.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ghynldahj.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gyoozgqzh.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gwysuwarz.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gzkypazuo.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gjerkzfwb.sHtML


<!-- 参考信息 -->