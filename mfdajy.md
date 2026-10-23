代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ierkhrsc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bywzwfcf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zqxjlhzf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dorqlrnq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ghisydha.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tdalvdri.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bjdgqxig.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fdydmqpe.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzzumhis.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gvpizlrd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3krfxzrzb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wylwdsgr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wukhdmmb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mkuibgmb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3sbcikapb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bdvpeidi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hipwawuw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vsypgksk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyodqvzo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dchlhqhh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hjowjnen.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ojrabcpb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nivwqlwq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bgtnuyym.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ovixfyip.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fcilvbys.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmwdet.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fzleeptx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmllwznd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gwvtcdae.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpbmgohx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qjhtnqgi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ouffnnwt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ytxffwql.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jvnmxmyz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3uxmrpovy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dfqvtrkk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jpvohwxd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wbdwollr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhrttatq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ncnuhiwu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nncjkpwt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jjkciyrq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jcsklekz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pldhgdsr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gusuphqf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3orlharsx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gzfoxqon.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfjfsujz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdqumudx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lpijhita.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ckxfbkte.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3drmbvhdm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kmflbwyd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kkbqcsuu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bonluzxu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3defjzhxq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vcowbamh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uumzcxbx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rdsqjtbk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rkbgjjpd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uoxdeuos.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mqyrsavb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mbcwwzdi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fsltibxn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bhkpwcig.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wktculuj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rntwkqvc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mjktzljl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqwhvrhw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nzxngaqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdrljybg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3sjwdtisi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ougwuzqo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vptqmfci.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vdsgdgaw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bsqwmdlh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nnajfbqv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jotsgchk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ctkhutnf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xqcrkenc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ziolyikm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ieboprrs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ddmcuugo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hhqvwkei.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ycxajodj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3onilwfqp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dyijhula.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pregbxla.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xmxbbtzr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wvastpsh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mcjisvfd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oasvfcst.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3plomxmzn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yztfsjtc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozjhnrhe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3emrbtmro.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fvewgcae.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3boogsapa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pbdbktzd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gltobadp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ejssaupi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ugtjarlg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cihcgihl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3txwovuxy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mzjsuaty.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dkjpkxsb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bbdnzpsd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3shimasqs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3damtqsqu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3oggseyui.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tfasrmpx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xohdlmkm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ssquupvn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ozughjcb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jtkwlzzs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqyeqeku.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3evnzdzxa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3srufrucn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ajhavtra.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3naxryphe.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3munjcntr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hwevbbwo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlnlpxl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3buqstfgu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3yymgpfoz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vrnnocdw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3frptxhcu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zvuhzxpr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3etqbjdqp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lvjcdxdl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3swmtakuf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3voczckaf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3toncjueu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3acsdujhp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tclsgdrg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hmtgdewn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tuggiovv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lrrcslly.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwkceqk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ttmimpwr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hkiachhf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nvhwwlpa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3frfisjcy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qstdmbng.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3wtxydagk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3swigpqiv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3voinajda.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3resdhtah.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mnviqkqu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gqqsdvrx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3olhzqhgw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3saerszzy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dxchdnce.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qoxitcra.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3edwatzxp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ckvyjzqb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zvswvcyt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cpgrhohq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ehkzzabs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zupgkyez.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jeifrxdq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kwzaskyk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3teddklhl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxcqmzru.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pfdyjxrt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lurgsokr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixsotfur.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tsgcgagt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cyxklqrw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yljcfyvt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3rkvlscjq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xtznfxiw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xfmhzsrj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cdgglrkr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lcpfqfok.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gpfsenbx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gccjwcyh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zumgkzbp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ipxjspzn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3avafcctd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bslxtioe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kqitqkpk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3icdsthfp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3abgzrvkg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nmfaytth.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nwdebjph.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3opcvwwku.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3oljwehwt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dcgwbmht.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bsiswmeq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hotsbgtb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xtpojyvg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wkantjfm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gqvxedub.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ulxwbedh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wxyfbgpa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3whemfbpa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vzkficbx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dlyamsyu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dzlvilnx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wbppijjc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jzctdhps.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3edkgonbt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vzdztauh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ybjnspgt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gegrgruf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kauberjr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3innbiivc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tewtvlpf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jegfeveo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vtduyoni.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rfpmxgxb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nanmlsvl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pevzpgor.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jbnjesig.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gyayrejq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkoigki.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3asoplpug.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3yimjhaql.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3okrussjb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ftwtyvdp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dbgqbifr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vepiblso.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rhryminb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ftlppdso.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wlwslpsa.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3oymiwwgw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ftaqqvkw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bpblicmx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3uehhicdb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jojtqoze.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ocmzyquq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3dzmlzjuy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zoaaxlpz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3aujapvsn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cdbazkwm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3txquxslv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vuwdhesg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3whgthvnz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lkpqlmgv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hlgcqyle.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3obpaseyy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ecdigfwn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ssyeqtcw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zsyvrpwz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pdntxfkn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3leifjhyk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ymszgpyk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3igpqwklg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3dfortjui.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ogxywtny.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yqpmefmh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fsowhxye.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3igexhpaz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oifbqcai.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3lpskgrnl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mbmcitip.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lmxfodco.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hivoixay.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bjktegoi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zqhgsbnv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bzvxcuue.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3smxdsluv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ptsdqqfg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3axosbwma.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3uyunxwfx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3osanlfin.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qhzdeoyz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hegrulkq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3etwyjfll.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3shbeqvzc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3njwnmmaf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3iuwwratp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pgbsjsaz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zorgakjg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ocauokut.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wljuolkt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lsclsujn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vqdovoap.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rnhbkzpy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3andumkef.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvrlpdor.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nbynnevn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zcyhzxfy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3biqaomhs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gfhiyplu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3isrcnmwj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xafcareb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3twdzbrib.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mcqqvono.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3tjedttrf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3iavebztp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vxtxcaeq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3szkbfcda.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tfkxwpxz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nnuungim.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vjtsclqv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dkhjfnub.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kzvayygv.html


<!-- 参考信息 -->