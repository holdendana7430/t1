代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2latjbxaq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vkwlearz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gzhkggqo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jtnmatzq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2zptvxren.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2micrpbwj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2razstzxn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2njjxiyue.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ozsxisaj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xjsleawa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fikjsktq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vexcxqhy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2msqdcdnj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qvjxoqpb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2drhymtav.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yfizbnog.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jsezksqr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yustxldp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfptvtws.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aynjqoiq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xqrfmchj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2iittrqdp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqvfpmox.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ayxqqgax.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rqzidakt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iglnlhtt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dvjudvif.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xjsowetm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hxioqnef.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vsqprzfa.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2drpbccrq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rmelgqap.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nrfzzjhm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bjiukjgg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bnuhhjfb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owugpiqr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2eydjzorn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eandjhmo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vdfbmlcs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rwtrvwll.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2igopnrdb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lopmwzdo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ulsjvqmh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mmpatfdj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kynvkccc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmnxipur.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvxkzewl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2trzbnprv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wcquyilw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mierchgf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dwtpcznv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fgwqxpbc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxecwjef.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2grgcveoe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lybiytqb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gcixcrdn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kcukypcj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hryfcseb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lqtkxfpn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rparlhzw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qmgledwh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uvuaauul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2idtanojs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xqbukthh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fizpwkcr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xirvrmga.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2spkbprok.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gcbempab.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zszjkexj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtkrvwda.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ymsudwbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgozbjef.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2erfsghuq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2grqnzedf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jqxvptwj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2utepxhyd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pjwdviya.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rupeygde.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fgxheqxy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xlrkwdec.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xvpvjgqk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wghcsqtx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lcjqzymk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vuxebsul.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jgfbggli.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lkwgxmfv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tacyqfix.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dfvzuqea.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cxlsymqs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kqwbbubf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fjibloho.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tajjxnwp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2axgwuvqp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyzbanoj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pveynqxu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gidcgrss.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yccmztka.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2apwiohbk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ndzmrkce.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uuqascnx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dhafyixc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pxqbpnex.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mwoztzhq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2avuxovwt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jdzblvaz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pcomddim.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rpxyardq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmtybom.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rnbpzvww.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2htwfbsqc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2giogjwfv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2sewicowc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gyizzfds.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oifowqve.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qguljqju.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2oxejbkbi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2cevgjjdg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wygsnnlv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2oeyiaxda.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wiysilce.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qgtbavvy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfcmxms.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2svphjlym.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qvfxddso.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jvdxpevk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ljsrlmyo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pnenqwij.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gfwvfhuy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xpcsxthf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yvgbduei.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vhzahags.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pqligpsa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vdqkojpa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2makvmajl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2srivnfye.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gixqjaop.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hetjdyvi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lijeezei.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bmiczkhm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2njsqdmmi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tolemkdd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rzacvheu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yoskolbj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2utkdvaae.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bonjwhjw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xezqvvmv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2msqwjlfc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ovssdqav.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2plpxurtb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gvygrqch.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rpbqsxqy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bmzsrpal.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hrxvcvea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vxbisgqz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fbvxbhsa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2oaagerhr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fekzfvwd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2npednypl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2eqqpiqhu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cbcgvigs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmglmyae.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlnsingf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhlssmjv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mwnwovea.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qjcguuua.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zbuetufo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qlwxuqbq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pevejpgj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vgqlagjb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yagjtmsa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hojxtmlc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2faeflkit.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rhsfcnfx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jpdwsafp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwsdsars.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xssjxmxq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ckcgmeuj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2najekmxc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fwccdtyc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ngryxzwf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvtfld.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nttpuunf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2guhjlgbc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbqnbhp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fevevhbt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2oolqijbf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fusvlfkd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2osmkxlch.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qieprygs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kxnyaocf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2avdzxcyw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vjhtrjtu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dpcwcxcs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qdtvugez.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ykrcypga.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qnjgkrsv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nilocxhp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2zlwvjkdg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vmahgoba.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qcgkcrna.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nattokom.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kodrlwvd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bwrmqbbh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nclnyunb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2xwyvlkjz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2janmakmg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qbbdnkru.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bvvseark.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2sqfidxkh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ggrotqaf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yksnhlco.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2nmcbemmd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2krgoexfq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ubkhxukn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ikgzoyre.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pnvloljz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wwqphpmw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2iqptmelc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qlzhyykv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dyuaepsb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sbbnumnq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2etmjneug.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2isbvvryj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cpphbqet.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xnupddge.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mmdhfcgi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qanrvubg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2npcnybwa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2elodxhrw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2pawvimwp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ccnfzuby.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dnbmzmaq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2owxhjbwq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2awysfpea.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vkgtepzd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xlsnpzsk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vnjfmdis.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tzmhreks.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xjabtwon.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2upaqzvpc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nefuhhmk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pualyylv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2npnmuztw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jtrwkouu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wvzhkeaz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ytvgrmth.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dykitojy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2goretugc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vmyiurrk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zzasipkz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bghuabxj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rhowqawr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2arhbmbxc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gbbppfew.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fwwpzpna.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yymjxblr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2avxxiuao.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2iopsbfdz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xvfkzess.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dibyjykz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gxszweej.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2almwszwb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2fbqjefqv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwqqrnrn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zhqfawam.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tbfyesvy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lbvaendj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nqqqclmc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2aovxoxfk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2esnziaeo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aqbxwabv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2giymuejk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rdqeqafy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kgyvplgf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pjipjffw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2llbpyqtr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vcjkngnt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qgfheavj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hrkpmtgs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wqzibfiq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fupfywby.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dgjcajgg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2roufcdib.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vdjzdkqu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2itcpeyhm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ijydqtgs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2cnmiziwb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2diemdjrr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2asawiidl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zrhceoze.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vgijqhul.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xkxxirri.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pswwazsc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2funscdjy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qzonnqad.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cdyglnsq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mgqekehj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eckmumnn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hvfvehwb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ujjsuenk.html


<!-- 参考信息 -->