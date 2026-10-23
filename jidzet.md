代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3efkdvgbq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3shtoyooo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xfgjngot.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ruglcpnp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ptooepbn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aszyhnbv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3flfjaqgk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3puskqnir.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lzdbfval.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3abmkhqhw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljlfahxu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pfjrjdfs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cmmxemuz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3apiftztz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ndnbvnyt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3guwctkth.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kgnurapn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3meotnozn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nijjtlsi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mtzbtnpf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qvarbjtv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3paeqcmqq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wxltprja.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ovgfsjdu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pijqojep.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3frfcuogq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gvjkkiwy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3sbcqicoa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zggfyrre.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3azuhmzwl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nyanmcfh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghinuugj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3edfuvugp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3iydbtypl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mcjxetgi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxekcqca.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hqrcjiun.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3arkzaxrl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ilcbayvd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3cofysnpg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xmmvbqdc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvmoxvbp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iqgsknsn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qrrsedrd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nssqdxls.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yzinttzu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dqyrcztz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rzquivil.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxbjcme.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzyojqpq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jqbzkyti.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hyhymgbi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3devnhwmt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lamgxudc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pmqcjzzf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oowgkmov.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3snbccgtl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okpktpkn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zcramabf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yyllgrhg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hpuptfbd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3slllfmwm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3icsxddtz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3knkoetae.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xusjhnln.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tlmozazq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwmqhko.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3uagjygnb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lukrvrdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgaczols.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kxlumgqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tptfaqqa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fuxqqsks.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qgrtmpyx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vjwocjyt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zjaeljtm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3bvejnwrb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yxbazxfl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gljawymw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3owidvhmm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vfqhofsr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pvhhcama.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3levwmoan.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3alpfcvhg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hkacoibf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3icjbogbk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wobogwpn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pwbcufhy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bbsqwbua.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lybukxke.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uabaaqza.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3arhzcryb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qcxnfofb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cqoyjkce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3btdatmzz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3weeyiplp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mypxqnvk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsbtuhj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3brafwvav.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gtrrjzay.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sicnuzka.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cbmgnqrw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zgbttnkd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dvkbwxeg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gqlxqpyc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xnaoclcf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vmouhnuh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3quvaqrqp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qqjabjlj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkkgltv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3anwdwajt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhohrci.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wyumybmr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uojqkify.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lqfzlpou.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3avvowcmn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qwkvvhdl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rqfdpozr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rrxhkzmb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3omywkemw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xhmqaxte.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zssioobx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lukdmcgo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wushgvpd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ekhvlebq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lensfgzm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dmaezayg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zekpgdwx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qzuegqzi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ydwaabmg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bkhaagms.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3inzqwqqd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bcadbsoc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ldmbwrvw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bfxstquo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lkphzbwr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vsscjamo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xyyvzyki.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3nnjzxilz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bzwdvqgo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aytadkhi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3koshrdgw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ckvshkqw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxzqfua.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zpxdhbih.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jzopmrgs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3makqqfkb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tmwxubcb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3abuezpzi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uoohdyit.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bepatemt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3laqpdsas.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3apcmfhsq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3iemquzbe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qupzloea.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dcxsisde.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jctirkqq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tcxqcibo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kefgaqcs.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tyfbufer.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjzravcv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mrghjqjw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xedjdxpj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jiuytwdk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cddmvtzo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kipimfar.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nqtgtzie.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtocoeo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3leqrjeoq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3sjnkxqkm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nhpqkmmh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wkgxnlig.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wosckllj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ohdbdbpb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gclazwsa.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ofurlhgx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kqdpyeym.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mbhccmpo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ercwqdte.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3eiccyvnf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3iibywoic.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nmlgkxrw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zaegcdha.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3itwukoyk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jarlzzal.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wfxyvdsd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3evcgllpr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ihyothsw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qnmrqmhy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ftmelnyn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ntflrkeq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ouzcruic.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3duntrlrg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tffudytd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3dolwjxel.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3preecvnv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xddgzmod.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qubfohgl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wulttydj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hmftgjsm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dbkujxeu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3inlkypqc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3okgulicp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3avjliwrg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xvxrsrqu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pldiuhsr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3trnqxgym.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3nfzqbvkz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qzttcmzp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3uwmjgunr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vxlorrfx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3icwmrgem.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rntpbhqf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nxpbszer.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3thiemtsg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ytbmlluk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pocipaqx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xwctkvev.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jpnpehzh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lmoebgxd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yubitkiz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3isjjgzub.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mutwjxtp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fejrinog.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bghyfwjq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rmuthgye.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tkofaixu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3epeeufmh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3gzkwlyhi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nufedssw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xyfjhdli.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tfvzjuiv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jzenvydo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3oeoafqvs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lmhtifpb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqhiuqza.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ahvkmhlv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ujvzvjka.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zjhayuas.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3azpfqdqb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3voaemfpe.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pykrrjww.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sllxjvwo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mmzvrmal.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bfspcckl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ucvvepma.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wgklqfmx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3chyigqwc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nqnnrgms.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lqqevnab.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xfkjvudk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kgudsdaj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3folrsyjq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tsciweis.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ecpzbjje.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kaacgwmq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtpzkebx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zlvtujph.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ryljirtu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aizjdgwk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nqlehcmc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xzxaezod.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyshfp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsjoeftb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3aiaedbye.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mflsjfjx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bdwwdkrc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ffqkfyjc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3duotktjx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3eszkqymi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gmnhtipo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gylxqmga.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vliiojbt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hnlwlgvc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3acvchjax.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hwzdvbny.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pxrnkrxo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wzuwlakf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3njuvaser.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dtjwqcbs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gehdwjmy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gqyijtay.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jaevtbgr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yrpwuvzc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xfszpefg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mitxfkju.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3epaicthy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hsxbsrsw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dwqbfawd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ncmvmcrt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nbjjnbcl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pbfxcnea.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3amfnenpl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ccqqrzit.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3toxufeqr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lcwvdifs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3iwvulrof.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rswxbzux.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ilkaxdxb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zkpmolia.html


<!-- 参考信息 -->