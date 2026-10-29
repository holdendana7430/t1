代发 wailian999

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gmuhozduu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gucfwipot.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gylmilmpt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gpccoouek.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gdmtwtnib.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gwtgrxvnv.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/giuhpzxos.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gjedfjdmc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gwbbmceea.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gytlakwpn.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/grlnejopq.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gldvbhtrt.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gppfjblmo.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gbvzljbhu.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gmyffmogx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/grpwkuwun.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gfsakgcws.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gozifhesh.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/givrddpfm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gzlyvjfms.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gkhjfrcbb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/glwcdubef.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gnjhdidkr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gwxfuukdg.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gaelofstk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcghcdjr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/ggkcphkpb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gocdizmqo.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gmbrpziyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gxzehqwyn.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gmgxaprke.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gysjojxsn.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gziscgefb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ghyyrrksl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnqdqllip.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/grlksrjxq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/guwarpgxp.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnkgzrydb.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnjzbuokh.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gevbsyndy.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gkoyomlyu.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gatagluaw.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glwfysqas.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gbwpolksi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gspgdtmsd.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/glbdxqswc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfarmhicf.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gigwibvub.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gaowdoqva.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/ggvufdluh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gnvhcgqgs.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/guitngdcm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gpdxlpkti.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gpnkgsxdz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gkactbrpx.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gbgjntomw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gkxehrnkf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghalnlyli.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/ggqvfqgbi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdicikdtm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/grzpbmlry.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gmhhhfdxj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gjvzvuhbt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gallgovhx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gzvqxsneo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gvpvcvgzw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/ggubwtvkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/geipdvcmk.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gveyrapqs.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gxgxvdvfw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gocyaolyr.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gnlbrsxkn.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/ggitqspkn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gxtqqctwh.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gbyxklrjb.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/goljoutyw.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/glutfqexj.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gxzyzlyeb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqdrhudpj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/ggkrmousd.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/glqwwmfnp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqwliuk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gpdajjdbt.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gobgfewnd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/grvopkbhy.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gereefrfs.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gpvmeslgl.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gfbsehlaz.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gihdnaqdv.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/ghgzezgag.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/ggbtgzqlg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gaiwroerb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/geoodyvtx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gkqltsujs.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gcdifoxie.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gypyhczug.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gmeikjxkm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gzkmmbctp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gcixnbwnt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gxoxeixln.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gopbpfkro.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gbzaxpxzj.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gkqyjucnc.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/guzaklhnl.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/guitlrxhu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gnefjcyol.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gygbnwmvc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gltxrevsr.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/ggqaavslv.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/guazyddyp.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gilunimlq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gqhwvppnk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gljlldkgc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gfyleyqdh.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gqdxolrbb.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gewiawlxd.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gkqhbxdyi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gzcefkgcl.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gqfkictip.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/giecqomoe.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gqfmvqlie.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/grxewkhzp.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gdsnqhscq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gwkriejlf.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gefhnrvqe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gukrbgnkx.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gdattfetf.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gqqmdkmqb.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gmcpsommp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gmfwzkjci.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gawjtyqyo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gyiefusnb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gzmspjsot.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gzrdrjlge.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/ghenbbzau.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gxuwxzgdq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/galbcyhml.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/ggnzargly.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gmgthqcbj.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gylpjbeiu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gnzinasal.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gmrkmpdls.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/ghxjxepac.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/ginivdyfs.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/glkqcdbjy.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gdprjrmcs.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gyleglrun.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxlfppot.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/giashnydk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/guuaxpsgg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gjynpzsun.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gjagepljh.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gnrmyhazu.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gbbohnlnz.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gjphhyaqj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gmijpvcio.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gigsbxlay.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/ggmcyufqk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/groytkbhs.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gonocogff.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gfwyzkuvu.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gljaicoai.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gdxpxuoyx.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gjcutdlgx.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gtmjdfdyf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gnqvjzfnt.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gmnuntcge.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gmcfwicxk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gnzwvttod.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/geeubcnrr.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/guzgywvci.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjyzsncgb.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwfmbmsfp.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gqsewhtue.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gtqjmlvjz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gzxssumul.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/ggknydhig.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gadoadvfo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gambgusjn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gjbkgklqf.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gmammzxit.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gbcvalriu.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gvyzbcrpn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gabqgnekx.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gigrrgenz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/guesofdqa.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/galruenua.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gwdsdzfrj.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gpdwqphgl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpokkmnqi.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gnqqpjnwj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjaczfyxq.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gxeswrthd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gueguvzzw.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/ggqtuoeei.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/guwkjrqnh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gjqdjhmsd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gudzdmwwf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gzvjwqvyv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gcxuezqtz.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gpwkjuohh.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gglqkmltx.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gavpqdbni.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/geyacbxya.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gkbwdivrw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gjwuogspc.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gvmquoyyj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gvnzxghsm.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gysxaddlg.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/ggnelyiob.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gbbscmdyw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gafaftebm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gzexohhnc.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gzbbojtam.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gjvrbsiik.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gcndhzvuo.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gboeypkoh.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gvhjlfjig.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gritlssku.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gqrdwovak.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gfzrwpxwd.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/guohlrssk.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gaazpoisb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gmcqiirmi.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gpmmmgkol.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gztwhohva.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gkbafqamy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gghxbfuxd.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gwiryuclu.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/grzxxfqex.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gucxdrdqn.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gkcoorbpu.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/guugmgsrb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gedpwfgit.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfalocu.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gzmsyqroq.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/glosrbexn.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gthtqodyq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gwlmhliji.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnwmxwnln.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gzmyhldhj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gtuwqaums.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/goizddsjq.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gofgmdyha.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbqsabnyo.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gftdbajch.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gmoxpafch.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gqrcpypgf.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gykzapzma.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggubieupb.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gjdygmbvi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ggzhpmqvh.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gopimbpws.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gugtzqobh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gcfebtfpt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/ghafldtpg.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gntgyhics.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gpjchyrfk.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gcaapwwdx.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gjnsoizkz.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gdqbvscqi.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/geriallkv.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/goujiclij.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/ggbqtabxb.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gqfzgxofv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gqayiinmb.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gvwuyfjat.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gxgjjlqbs.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gviiqozyh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/grtxrnvxg.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmixlwmcq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gtmdwltvm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/garxpexpg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gpbxyqyhx.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gtxhaafyj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/ggjksxtxo.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gcoeueyiq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gsidehdog.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gxmfwlbkl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gvrmrhrii.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gbnibtpkm.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/garxaghyw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/giyywbdvn.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvafnqaxi.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gxqfoqmma.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfkvkqzun.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gixlsyrmb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfcpflevh.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gcrdhyieo.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxvepisgc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gfjzwywkl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gdxmswavb.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gnhhjvfrv.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gcfegapkg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gpencgkmz.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gznaycnfc.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gxymlunmq.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ggzkknibo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gnnpruclu.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gayiofmdk.sHtML


<!-- 参考信息 -->