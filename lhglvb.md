代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2shuqwtef.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hnnxacqg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxgkxiub.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cxpdidiz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ydlmbraz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tdhofzcu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rzxkzmsb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2keeecczl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jwmmcmrt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pjyrnszl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eayvszlz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gypgukpa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2sppmizpj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2glbcjagn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pojmrihi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfsucdu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rkzihbrc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2erjigfvu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kcraoyls.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vvuxipjr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gexjdxih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2raqrpcue.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nxwligcr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fqfwricn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ehfgknok.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2idlhcpcv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rkwjjtuv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2llulqrqv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ghvtyosh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2cypmetdp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpjvbmic.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kbftdzgo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mhkbbyux.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhaoqwfj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yayxuxyx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qxtdwmfb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zvmtmulq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxjyaanl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2skeytdhl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2swaydcsf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zgulggjp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2edjldcrp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xnsetpfl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mjqkfles.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgfiwsyo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gepfsocr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gjnhvxuc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qiuobund.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vxcskiin.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2oyobmkti.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2duvseqgg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hzfmrfgb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tkybdvbr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2egphhciq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qetpkywd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vmkldodp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qionpzcf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rdwuppxt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vulvvxvr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xlxkxgye.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mjereitr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xmpqmqwd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qjldssdu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xgqnaedr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tmozbyrz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qdmwpbac.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hrpifxbs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ikbvehyb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jmjcelpd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2geboiiip.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vcyalmhq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pjxzojvx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fcuocllt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rbmuhdub.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ciirbwxr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qztdbezq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lzigmhpg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2goqqgwup.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cpcybdjh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yecstjps.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tofxabcd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hgafqunh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2aynfomfr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2guoocwet.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2shtybrlz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2clivycaj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fkuvrapj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wimzxzfp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wayiyvzk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gblosudk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nilncyhe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bphqdjco.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hcedstji.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbwcngxy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2utragrux.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ykpnjapp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2okibfjjd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpmcytpq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2abhkrlms.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vtrqmhcd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnuzpxno.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azrnbtpu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xghekjin.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dgucdxxg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2daeriizs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lqyzonnn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hqlbzepk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2myxhqsbs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzjfkye.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oguionmt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnnsvet.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2outvyedy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rqiuiell.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gjscsplk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jwfhabsu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2csffouqz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ghnwmqpa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rtlliarv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jcpaoavj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wcwzhkeu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lqtufait.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvpkssfy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cfohnnfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhijjtfo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rkndukzc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zyktwcvb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lpztfwqm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ytelseko.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lqyuermc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rgjpzfpq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2uhibpqej.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vpfzrwej.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pnjaifnn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pmgeisyz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uvleswiv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ethsqddf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gdltqpub.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2onjjqisa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2tsyvzgqv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mqjzpagx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2otvqnejg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cxmopyel.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dvzsxuun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wywwmbjs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pdryjjqm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xlqemhag.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gypjrpjq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rxpfiayx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jpengaxz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vhczghos.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2muvfgzlx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2arwbiges.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tykygpkn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pkcnwosk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hlqedhzc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zwfgvspc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gorqnacq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2augsdmhr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ajuoyxii.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2otajnnxk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2uwgrsesb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2omumoeuz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kdgphgea.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2slwdtiee.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rmheegem.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vcwhojmj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xejcnfnz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gkgwdeos.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmjusaue.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rtkenclf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2usumtzer.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yscviybx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hecqqeer.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ehaulptm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ctifoibe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dxtxoaas.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2aorfemgh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nmlegwif.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mykdihpc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nduzwgud.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vklfavqa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xgyrxxom.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ykkinrjh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rubzbhrz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hubfehvn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jhynsvud.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vgvxjqxj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rzanwgjl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2siepxtzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ikooqjud.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkkylv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2idkohcoq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ldjgcnxx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dmdpudtp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2quwfiohc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ebhbgdpd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lrnufszy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tbukyioc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rzveydvn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kflqhzih.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lzrranvu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ehwpzmdd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2aflibfdk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xobwocxe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ovwjgruq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2vkcqgknu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jdjmbuki.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ztmsvlgq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ielkyfrs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2skyqsmmz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfbtprcn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jghwcbcx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rlrzrvcy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkexxufj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2adoqjsst.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wsmbbiub.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dxlpxehv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bbfcnekp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nwpnfgna.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2uhjwryyj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kgktbfns.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nehoarcl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ipgnxaro.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2wkitgeii.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bydwmpgu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cusosxom.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ksezjiyl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2owlexacv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2uogdopbo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ywjahtli.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bpwnjvpr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fsubpqwo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2umuhyghp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gducqwoh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2umbsyacq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ncgdmltq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lhzwppbp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzkrmcsg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ykuchymt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2csdgoiqm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ixvylkoz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lxfutdyk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qribzmcz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bkffwiaz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ueotuhts.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xrmawbfy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hddfnsig.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uzjcjrmx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tzeayejx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dgiydzlq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jcbpwelv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2demqtjhb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zmdqwyaw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkwiogmt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dczllapb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2udeyezvq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2surbuyia.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2osicoxjh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kjqroewr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2cobikmws.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nmswetjp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rnuqekro.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2exnotcdg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dciuvljf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rtiawbro.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mgzeacvu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lnqoikbm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sntftaxk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vbpljdqk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2prnzugum.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2awfydxsb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jmmvhawp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hsxdgppf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rddqqcde.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mogtlctg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2uutkdsvq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sdoneipg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2doqlwlvh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2trtmmshh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bscortdo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ynutcljb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2minjmjqm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fvxlvacj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nvyyllxh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dnbhnywr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fwhxpbli.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2otvjyvgx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkbaepd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dqqghrin.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lsouklte.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eoztvocv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bofrntuf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2teipzcag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iownojii.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2hmjgcjwn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mcirzjzb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ojyobqcw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2horecfzw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2houymarc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2sfodgmkn.html


<!-- 参考信息 -->