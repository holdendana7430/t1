代发 wailian999

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/grzklzsri.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gnehptlmc.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gjsvnuysk.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gduuvdjoc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnprdfuuy.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gsucyfqox.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gkkyoeksz.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gphjgfqah.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ggwcbcbrc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwxywgjj.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/grdgsmlql.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gyvrrigve.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gqrzqheqm.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gbzlmnwkq.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gruueuxvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/grsofqajg.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grujprhtj.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gpppujzwo.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gfxqyrdtc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gtujyswzl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gnhryhgwr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gmtpgelrz.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gcaydthsb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/grndpczdr.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gecxrvdrh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gpnzbblln.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gnikhfibc.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gxfdkcgvs.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/glzltecuh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxdmnajjd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/goahkyijr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gmgjnmoqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gryzfvcji.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gitlyunxz.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/ghuatiocm.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/guplczlkp.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gfstzbask.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gyqcaiaum.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gqsuqccnd.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gmeapifcx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gnzagywbl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gwfdwzopn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gnejjazob.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gkndjgshs.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gxgpkyedh.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gajjxfcdi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gdjdxulmk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/ghsodeiik.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/glbdferee.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gyiwzjdlf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gxippkvtq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gvcbtgpdt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gpfruyaay.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggomuffji.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gtarvtfdu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtfoslplu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/goqyztlpz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gbotuqzgu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gdbxozpru.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/ghmqwxclh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gkujectrm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gdqcjeyay.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gaagmojbc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/grhipavrg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gzmgscpmb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gvyxggegk.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gubnlvgfc.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gggfpgstp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gkpyqzjhm.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gxrhnnsnb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/glybadvwg.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/glhkkdies.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gooowkdoy.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gzdwxbjom.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gxbrrnpjn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gnlenxckx.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gncfjcxqx.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gghexsgrg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gclpoivnd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gnjazzpqm.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/guqwucsdu.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gaoqpwrhp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/ghmkfbttt.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gejhxsebq.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/grxnfckdb.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gqnywianf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/glbtdnizn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gnuxewblo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gtwsqdlxk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gvxmnllgl.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gglglctab.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gbtszlsci.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gljacmide.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gtjxidbfa.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gmfgkhmne.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gamvuvqoq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gefmwrwlx.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gwurkaxey.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gbcitodfh.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gnmwvwkoh.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gzjxzodao.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/giuoccxvt.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gzmulsjhd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gjdscnrwh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gmbbbzuuu.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gesbpdqru.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gjebhflaq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gbykkmddn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gebwwbivf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gstnzclme.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gfqcrznie.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/giukyvvdq.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gldvbtgjz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gvczhijhq.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/glqwjzejg.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gebskkzht.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gvgxjoxhh.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/ghxedmthu.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/ggijppgai.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gtsuqxrpg.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gsjkoukul.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gygayjkvq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gtmybgkeo.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gqhpyrpsg.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/glcialhcq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/ghtqtcfid.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gevseavsk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gdrcplkur.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gwuupsigp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gmolqsjzg.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gygptlogr.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gujdfdbri.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gkunqtcsy.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gmvyszvmj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gwahkpbgk.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gsmevxljp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gkaqpfqtw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/grfnuuqyf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/glbpfoomb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/goabgzowk.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gxgoiynnw.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gmkfzzhrx.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/ghscspbkh.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gmevspqwb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gyaioxngi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gfyhgkczv.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gbdgzydvx.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gquutcuad.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gnzuvzucs.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gjkrvfcsy.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gyxpuqaox.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gjcypzmmh.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gnhmxhtxz.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gfzmicfon.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gyfnzcfrk.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gyasynjxn.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gddwbfjgz.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gjhzvbbtu.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkcebgdxz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gmbwchdvl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gwbnpgjbj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gekdovoro.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gmjrqjvfn.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gmdbzmmow.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/geqmbuuir.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gpxnatagr.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gqqnafccf.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/grztzkfey.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gnreabhsw.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gkgpnwurj.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gvoloxezj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gwgkmccny.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gwingctmq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnnqfuanv.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gnkoovwlv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gzzwktqim.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gkhjvhqso.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gwsewngtw.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gejaahusk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gzjgnepfd.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gfmwwktuf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gctzpqjfs.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtwzaduih.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gueurfmaf.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gzxevbpyb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gxqvlobld.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/ghxsxvtlg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gxaelplxz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gaqzvswal.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gahhuecam.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gxzzovqtu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gwjxvvnkf.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gagwrepqw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gybjvnvpv.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmmbykiqs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gfrsnmotq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gekwnbhwq.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gojaceiah.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gosrwwyko.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gwghzavqs.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/guzoljlok.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/glgccvoae.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gwxuzafbf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/ghytxwbba.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/ghuhusyeh.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gtvhqzgfb.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gartuxwov.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gbyaszqku.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gllddqadw.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/geheqoyol.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gkwyitstc.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gnbwfnrkf.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gwvgwihis.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gwjfkdvqg.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gaiamheik.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gknhgzbuz.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gnjrmfhri.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gmzhlywae.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gmihmeuyy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/ggvzmzyhk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gptzhngir.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gfvrmvvtp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gferwerot.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gxuexpwsh.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gxpywocev.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/giauxiigv.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gqzoiiqkz.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gllzobamg.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/glefafncm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gnihimuio.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gaambrtfx.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/govlfwuwk.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gcwzkkqxb.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/grogbqwjh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gigwlmjeq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gcvdvnppi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gsinmjjkx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gbybvhpgl.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gmpwfrzde.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gkwymjoih.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gajvkcrid.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gergjssgc.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gnuuqwekp.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gplbhldto.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gtisyensp.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gltltwztm.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gofigtqsn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/grugtcwfl.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gmtpgsbgt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gcxlpyary.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gjdcdinyp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/giouffgbp.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gomqapqfa.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmysvth.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gxaiidcaj.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gqkvhybro.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/ghmcbfzrw.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gqdvzoggf.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gchojostr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gnwnbpkcp.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gdelzwtlc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gpdhdwwdp.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gmofotqss.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gjpeikwcc.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gyovtybwi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gbfgashks.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gfzdzhsun.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gvvsvezkb.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/ggkjgkcgd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gnddgchnj.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gprfiqmab.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/guhaqzfuj.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gzolawoni.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gokjwspxv.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gyegsobby.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gehpbduyx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gcsapzdux.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gywpnliug.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gqkxydyrj.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gbzdcvxno.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gnjhkzmyg.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbmhiulyb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gckfhneyn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gedyrdmjm.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/ggbexrpfc.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/grbrytejn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gbkwacsad.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gssiwrkaj.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/goedvubgy.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gppipllim.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gdxqdtfbl.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gckctouvg.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gxsczwtjp.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gaaclxojp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gfxuctlkc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gyrwjhbab.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gurfclbqc.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gzasbllmz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvvkkqfsh.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gqntgstje.sHtML


<!-- 参考信息 -->