代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zkzjkfqf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3olkiguzx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3frmikyed.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3putghixb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uurpvocq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zkftvmqc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfzeeaoi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ulkeqqgz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ixvgrfhr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lurmnggj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wcvxpswb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ddfyesno.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uyymcqcz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xcdrmatd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qoxrlise.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rhiwisng.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3scufdnyv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ndbcuohi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zdmzbeya.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jvzlpasi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eqnadvjq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3puzirdue.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qryjanjb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlflduob.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlhzcnsu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uaowsskn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dlbsczfp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mpfqxoko.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cxfezwqs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdbrjcg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fmucpjll.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3exhqgaug.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mogrtgbt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wafvemsb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmsoyzpl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ktilmhif.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pdkofzmg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rmlmczqc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lhvzqpuo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ppbbidoe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rapmzpbc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nnbztlee.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xqenzdyq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tlallxfp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqmetai.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zsujlrcm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lockpurr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lyxqvbet.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wfcnyulu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kilcflgm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ilvaufgm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3behmnkxj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3swclwsli.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fyoeqmvi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lubjboky.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wxqibwbw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jfsvljlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytleraxc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jujouuwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdnpdcvw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3prjtfcmc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bqdifkll.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mmfshyrh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ckujjped.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3miyhqfly.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fzdhcrhl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3prlworex.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lzhlrzkr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xzwctrio.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xvpnwsok.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fnqdlnxi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nnwvwvcv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ozmlqwov.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3oqifhade.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3cmwtvnzt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zuexzquu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hnwiroro.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tbrnnhns.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qqqcgjhf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gylbamsu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dnmdzuzs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekcmpidk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gkowlegl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3buvkcooy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dzhuvshg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iwupcuit.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nwqehxgi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3chaxfwbq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eldgdikm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hpxgtqgb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ooorgylr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ousuiibl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gefwnmii.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dgihwjmh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jlkjwiro.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fyobqjpl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ghzbeztv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tqbvzooh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3nfrxiupo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3duyqpnaa.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sztqovev.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wfuqpxib.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zznpiegj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tbzoxcly.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zdrkhmxp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bqvqizhq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jwsuhszg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yozjqrjq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rkvzbqwy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yyxdkvgi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nyzkbgrw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jocxmkwu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mvkxmpkd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vvojrfro.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3plmvjqwj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3swajozji.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bawbzhpt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3craqwwie.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dlzhcrpo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iafhqtlo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cibescwc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nlxwoytt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ojenfxvy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ajrhjxoh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qeselhjt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3msqyqisf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hgrvbleb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kzjenehp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ppddsayn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wtlkproh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pzsatedh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fvlnqgfd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uiyxfauv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bluqviek.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wfohpxwd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kchfiqgb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vbzywtxz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qvkmxmhz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rxfdplwx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxoxwur.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ymbxbcox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3skplinns.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ztnexraw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dnhsflwa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oiyhuysc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jycwyqkr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bxorfbtv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dwzuchpy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ptcomokw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhgruotu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rfltiqaa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kfqnvuuc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcgijeka.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pkugkaqo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ogefejfg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjqiosrg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3veowzyix.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zgywwnzv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3odhwymlp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3shttqetw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pkglltpf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dcqupdvb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fjsdvwcd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lgoxgplz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wmdetzco.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3uwjlcjuy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ovmdowpk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gajkcdji.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hvfxsdfb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lczepjac.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmythpsw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oyzmbrqe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eaxrufgs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gtbkbyjp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3igkkszba.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vdfdnrto.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lcqhquao.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ohrlsqam.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zjqurhcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eqksduqq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ylvoycyc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3phbzvkcj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gxswyqcf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wfywkeln.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3cxfjyfey.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vqymykgv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dzzmfshm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vplckqaw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dehtqvea.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gafliqec.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3upoqgepm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wsbjdlgz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qfnqawlq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3sseijczt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hyemdqaa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3icwoqgkm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fnevqsaa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubupphki.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xvgyjxgy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qbtvrrrd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jjlslolz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ozfhonrf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zccmwdpr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3prniebgn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jcpumzkn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ldiegidk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zlvtkhpo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qxjnhrdn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mkdmruak.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gjuoiict.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qosrhasr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ydewytro.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vlptapoe.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3aapedyfy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qhqolupz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tjpnlgmt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jelkstkd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fydlvuca.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jchrmtcx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rvpfffyc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mwxokfnm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pdvoreth.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3okxvnlbu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3yuajoaxj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vtnzdhrj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3knyujybz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qfgoqdex.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ggsexrzk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pcmdmmjo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3boorgegh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ivleltxu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hqsgshoa.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ctkjfwjq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lbtxqfba.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ctsxuswq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mghcwkir.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bbqpzdmp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nvovofhp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qtjxpuie.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtlukqr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lxbjqeww.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3arvfsega.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rpveqkxj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhbalzkh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vujjwdsy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zvuhkeap.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lgamtazm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jatzgbxj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3amzridsw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rokrjsoj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yhkbwuki.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ffymmmdi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ktvuyndc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fkirhfom.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ebzjrvxj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3aaaumkuq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fmufdkgc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3duqvissk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ywrubgac.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nspmfjwt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3omyfiygq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ydteluiv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pijwaiik.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3enecrhyv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3prntaxss.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ttaaxjjr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tkpilfza.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sgdvkvpn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3olreyigo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3fnrejwvu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3czvqopto.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tfxkvpei.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rlyztngq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmnnwdk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ysecttzo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bvooumnm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3krpfobfj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwxnimi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mpnhgwap.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jpawdszc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3focvakll.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ylnidlwe.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kcvofkql.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ftaawrrd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3eqwkjdyo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vbvolhuv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3effdvkvl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbarzwjz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ylwmrxta.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3shnahcya.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vrdzgqgu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uldblrdd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3frsoetdw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3msaaklif.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3witzmoyq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vfsmdcse.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3umxovlpn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zgkknfsw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3okuqtkwm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3sffbtbdm.html


<!-- 参考信息 -->