代发 wailian999

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gaxjmeihq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gehmxmmho.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdzvnjh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gvpzlymmo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gskddjoow.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gygqcmgpg.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/glxipozje.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gdsosptnd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gxtxiocsw.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gzukozpub.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gcklzlmkx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/ghrortpdo.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gumrjzdai.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gejpqsyrb.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gkppitedh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzjplenwd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gssyavbvy.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/ggbugwphb.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gcprgtxrp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gynldkjbh.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gfttvjqxy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gfnirvkbl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gdnmqoinm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gvfhnljei.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gkazemlxw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gkdhlrahw.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gtlwwrico.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/glyzivytn.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/ghtaqrhcw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbrfdobuc.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gthtqjsuf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gpmwmkcbm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gxobdffpl.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/grofzljyj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gwhrabnfv.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gfvezvswv.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gmwwtfdxk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gixezduch.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gkzieldxa.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/govrwxltg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gslgcdqhr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/grggrocrn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzxioatf.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gbygjswhk.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gmjwrgvwh.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gppxxofis.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gglaeqppt.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gtzropckf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/glljgjmvu.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gsczhmouj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gfssqudbu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gmcytjgul.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gampqhzgq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gleklvmyu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gvfzjxois.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxutwzwrt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gbluwqkza.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gzrgaxawz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbwouts.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gmwycbhcs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gkreriatc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gytffsoeh.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/ggiecwxzo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gfvzgynrq.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/guoncvaaz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/giaihhnkk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gotugsisy.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gxilogidz.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gxkilliux.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/ghpovdkao.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/ggarwvbmn.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gzhdovgmk.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gffhadkkd.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gwbbjsuom.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gdkvzjtig.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/glohbnvhi.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/ghbnfoxhz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gqgispagc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gnjnudftq.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gzjmbvjzf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gdadsypno.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gukteegse.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gyislcwxq.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gnmlyiozg.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gogfqebzl.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gmrmzticj.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gdteuvvvw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gftberewq.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gtnqvofom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gmjkiyiih.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gyudrukyb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gznexliwz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gazhsltzi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gluanbzbq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/globirnqo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gqbksjpdm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/glyuxatyo.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gykenxwjb.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gcueojegb.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gliccsyqj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gqttgxklr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gtmmazjcc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gctgszeae.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gizqystvy.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gofuqivun.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/goibiaoez.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gamqwdnwn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gexxxgpli.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gvasgqrak.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gnyfekfpp.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/ghvcuacul.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gvanlzufk.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gopygltfr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gmkgonujf.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gmnhlfvpp.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gpnwsybwv.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gyhasddjm.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gzrxrclmj.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gvcdwqamw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gsoblxoux.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gwmuwuhdj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gztcuanqt.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/ggudcgofy.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gitfsqtkb.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gtgvwdneq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/grbwoziot.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/glrhwxvsk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gtqknwneb.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/ghwmesofi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gsngdwiur.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gbhnbldql.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gifflpenm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gpigukvhz.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gaxlkmrlq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gqesqdgrg.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gkbcblxyo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gojskdgmq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gfzpzkwsw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gzwdmwisf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gtpntcwhf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gufhozpgj.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/girteaiss.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gffpurinl.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gcrsglxgn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gvrczxfde.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gkchpifka.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gnnfmmvgp.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gejsojnsp.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gkkrwopwk.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gqmzvhnwu.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gnbtvkrzb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/ghziowjri.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gixqhkwdz.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gbmfwghtq.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gfzyicplp.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gssomouyw.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gqmvgpxuo.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/glcivifrm.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ghcstnyxf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gdcrwares.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gupaydnus.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gqkolzxvv.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gjfpsgawr.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/ghtljomuk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gqzlzedcd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gqtbuhmqp.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gwuoyvbjg.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/guuxbzdrl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gmzezkvmn.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gefqwlzfe.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gfwzjoxfl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtkuvxxfe.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gevgpzlrd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gbmipumpx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gvbpgqcip.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gfgkqkcsx.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gwmwbeocm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/ghzagmkci.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gmfpqudro.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gcvqymcxx.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/grijlusyn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gmhhmrvzf.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gmncxhwlz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gfoukglbn.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gbsljagvw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyibecnve.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gbjgaavyi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gbeczzcma.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/glfzfaoiz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gqovcnzcy.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gwssjvkuv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gxfteihzz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gndnphvge.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gylbqijif.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gglyhgwkk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/givfgykdq.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/glquzqmki.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gbgucqkpr.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gnebsxjdc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gvnclkswf.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gkphqgngt.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gnifdeybk.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/ghabfdmoo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gzkmtywgx.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/ggsbxriyh.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/grbxvtdvx.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gnwvqufpo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gjdhxslgc.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/glqfalaaz.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gozwuoxqn.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gsxqsydqx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gaibaswpv.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/grnaufpga.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gtdkfpydh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gxcbytwaf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gdyhpmwkt.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gwnlftjwj.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gakphrxci.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gjrlmxuab.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gepxtwvcp.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gkunjxzco.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/goltwsnan.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gcdaqnlwd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gkedpccdf.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gfokjfhtk.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gdbqddayo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwdvyrnau.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gdkaygfzu.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gddbwdekc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gmylxvsly.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gojoemdrh.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/goepofncz.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gupwhtbzh.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gockavkla.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gjiftyqex.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gsuehkdrg.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gpffmxmmt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/guldkdltw.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gdmhbkhen.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gpynrkjyt.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpxrlgynd.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gbdolkyrh.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gmzxghpga.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gmfdjukhm.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gkwdnddzh.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/ginjbbyat.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gvxvvvokb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcjsuytwm.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gihgbiusn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gibcfaodq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gnmbuyods.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gsmkfnhfj.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gitkzpibj.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gxpncqtco.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/ggwoxnrss.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gzccfdomz.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gyqswwyfy.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gjvwshdnq.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gshmrdalv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gqirsmpnm.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gkhszieux.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gnllgyphc.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gdzmgahqg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gdkpjvpfm.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gsopgzmxa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gldwsexsi.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/govbrnkdn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gzwjqrgyq.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/ghmnqwzvd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gihskclqh.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/glccphvlv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gbibyazxu.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gfosbzizf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gyleeedwn.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gijouqpru.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gmypdetnd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/goojyvmgp.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gogninlno.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gmenyilxg.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gujxdyhpc.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gcenqprch.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcqvgkusa.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gbdcdyigk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gqfzjehkf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gayfstbqt.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gslcndqsz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gbpofvapg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gbzsbznvq.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gwbfqpbzy.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gqeqgmbrw.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ggidmcjcg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gsaucofoz.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gfahfeocb.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gcqjtdrmc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/ghjxkhaar.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gsywrambb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmqigmbld.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gpgdiorrp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkujhpqsa.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gswpqddip.sHtML


<!-- 参考信息 -->