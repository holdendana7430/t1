代发 wailian999

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gmlxokavk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gwuefmvfe.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gtecwmpqy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gwydjpsss.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/ggqzabtmq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/glvsdxzsv.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gnupcxvux.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gyahzcukv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/ganigsmmd.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gasjahlxq.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbkigxp.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gzwdhltey.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gpzlxrpqj.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gdgwkosof.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/ghbzohopp.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gnyfpocbi.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghfelnolg.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gdngevube.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/glvdxreiq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gfzifuopq.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/grckvhjbz.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gumbborby.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/ghnorawos.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gyrpibxnv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/galdiyvck.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gwqbnoydu.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gituzough.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gaqihpesi.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/ggqwkxabn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gflhwucem.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gnorgnlkj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gwolswmot.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gojuykykr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnhfsenbf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/geeavemtn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gjlderahq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gzzsvijlj.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gvrzyanmq.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/giaewhinr.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gsopoivjz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqywkdr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gssfcxddh.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/godmjcalp.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gfrlazsuu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfnrmvzvw.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gdtafzoqv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gljobasam.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gnbyfaklp.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gvunrjzpj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gsttnnukz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gpgwdgzjx.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gnmvpsrmr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gsjgampjb.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbvdlgziy.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gbyblxblm.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gztqytqog.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gvjlscqhs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbqalzfkp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gvinwlaoo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjjgfugvd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gcmeqncbs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gebpmktch.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gtswpwlag.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gmhmzymnd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gjrthfmnn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gxugnkdey.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/grryufspz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gkhufloqn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/geueeuonv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/ghfuuhonw.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/geqcgmgwy.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gbkzyudwr.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gjifojfcr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gbybryirg.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gtzfpxyfb.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gxyqwfnbh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gouumkdyz.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gimbuuobe.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gqzsosuzy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gfvtxgqgl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyejcocbo.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gnbkjrmzp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/ghnhbhqea.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gzrxztkzm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ggtkidenj.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gfdyqlnln.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gucbwzvtb.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/ggempwtgm.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gfxsimyjv.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gitxbgkrf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gwsveyoir.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gulrzihao.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gwqrddfpl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/glafsmycz.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gofwdkcqc.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/glvqaihnj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gmvirhbpa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gnbzpwchb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/geenejose.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gfmljahxx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/guaulfrwz.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/ghfhtjrxe.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gpdpfjgka.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gccquzday.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/geljjmxjh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gydrausvm.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gdodaunlw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gustukcou.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gjdammqec.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gmiqanpeo.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/grfldgvtp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gnxyldgvk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gmdgiklch.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gvqtuwynl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gbyztttsx.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/geewywucm.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gxvfirjyv.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/goymncvfp.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gxxmhsgou.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gjasthykv.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gsjinvdxn.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gbxrjsekc.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gblflqlmc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gdsrcdqga.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcxbgbi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gufemsudw.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqqjgyg.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/geygfxnkc.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gwhaoevzt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gdfzvtuvm.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gqckkpjxe.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gzmlrlwlh.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gzamyitbw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gnhswnrus.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gjhosxwlx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gearddncg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gvryvoqud.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/ghswzdvdi.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gwtxbpkfx.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gkufcpsbm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gukeqawrj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gjdgkjceu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gpedfmwxx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzoxfyvs.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gpvznotvr.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/geybyjwcb.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/glnypzfld.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/ghsgqzjxj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gtcjakect.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/grsgpwwdk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gshikopfx.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gruucncfp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gzwqkewmw.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gimeecxrc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gjlncpiew.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmujngopp.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gwdniocyg.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gweijuqff.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gqalpyjko.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gmlpgbmbf.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gkcdrqywo.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gcdjclwtv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gefdfyhwb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gdqprjrab.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gyvpunwyi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gjtihcojd.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gardhflog.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gsgkmeplb.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gziftjtgl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gmxfsdkmk.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/grgtuojby.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gwaesvxsc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwptjwvbs.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gjafninru.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gwcqglsnq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gbbhxfmjr.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gfhsmzwrp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gfkhsfyoe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gxfdvdfve.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gtkeebdgs.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gizwaxhjk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/guugiaeqq.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gohmneasv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/ggocpsaye.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gszaxxqpi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gaifyfmok.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gvfbxgadl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/giygeihbo.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gtounrqey.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gyriswtgq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gdelehgnn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gqjnewawf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gjclprewb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gvcomypyc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gfibetwvt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gnlixwdgq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gurzsrdkh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gmbiaqcro.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gjxkauhvl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gaaiskdje.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gjtmwrspe.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gjemffbzz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gpghcukiq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gnhqxukqp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gncymbnoe.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gdadogzpa.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/giwunqwhr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gletxiava.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/ggvuusbbx.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gzolfdwmh.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gyrnatoyh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gavdzowet.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gjwmukmvq.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gwtoawufm.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gzppurzus.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gicrvpvlt.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gvoddgbnw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/grixamfrv.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/ggfglefan.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gmilympfn.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gpndwekoh.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gbzcafadn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gykfsfnij.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gfamdjxnq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gbrzklbvc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/guiblclsb.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/ghtmmsnzg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/guhpjnijv.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gkmwqirbe.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gmrduayjp.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gjpfzntxh.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gkvykfvbh.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/grlujspdt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gamzeeyqz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gnqtsfsgf.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gcnhxzhes.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gmplaxqsu.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtxwmjzmw.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gffyroppy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gekgkzvha.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gmmxlksmb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gcqroiwpv.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gttanmyfn.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghggpkkem.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gpzynxcoh.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/ggwktqrjd.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/glctjgcok.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gnrqjmrnb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gsdtpapxk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gruhsvppg.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gvokfmycf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gfvvfufvw.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gblbbkdyi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gfjiltxqh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gmsjsjbhc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/ghijoxkhk.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gqdujblme.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gjjghtmwt.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gctrhcvob.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gsxhjcpxy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gokinihjw.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/godczzxtn.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/guixidujd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gzqucfbdn.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gjwiqaezx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gjvbykfos.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gdqczcixl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gydeaalrm.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/genhjfcta.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gpkwdzsiw.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gzqvgzvok.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gotngngop.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gfdnmhexv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/grgoffenp.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gupysptgx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gvsqgwubz.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gfnorkpzy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gkjzdbrxk.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gzctrimrg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gzoqymlgr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/godgfxhxd.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gvotgtlfu.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gsegzuysd.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gwerktzsl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gcbkiolcu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gutszdagj.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/ggbijqrwj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjqguevsk.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gxfxabtlg.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gthpwckuw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gwfczddlw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gmyduoacg.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gmruigcnh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/ggpaimsol.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gvrbvnppy.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gwtvehavl.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gfiyfosyl.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gmmwxtjvo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gmcaivbwd.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gykelqqxx.sHtML


<!-- 参考信息 -->