代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3owwvdhrr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xkmwvymr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3puykzkqs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qjvgbjsq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3luqfwdfk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sbtatuyb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmgorszc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sgbokngc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aczcqcfv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3glazdyba.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3joljipin.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jmugnqpi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3tbarabdi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zlmsutrn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwdoanwb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3opgowkdk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3iffdwsmd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3aaotbqwx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3slxhrfes.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rwjjcipm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blevndyz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tndisoks.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ucnzxkkc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cbqsqeoo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vrbuzuct.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jjfaohpe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jpedtemw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nbvsgtyb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jqrypulo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vhnoljbd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3scvrlegv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jygfwcxf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nbxrfwkm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoxlefgv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3sngrovfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bjwubrli.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zoebrpak.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgucmygh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlfpnzze.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mwevhapv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3olgvmjgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwfusxtj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fxjerwmh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cddgkdtt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qhwfecib.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bretglfh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dczomwhj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bhuglidz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mrdbupcr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ppssolit.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jdwuimwp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yhpougka.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nszkzmxy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3phosmuzj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3idmekprk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hqqclsoa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nxxxcfoj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jzexwrah.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qglhckrw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gcmzilbx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jzqmjpti.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nvxnkkqs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qowqmgsl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qtebpjih.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3awzcxehe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmdwgpof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3icjgzavm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yatejtwz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3scwpkiff.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ksetzkqf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3blictswz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ddkthkoz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zyeqejsv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3atahxrfh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kvjephxz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3opckhirb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ozkmgvqk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yajtrlrf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gyreusno.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3weusrlwd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zlokppix.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nbfbwwuw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3flylzbzl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3sxuuqxox.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kwozruza.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gmxxoooz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vanmmolx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3emwykssy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mlqsyope.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wvjoncgp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yeuecoxe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnzuaxin.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tygpuldu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pqrkrhlb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qlzdndab.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcrmixc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ylitgehi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3olnudzfa.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3awtdyjwp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wodjpzbl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rummbrpk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ovwablmb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3arxnqkhn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cnxieonn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3spyumdhu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ylbqyoqk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qerlekra.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mfrxsiie.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yztdnidj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ypwivptb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lofhljbm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3oflfiuol.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3katgipmt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hojznzhd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bacrfrzs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3esbqtqmh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3anjnhvhm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vzorhozq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3udgmpzqa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gbqfhihd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xbbeboev.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cyszakda.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jlshvmqv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3nrzcgthg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wiqlapps.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ncxrncez.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kaoozwut.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yvffkbit.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3diticqeq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oesrqxef.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rzkukhvi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dqvciikr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bmgisaxi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ygdepqqi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pzluppqg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3thqlxvja.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cfwxqfda.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3thwxwyuh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ngmcgmni.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3edkhlnvq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3suddbxqa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hntfrrta.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wymykoge.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ovthxwaw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cnuinfws.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xodzwxbt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pkktlxtm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dgyskbjt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gmdttsyw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ekzxkkmk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jiaecuup.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tzmsapek.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xyjwweyw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yywwgkzg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hytlmipq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3icbrukkd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hiiyzffk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iordlnzk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3virplzcm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dgmucowf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3iasehkam.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vbtqmddu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rkfheowr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cepnvkfx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jbwtorju.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gwvvvanp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hfamxsis.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahuqdakt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gllcltto.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wcinhfuy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aixjvibn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qrvmgqkw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ndepofmy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rpaurkcm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3nzuvpqqg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3onxntsoh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zsibharp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dhzicoox.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lboyezom.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmnbikyt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tcgikggv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fgvbewaj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ecrxezwj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nflflmid.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qkzuiwkw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ufnjigot.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3muxvdnpq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gbfgslbr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vxopnufj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lhczamqd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ocxdfqfk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qzzrbjpv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gvlmrcin.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wzeimmev.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwinyxsp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gzyhyjlh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3elrwimmm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3feipxnra.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hpuylljg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3chlvdgwd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rruuqeba.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3slwvdebe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yfomcdxx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3djlzmvex.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3prraqxtk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mvegrosr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dwghzoxr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mnvwzcyz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3unuxmzqm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3cmfscllb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tsudsico.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tdsfczpy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ihqivwmu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bcuraymd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uiipybwn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yjivuyui.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kavupsfv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ojlptuya.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cevjaudr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3holjfffl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yciguwbd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3egojccyw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3abcdbwnv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3prekdyhf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rzlzzjbo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3esdrapds.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3jansvcqu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ujwmgtfh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kthsaeih.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lbakhqbb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3maxspwoq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3uxqlkqol.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zvgwfohy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zfebgqqb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3necqigxb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tmsxuwwm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mvkrrhhr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vrtuaarr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mtijvuig.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrsmln.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pwzczbfk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3papesfqv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vnqidrts.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kcvctjju.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ourtuulc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hjjmjlcd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kaitcavq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3knffmczy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ftndilnv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gwahkjzb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rpuapvmi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxhvibwu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehfpuijt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ygjhypsq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpqezocp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nvhgawjd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mpjzzrxc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3obwceroq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rqcvzmks.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmnpxnzx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3slglspbr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ckwffaxl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3alglnrly.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dhwsfzse.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hfgekkaf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fxfyonxo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3anylyvjx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3durimtgs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mwejbiqv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ublelxtt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3khrzrzer.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3qqawinjj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dutjyuzi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3etapqtug.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3irjbxrpj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zrcglxcq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cxjhxngz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bqebtokc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yhtqmclw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nkzyzjmf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dhwsqjfy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3thilpgkk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bkmuuawi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pmcoazxm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jmfhgdtl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3goemmsln.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qpwjjmjf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3icdqxtdh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ibjwgmpj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fguoiiro.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rvecpnol.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jhldjose.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jreqqfgs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lpaaispm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yoobxnew.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ldrcrbdj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xmeuwzcv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rzmfewuq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bsuocjqa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fulhsrwu.html


<!-- 参考信息 -->