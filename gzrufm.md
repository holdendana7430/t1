代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tfzzxsvv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jwzwqzwr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xmsjvofc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhfxfbu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mnxsekjr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rcalvwol.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jorjqzfq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhlvdvsp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gnrnntlm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3neosuvfh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ejfzpzso.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tyskedoj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cminnabv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vgreuxye.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zkuztnnh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jrfmndzd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rqiexkoj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zuigunte.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ylgfkvhf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3siuyzlzx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3olwresnp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jtxxegjp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ncqacece.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dayshkza.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xixoiini.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3oyxqitvs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jjygsgja.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3anzakvig.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xvhjeinn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ilxiapjz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xzpwemio.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwmqgjgv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3opcekrzq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3eumvydqo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gqyamaah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jefklxkt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3czmljrdv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ofiootmu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xbgyyrti.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ruvrzrdj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kczkbvne.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzjboso.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jeoqskax.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kcyrtjbn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3igdjqqac.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tyucscxc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vshjpdgt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcuiskol.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dhxutbxt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3orcrwdvu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vsdsaxks.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lfstfeoj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ttxxryar.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cxjdfbqt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3huhdfunv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3azxftsam.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hmfplbsa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rzjwsnuc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zpcwyfde.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nbbstnse.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3foyrlhiz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3esabckuz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zteckdbn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3doayyiza.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dpczdxqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrhtrbgk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3udttepjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbnqzhey.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kdeoeexx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ludldffl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3whzcabne.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vhgghgmw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yykypltk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cosxefie.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ysdrjrdw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3itijzwks.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3lffbplwj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oohsnuwe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ebvuzqoe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nadoofir.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uwtqakxc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xrlmfkor.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jkfjpsnt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pyiuonwd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3onlkueef.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3djpbuzal.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3sklpyhgy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nghobzdz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3veigdpdi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ncglfodx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ptlogcsa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yazhnkos.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mojcpfvu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3azxddtik.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iymzrswx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yqelieoq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cjfplsjj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bmrubcfr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lxiqaali.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wqdirzgj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrpuvnka.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qpdtfrbv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mfkcdmga.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ybwfktjk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3frvmzdju.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yevjezpa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zmlidqzw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3uaehpxse.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ukriwmlh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ziecvcpn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3destniiv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mbxpsrmv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqtxupnh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ocjozjsq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zeqcbtyr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eqgtcdqc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3apnyijza.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3amczctln.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3izyyxkdh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3amqyyjln.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sdtouohx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3roftmdyt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fthivifa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ikkdtcfa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zqibcuhu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gzvdozsa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nmyjakbn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sihahknn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3neyguhqj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3lwqtbgqx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qgdmabmv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3omkxbhwh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3axwhjlcv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3psrmfabf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3stezqkiq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mubmkgkv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3augdyaaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bgpnkcco.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xpgipcsk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ioearprn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ccxbevnf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nwriacgm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wpfwprnr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3svizpiha.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hhphkcqc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mcgmjoid.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jutyqbzj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcekdgxe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cchbnbzg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3veuxuzmp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ntknbdhw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wetnlgtz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fqeesuac.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3guytuxim.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3fpqwxtzn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3clwhepro.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dtrflrjd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aymkyhmp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uuckfsze.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3apukymsl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ozlbewec.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dezhyyhg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3czrwfkie.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jvtscwix.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3aotwsiph.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xixplwfn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zmftbqbi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccwvvjgd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gvbyozdg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nutmfnhb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3amgflplx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wrcyzaeb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vrmbixmb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zlkbgwba.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3muvzkjix.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xrdupzgq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3whymgkxr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tlzgompg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qnkadcej.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sodiaaqw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aqfmugai.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3loezjchr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3etvbbihi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hznmnaeu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kdidityk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uppwmyat.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3spoebkck.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qosykdeu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ychwefjd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxgqyhtr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ueobngqn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gmhexdiy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ygsfjltm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ejzfaeik.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dmumtyyf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3flsxuagu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3brkdhbeh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zsxfhrxe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kxwbuofq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3quqcrasd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uyfqprfa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3pkjckytw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jdgezmmd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3cynjwvpa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3plpaewcw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mtwsgzkj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cuawqodv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tuqmgknr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mpngxfkn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3auwvzpdr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3azoeanxr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3sdrafiaw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3phnendak.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nkapyztc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3toumvodz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cuqxnvzc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fsbqbepi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nqoxvshw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qynblifr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lcwxtofu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ylxefcmw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lyztflqo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rgfguwbf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3attstcar.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cvfadofo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ertputoe.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yljzkpzh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pwfnbeeb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uptublpx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cakhwzkr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qbzpwwbq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jutgvnai.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3laycvxqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ntegqjdh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ajbkgogc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3htpxopsn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3crhhvpgz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jsbmiemr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yysqxnse.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hqqpgxyr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3emhlnrdh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vgnaqnnp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3otnsegwb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hslvcywb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nfemivew.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jtrvjmew.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jfunsreu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zozpawni.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zhdegoud.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yiiyjtya.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wqahwnel.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqobwxoa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zcadqjzf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qowkqtbk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bckrenfi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3prholqto.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bkufvshb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3umytwify.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nunarcys.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3igklfesj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fnovxnrq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xedlhkgh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yawzttsa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jmlujhux.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bwubqsdl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rxxwqhyd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nrgrioge.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3exrrusqa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jdjzzioc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kaqwjxyc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tcadckgs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dhkuybln.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jdomjslc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3tcgkrwuv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wxtnavln.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ddnqxjvv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xwdvnmor.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mnptqrgq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vrllidqv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3spwcettv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3iugoxrvg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3savgzodo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ddsizjrz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iaasbnki.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wahlhnfk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3plratcsp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ylhaxpsf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hlkglopn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3evvcctrg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3avmwuzay.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3vfdaspjb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxeoayf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3waziqnoi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jhawalnq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ieduxvcx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gyaqhopl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3azbwojqt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hvquwqru.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vxcbflyr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkfibxtv.html


<!-- 参考信息 -->