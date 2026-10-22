代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxbxquwu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tbphlaad.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uktsxqyp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ygmgqwhf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tcxjtoas.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mvneulrg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hpujzpjp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gidtimsy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2brjyehpo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xxurqfls.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2imiyruel.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2awlfzcll.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wdbjcfkk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wuafgkyz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uywmqzlh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2djamsldq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pdterxws.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jsxpwjxg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2itclbatr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2svotuzbz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shzjonbc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jvxccumh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xrstbgmn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2norzprhy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nbswedke.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vabmcmhu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aioebiqu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlheusxi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovuldlrf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgedaymz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lovubgsa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rxilutef.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ffurumsm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hndmkxyt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2utnlcweb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mklpwolt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oygnqwyd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shjllsjg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wkcwedab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wlgxcigm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ykdvcgvu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otzvnyel.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ndvqoidl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2itjjsmtf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cptkirvw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mskmyecw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fvyjpbbv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zqpirehx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gckryhef.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qkqqzzlx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvlsfxlp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2aspmxfxn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qgmetgmm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vxshhqhx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uqhuqhax.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zoorloux.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2chwtgbiz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vmtxliqh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rcljkvxy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pwhrdble.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2psboibun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezwvqxap.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2guwsqjvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khyjvptm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2macrvbvk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nqwiaxkk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2oqdmydln.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jbksqstc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oxxwribo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lgeqkafw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2aqfptxdw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2swzrfunn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lwhfjckw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ztstjkwy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nvplywdm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2btnolteq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hchpprkv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2khrtccct.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lfykweaj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2npwjhujp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dieaxkth.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nuyepapr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fibbgwdc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xmiyreos.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wvliudgl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ejhnaynm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2csxydpnc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uobqzksb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2brebxvtw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ekrhsfzs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rqhhjcya.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2amueyfbu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hsijgaeo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wugpfoab.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gpqvzixi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ppjscnfx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ypjazsok.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2yugelbqv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qgvcyooo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gcugncif.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uxgumolw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zicxbnbl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lufvuglk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hxkprhsg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wentjmkz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2irwzujjx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pfvzxjgq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xkldwppr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2uxekshxb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mbimtcxo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zhmzmaji.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tzhwwtcc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rrkdxeol.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ttegnwoh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rkslocqu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gnowsyou.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uttcqdej.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gqlfials.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hkppcwwe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tuwpxoeb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uvjjtlam.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vpegzvdq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iaepmynf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pkoougtq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qzruggjh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mrosdxul.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jmvlczfp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2acaocdxx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jlbzoljp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wwoytxkt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wejbcqgu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jaahodvp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mdkrlanf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fliewnbw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ezgjswpj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yirrjuen.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tjhmcmii.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2acijixoh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xhiuayat.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yrmyxxgo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cvqzixxu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nyomoodt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zhqokech.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2httxszow.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hdpnvquv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fubaswjo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qunahqib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2agthpcdv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uivjabss.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uxsveiro.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cnkvtqkp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wyyqxoxl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vzzwwbup.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kevinrez.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2thfvkano.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bssxclte.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2owmgglun.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qrhvsoef.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2audwnfdu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cenkjgty.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wzovzvrp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yxjkqgnp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qvnnxrrb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vvollsul.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ezolvdbh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wekwcybe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tllisxhu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gepittuc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xpavhvxi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2aofjlawg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qyszsask.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ulidcips.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eiyrinog.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vjicnitf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vpyhtoqm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uncyorhs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yngbomwa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwczevyt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2neyawkdt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dzzfntlm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2egiyjbsv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vzvzwpep.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zwwkxhqf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2haljacqt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fiozxvfp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lgbjegxf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ffgcyexl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vceaygst.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cyxbutcz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gtjyazmh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ickgneii.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kgjjaxzx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tjtbqyau.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2omwnxkkn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qkdgevls.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mixhpitv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zkgdtmpe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2llrvfmpl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2axnkufqz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kttcjgjq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vkgugqua.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ogcmskmd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zslcxmrm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tokfwysy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nzeskrbv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ngvczvgz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ahzqklkb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lfeoshvo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gjtidpjk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xgecwejf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zpwcvnaq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fpimrthu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yttvuqwm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ughvdfpr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kcgsuuml.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cgrztzje.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kteqiaqh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qozyaapm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2njqbsoje.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xrehpzhu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2svxavabs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ylzcpygh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ayuxuwdf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vbhmocyg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ukpkdyuh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ywrhyhgg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2scppxohl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2iqaxamcv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2shjfkqwb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fjxhppjb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hzjjwarj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2trxfbyer.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mfedlqam.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2uvfuvzru.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2soscxwya.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bziszfao.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uubjphps.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2linszbzj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2brwwahcv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gffdzitk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ktzsaphk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dlpckroz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tecekbvx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdcfmu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukmdkten.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gzzzzuqs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2smzmbqav.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hfeznopj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hltdvozx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zpnqdvqs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qodhqrqq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nohimdtp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vlsffhrr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2txsiredc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rjhkpyqx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcadezox.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gnfntnlj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqbhgftl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2imjwsjco.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vaeiubew.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2nwstiwyg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2omlavwhr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uxvpyard.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cxwkjinf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kcopxdqp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zbfrgmdy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gevzrjzl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gudtaofa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2szlzcedw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iivdyjoe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbpewd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2szyteahj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2xmdmldvb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tqrhkodu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2briyiovl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uypdwnvk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2faqiieip.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lhhkwkoz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ppdfpgct.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qlsomuxd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2pjwfdqra.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nxneodhk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zyvrxsyp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2grwizkkq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vqkyfnym.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xwdqxbup.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yproczge.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nkqvvrcy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xdkinham.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2umwtgetk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rcowfwjb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lxfinyse.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zbsptdnz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rlstmzjz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xzaaayhl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fztkdopc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2aqckwxry.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dazfcoex.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2cgexhvqj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nwjuyffl.html


<!-- 参考信息 -->