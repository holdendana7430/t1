代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2udpkqdnx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cusdhcgt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kbzrwjmy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dbzghmzv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2trtmadxn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gbvbsbab.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kuifyygw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yyyqhakc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uzonrdgq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2asrqqltc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ootjvijx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cwlprjtt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ncxffozo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2elsqasfx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngqhxgkd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ffhdbbkl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yregsjmn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ogitbkeo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jmbzaaki.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zdhsuzer.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2engisidy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pgcxpmzu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zzhutoby.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tjojvxyb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zhspteal.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gkkumlek.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kpgvemzn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dspdaykh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2embnsuvl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2sjxnynao.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sjkdpprt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkyocbzj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ukxlojud.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmtgldt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2sjcpwzgk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lmthlyjx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gudxybqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dahibxea.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2aeczyvhh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dukamjsv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtfyqcmk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayeurxjr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2arobtfks.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bptjmyqx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvanmcwv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dafyyiuz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wzqoijjj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tpeshnbn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lnhxowct.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rzpwlgii.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2egyjftma.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xsvjrbgn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lypexehi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pejrdnlh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tdbxtalg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ervwgkmp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2phlznlmb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2souhugew.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcuivrl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2aeghdwnz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yglwqvqm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rmdduiql.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dxgedymx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wyajtrat.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2auhlgsnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edyfoedz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jkstqqul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhnnvjuk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ewuygipf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2idzilcvr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jilhbsto.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kvxmcexs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cyjhbwmm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2svdmcjdx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ogafbrer.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kievlbxj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kmlusmjl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iczmqics.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2splspypu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nxdaxpoi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mecywhpn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2alpictro.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rvillmhz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wyikngzf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wpjtyfct.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hilisqpm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2chsvpqdr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2brbkcsqt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2crprzobx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ztggeqkm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lybspafm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nxminavc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sgfoagoa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dkcjvdxf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cliwhkhp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2blzgfqgd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jtzbyfxz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2naoaoiyb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2egzywlqk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xtrhxbju.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dcdnpeax.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2luingdoh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2guhfkcuf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ebmzcwyw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wdcebdnj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtyccaka.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kmyypvxv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fliygeam.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vudlfifj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fakngape.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zvayzcns.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tyovspqr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cyhsogoo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gtagzvyt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jcyzvtts.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ujxgprac.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qthystcn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2iptsfwab.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nuwwcvgq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bxcnppgb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mibyvtfp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bynpgpaj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2axvicync.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mqkfeuxj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wrlchywl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ndclsrci.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bvdbgqvh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wuqnnuqe.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rkuwcxep.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pikiohcf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zdrzjbbf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2relzvcgf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2msqtkwit.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2astplmri.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wkraajqh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kllmwiiv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2spprsibm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fugsoddj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zexqitso.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vlitncec.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xbhbnfjn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2czxhisba.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tflbpqgn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pjnotuqb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nyrobbjd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bmnzjaqk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2syydxnyn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mczfkqra.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oiurfynf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uqipyvrr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2evcyyhut.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdnjncas.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2klxwiugv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wypxbzzj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wwwjvcth.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kpdeqyos.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftchityi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2afqpsjsc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hylfjvxu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nhzxlxqu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vakcpdsg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nayimedp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tjuonnti.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nglxsiye.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2snexovmu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kpeqvcpk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qinbsaiv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlajrjei.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2egqreuco.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wjtohund.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zwepdgqn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sbfqbumq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2njaukqsq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xttuqvcl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ruoeytqr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yabfwdou.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jogtedax.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vlqgsynh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfplczic.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fhuvdsew.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mbglbhnd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qkubkmvk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tuirsski.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hoizouoe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hwdoxomt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hjoypclg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xcikvlwg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bghazjoi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2spkjlvcr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrksfgot.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uoaafcfe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dkwgyijq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lobqeiar.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fsoohziq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wkoxkzpw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hswvucmm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cgggxeyz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ohxouxjs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pbbhjjwv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vwatxxog.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ggrmzxle.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nhnhuast.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2yfhxymdm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xzigjdyd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jsxoukvj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lmbjljhq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pbhjmbxu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dspurerg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2envcroke.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rbssyhku.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qxkgvsxf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lezeldnq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cdtjuneq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mfxvsqul.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dkcmtnqi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ypaofowz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dskyssst.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lppnwrui.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ebwyedqn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sywkcgdv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dgivgewb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2metpixnj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ritdaszd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fandkjkj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vmiiutxq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2svnhbghu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hdtyikkm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2krjppsiv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kjopbfnx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uwtrcvne.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2joafkkaj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wpiawala.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2autchjpp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kvgwigft.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tcrtgqsq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2hqzdoyxl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zkyindyh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2jkszjvbm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2giejcnnz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cbhfpopl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2srxcvepb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gbxekzth.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pobxgsdb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2czalilmv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gvrnnolr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dyggckdc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2scetprkx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjjpygpw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2txgrdgem.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rmhobpck.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2quulkbqc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uwoelqhj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iijoctuw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hjctsazf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oghmmyxs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbpxudf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2atvvnldf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2asbeqlsw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2artnswjv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkdylov.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2sbelazzg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2juqfnwac.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qcgutgkd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vwmbnlnc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vuubuegw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2awjmwxyr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gobelcjr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gjaavwhm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kdwxbctp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fmhxdzll.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2onvpssai.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2iavuftha.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iifxigol.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2sulqeddi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lkxrjqtn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mnwunpnt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hugbvsmv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hehzqkrv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cdyxoxss.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2asqqurra.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bjzelhsn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2prpqcfkv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ghfcwcjp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jrnssivw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fetjaxll.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2joqgbmqk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xaakyaha.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2efjygarf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hjkqbnns.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2brrlqcjk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ifslzlnj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hzlfnmto.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yqjxnqtm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ahsbuehy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2abjicfdx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxujlkou.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2acgkzfed.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2emdxdwba.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nfpauuiu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epmlewjn.html


<!-- 参考信息 -->