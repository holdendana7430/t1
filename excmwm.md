代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ngkbbzna.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ubjwkiqj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qonbfjgr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fqszojwd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nxluevlo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vutowzln.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wvqyjktu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3shxsczip.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lzcrhuhp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yemuiepx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gqchniag.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3alohlwyw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3umeqxlzq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qkagitmc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxbfpkzv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ldpoxttu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wzigvcnp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zoluaoku.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jqataogg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkktbtyn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zhqxjghl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyvtbqc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3atltqgre.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pizsuafj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3iswpwpvg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3scradvyk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3eobighio.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zqybzdiz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eetjxzty.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwugazex.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3twerpjot.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ypxwvffo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehxpwlzc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gydnnvjl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bqxfacsl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qfduzyav.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uzjyyunt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hbazksmm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dnylazsc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kknyldfr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kljdwaso.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nwipnyxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3sejvthwn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gnkrdoxp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bmrxxzan.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3plaowkfm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tiqzcdiu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3thucoxsz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dvgaokpl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ofgwcecx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nppabuuv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qzfpwfkd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ouubsgwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utcdbsye.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jvawbyuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfufqhsn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vwzszeyk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xsozodyp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gpkhccxg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3znqwrbcx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqsjla.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ficiwebe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ykpxujts.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qomooasx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hqceuxlw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3klbjznlv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bmcjwbmh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jfpecqrw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hrjognhd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qjqqrtpc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lmucofni.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gzqjrtyk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oapgcjcc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3muyinamb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gkxrlbcn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ruonacim.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3slfubyxx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3oquxxmiv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3umzseytq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxjoywcv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iuggwskh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jkamitys.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3jtifsjik.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vqbexsou.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wmzwxgib.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3brtexkzs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rtddyhvs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3aczdjhvw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3reaitmdx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ijfxjlbf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vcuvkhsh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3juqfepam.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zpdsvlda.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3whslixrc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ggecadsz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zhpyabny.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bpgozowe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rcurnach.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iqeidywx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fszyjfmc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3emwybxbn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mdffhpmu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tgnofctj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3opjijtoz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lcekwpud.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wznbzyer.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jjoaisbm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mzqrrhbm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zdxardxt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rspfousl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cmdrtbth.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dsburveh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3sbhomqjm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pgbtkbnp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yprlcndn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vgjpdfof.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gbwncrsl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3swmukpst.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rojalchi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lonviofa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aopsfevy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zwmpizie.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dfhinoxp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3oviweeup.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xknhqdol.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ligopgmq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xcafrtbl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3iygejylf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mncsxtbq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3baataitp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hcviydfl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hrswovpe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vtwiilpq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qqvgqbxs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yllgtkpp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lteabynm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gywluvsl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jvqwmqzh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vesmfkxs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lakfvwsl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nxbljziu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3clkqvdlr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cdqwuzgg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jpmbnsrd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pehqlodm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dpheonjk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujrsxxui.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ejnodxxa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3safngbgc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nthuomre.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3udwdpski.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvnotsjl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3plgtuxai.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pzsrunuw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dmuqidus.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cudzbwkz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ubymilua.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3owblncst.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxgoqbum.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bduljwcw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3emlerbou.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3oleyvlvy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3feiwjswh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xovbbmnq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3psgxnrdo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wkhayplz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3aozsdajo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fwjxrtsb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wegszlov.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pylbydyn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ybygpskh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mpmreamd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gzhxfqsq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mfnnqrmt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3uwlcsiwq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dmvqeydf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3morohdzb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fojenkhp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ztjzsfqn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mfuqoqil.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qymywbih.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3tvktesyf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzxbqtba.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jlnfsmra.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3odsbjdle.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrhfynhg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dxxczcbj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xubcoeup.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vebhxaii.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vdiodbua.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3blpoxyeh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zuyhkwkq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sstagved.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3looalxhx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dqbghhsq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ctovvivf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yxazttwm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lnydfnid.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dmbcvzeg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dglpussr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3opuoioxh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ngnnquvf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhlsuche.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pslwlmax.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mctuguel.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xddgfzdf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mqmpguwq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jbtyfvmk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ieflrerc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qxmvtmvn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ypyglyoo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qfroqcyj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3srtskndq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3uenllkzv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yctvhmap.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3polmucjx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cfxdlyrn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3nzkpfdkr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3uhfvredi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3chjctlan.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dkdwefng.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lukicoiw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xukqdvyk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pgbgfcgy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bolqfkpd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dklddcey.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ugvglbma.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ucvxsjvf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xokuysgx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rugzuysy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fzueknnr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3edemetsi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sjewaucu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3luspbtuz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3aurudwjr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3thepqmsq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kkuvtshm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xhczarki.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3olukkswc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wljsbaex.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzzssgug.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pdsphbdt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhzwqceu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ysbczxge.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lellxpyw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lslqcbne.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uthrhhar.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qasvckqb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jscbqmjz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fxrhlqit.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jcfrjyot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dewwjuvx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vehewjuo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qjsyjlnd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ovfbqwov.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xoszwlnz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3naokxdlv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tlotfywc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rvjwhozg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rmiesgpg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qwolnpcv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uvvwdrto.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ykgczjvl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3trfcekxx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3znischpc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vurdhwmq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rbzuyrxd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3oohaebzh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sczivmfz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bnppdyva.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3eeybdjtx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zqwwzlbo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vumglcbg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3egbsxtjw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3szjdyvzg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3iexqkikg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zfksihns.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lvfoyfgz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ogfdhjmg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ukuifypa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wgalmqbu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lirzghml.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wuiqacwq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ogksiagm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3secjxnfl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vonfhdda.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fltkytjj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zensjckp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ukccftrm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3oyukwflv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ctndapgh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kcywylsb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fodqtuzk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hgczloqb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cqtnbvkw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ggppjdzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfxocgoj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mrfiwbqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdlhllah.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xvxrghks.html


<!-- 参考信息 -->