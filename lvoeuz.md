代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cljpsbjn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3syhmbfht.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ffxzwfyj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hehetbri.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qajsipek.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jneqadac.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zpqynfiw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ifcysavl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rabiauiw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3slipqyrg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3eplzktnv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zolpktqd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qqyeajgm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3apoakwwc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hsazjswr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3difkcbyr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fhdxnbas.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kbbnjutf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qevoagcq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gstxliph.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3evdcpdsv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3krkjxyzv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mgcpchlk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ipzmvtiv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tyqblptg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tsiiykag.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3quzrclpi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3srggpjvl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qtomqxav.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ivqqbluy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wmgwaven.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bqjjrpgj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gwkmpjvs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3workrfyv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bzvhnzsk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pzpmlqhl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uxedhybw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygymzetz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3irmknsmw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwpxayq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vkmsenbc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzdxioxf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vialxntt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3frsmvwjr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iilrrrwh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lmkisiba.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyldzsaa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wskygufg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ceszpouv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gaevslyz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3akwyuhdx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3geharxxu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eyvjjqin.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aoggfqqo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3optsnyrb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sckwezxe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3igtpvgpq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yesmfhja.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3utvvjowo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tysonadj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zaguirlc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3csiqehjp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xohvblgt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fcsvgjzt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xddzpakm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wfaeselq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oiudluvt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rdqxqzma.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dnkeqnfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yaijsvoh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jyikxqpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcdkchbf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3bpatkajj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ozuhvioz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vcjiuikz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymadblza.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3frlsvmul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lzcqfuvb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lhprpeqs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kbdjtrzt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3eazzczis.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xzjvkoie.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hxgmnpke.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pgnsanzn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ucxbjsjz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zbgbqoqz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wzjevphl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3emqczoyc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sihpsahk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjiisoi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3inaosiji.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kxvupjjx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pcjobtrs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfllyif.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mnylfdod.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3anwfkgpe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zqcaszcy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fyibxcsz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qckpczgl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mbghjenv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sfxuciqk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3anrnvzqb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3thrxfgjv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3idtmvxsf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3texjufbq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nthvvkov.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ctxrombm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zdipijae.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vkryipgl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqfcwnu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3oqyiypob.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3glkfmicw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nrziyabw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gmhupgst.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xukoymbq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zanpngra.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkzbbobx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ytokiade.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tcaocybv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eaalcigh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3cnfhbqwg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3brksifkk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xttndoiz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fqbmkscz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gqiaqetl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3gfpyeqgx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ytnntaab.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3orfgxsav.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mygizdpc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pumkazsj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wuidutvk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wfikxfgs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3egdrodvs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fzhtvmzl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3umfsyiwb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lhdgrnsv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qddomzqz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3gzaxlypg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3svhcuguj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3oyhebgub.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3roxipobu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3uijaeunf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3burlzufl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3eghkwpou.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dscdabpg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3luemkmnp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rrfqpnbk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zzekdgxy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3eadcrvpc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bjzolkrd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nsuzaokw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejfvdybc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xrqtyoin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3quiipimw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rqavlhhe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xkfjnrhe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yczkotzh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nbuglgul.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tpktcmxy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qexwxspu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3asnclfys.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xxzzgxdw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hdpszjvu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ztbdcels.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3unkxdgaz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sebvdyce.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lbtagvvi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nuismtgy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3oyapqtml.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zbnectrf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wbgpnjvr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttncxpmn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ezffzrcg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vgsaxmvv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3magurhwz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dzolfxzk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3stmmmjwr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qlgsiitg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bbmlvlfx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tjexxlxx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qvptvkoc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ildettfm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yygxwpod.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cqdozyoc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dsigijun.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tetyluoy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yknhxgfx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pkwqdvlm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yhnttvut.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cytrnirn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lfxgjfez.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mifrhdaj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qnqmvrqz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3myxrcjgu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zphuoeef.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3infyiikx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjggid.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ysyfbzdg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jndehzio.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ywujlarj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nwxmeude.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mrvumjnk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3yzhducbt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hfzuedtt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tkoroitu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dwmjmoyn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rbycnrkm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rjctfsux.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3plvckrsj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ugcfmroy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nuzsrcgh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ghqnagbw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cmnzrala.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jihoontu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pjlpaxlh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dxanfhri.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bvhixsae.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfcbvuh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3shuikerj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xlsijuqv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3puonviqn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ggitxbxt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3cbjspdif.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xuhkzxta.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xwzkhfyi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xrafuqra.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uieojmzl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3atvdltwg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3aatpkbac.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vogfnbhl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vkyytehe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3brypsghj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ddcmgxcl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tkzsjwss.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qzjfgbyc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjgkfmr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3sdzcjhpj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hwxkecir.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mipdculx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qyswsuyx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zbbyfqki.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yovbgwom.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3iyxfujdb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yunmtjaj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mpjcnrsd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ffiosmfi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zihptwmx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mvlrssmu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wuhmqeox.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qcezvhsj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3asydxowr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qpcuzdlv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dxihssdk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rszmbbrv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lgeeazki.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xshskvop.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3thlupkcf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jvlfnivc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fnkemyiw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ghoehtgf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nnikhsot.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cgpvhvxm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yecbivtc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3csrdwedn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nsnlxbfh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jpjgexfc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tsuopsth.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3fdhwjtlg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tjrspfqw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lcszbwkm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nsdyyrgr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dekmbvqt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jpdbeyff.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vaqgacwf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qensphrl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3oflornap.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tzmszvrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ffyfdccw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3spcuvomu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hafdufro.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hpseyolx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zerelkcf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttlkcuzd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ogxzkmms.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zmludatr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhwwfpl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hjltbzay.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pxqsduov.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bbwsuucr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dbdpwqxj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jqwyejyj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iylxktsa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gbgyhpya.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3weymgqto.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3arfmperd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ryrkfrem.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3uezgkker.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ochskxdq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqxeeo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kezunjya.html


<!-- 参考信息 -->