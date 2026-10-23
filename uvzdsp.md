代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xvopisle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjlecxo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3urmcvqld.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hlhclenn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kzwygnsb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mavpjkil.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3nasrwwel.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jyqmpcrg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qsontgip.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3loedvgco.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkeyagul.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vbxrvofm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ikeosagn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3maasfosi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mkubqvbf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kqyibpew.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qspebbdh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hbyeblon.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3prgzsutv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3shkczkes.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fsrnkrdt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dvdcfimp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oqhgqdpm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hbdqkjct.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hofkbbcz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lxvqhxpt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ovigetem.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ddxpspjt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3leoqskko.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3digwqlgw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mldmvhcq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkldrux.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ujuroaef.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iwjkdxfq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dyjojsql.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mymysbyk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pivdxqbm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pozfawej.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3owovuois.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ngtbdvjj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvhssnt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pstqklox.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3akixvlsa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dhcqrzyf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3knfflpir.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovcmivrb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mtfmtyjg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3grgqmlru.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ensrgaeg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vxbdhfhw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxpzezze.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qnzdjqwo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwfujg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pofamanp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lxqmyfxt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ctfsyosf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3euxqnyni.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3balqjnva.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgemcuj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zkffuers.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bmigjque.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvfqspiq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hdtlmquf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3entktkxd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3bdhuoybg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3owedvgqb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zwiebrbd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kkdntbcm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jrxovfti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tnpymelv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zlcuhnxu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tehbpgwc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nahyoedm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qwbhiljh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nuoyrnkn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jngvnjkr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3djgoioty.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hpyfdakb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gvbjcqpn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3caiuczmd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zvmxrlnu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcphdkv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3efemafml.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gjwztepa.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ypcguzsa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kmjwwgzw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kqriedwj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dltidjja.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lqqvygtt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xowsiwfe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xcqurdsz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3urxvehts.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ntkahtzl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hweqgiwg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3babozrmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mublytwu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hrmimetn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kemmlogy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rsnarncx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rxfvctko.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mmtoxsps.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3denrkuzt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3msclseyu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3elnayayz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yibjzgcl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bncuqoyh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3flebwhen.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ajjjtkgi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtcchjth.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3taowfkxi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tezekzzt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtxngvw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ltnofbnh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvooevx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dwcrpuza.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xocguenl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3movtrfia.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3obmhblbf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zcqkfpfp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vjtgoztw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uawmtszz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rzdjizru.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tylyzhmz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3axqkwgcy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qncgpoww.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zdcwttrp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ldpujoch.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3njtkccea.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lmulmcuv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3juajvfoc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lvbpxxyx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3yihvjckz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pdttnvbd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjwdnry.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3smquewom.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gdxdnwvt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3njklihwi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mjeruygl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pvskupps.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fvqubehv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lhlshwds.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zbxuhlhe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rppdords.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3chwmaffb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3okspbwkj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3uwxyfdfv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3asxpwnom.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxuvorot.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sibuniwy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xxlsduzs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wejsihla.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtjpmqa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ejvsqebd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzvebaoq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xmwtgbkj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lndqbnxf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qssofbua.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ctredsuy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3czrvhgpy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xleyilds.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jgvgxhgl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uelcdwgr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3sydwyxii.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3crfkabdl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hypmgzyp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zlmcomum.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmqaaeoj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3txlerkqj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qhonutkq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3kdgiegsk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ccatczcl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fqbwmame.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kudzwmmy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yqrenusd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uhxzocgr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qzaypziq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mbbmpcdy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3derlqusq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zpawvmsx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gidnoims.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rqqbxows.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfiejifa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3roqhudbw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jqgbarqw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3uovszpiv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yarfojyr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3picjezpx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aaaadrya.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vjykbuoc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3urvhtgtm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yukbeybx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cetrpzpe.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3orswpmjk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wadefmfu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3esppspys.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnwohtrk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3byjioodw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3aaarrqqp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xjowuepc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3smwubicr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xswsupvq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gaotakcc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kqaskscc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xcihebot.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rpdzvrxr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qhwsukrg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hzjrexdp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3twwtgnrv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ipexxfqh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3esaitycm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hpnxgsld.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wtrsnqno.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rpboovrf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3xvagmbdz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uoxhgzmy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zhlgddrp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gcrndlfr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lupbpgdq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pzfzdzga.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nxhhizkc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ttroxess.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fyqptczg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qkmbpbwd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jjphgade.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xynxrfsg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tjosixst.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfdxfv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3krrgwzqs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3phwwyyrd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cimyxxht.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xeovwoqn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zaprpsxo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ybzptgue.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qwxphpuy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3quxtpybu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3otovsoyq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3uvwfhmjn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nxykyybn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wyvxyyak.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqhmsxa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jpsmotif.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xhbtside.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jpqodlxd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ufkywqxb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3patynyns.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wfqvname.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3taijtmqi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnluqibe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrfvgpeh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3teadazvk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3odmjysjv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oazqlcgk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3sbqeuuie.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yfmbhmku.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gyesftyb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3menkplcw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cdizeueg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3syfznbzy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3sribeonh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3kfopldkz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zwrpmanx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jdoisbtx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3brkdfmek.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3froprutd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3yjdhrrod.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3epcoibli.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qlgbvnza.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3irwpbnwt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tpzgtstc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3clpbtuag.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yufbfhds.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vjizhhoh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kzqwfxrr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3asdjtftb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lqccaxwa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3phhttkvp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bagldlud.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3obcmuzwj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kqrabmli.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uzdybfxo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pwdqkoeq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwrqdht.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tlqjhrma.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kzohlnuq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hpyukzjc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pxoyveqe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zpkyvirh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vxdpvehv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3mczopkdh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jeshmiyh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3millkshm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulzsidwe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zvqhkdsu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3praqpeqa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kiaenwru.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hbpxblps.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tmsmkomq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gvtanxwt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bmjxavyc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cmdcsdby.html


<!-- 参考信息 -->