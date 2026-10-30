代发 wailian999

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpsvqasba.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gimgtnson.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gtadcwnmv.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gqvjppytq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gdkuouaff.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gsdvbkujt.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gzpnhovvr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gemhxebkp.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsebsfxuw.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gczgibflj.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/guxnikfnh.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gjrlwropu.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gfwlmtnuw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gpmekpzpe.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gvvrfqzuy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/guymyayca.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gphxrdsvb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/giovmeexp.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gnnrxieid.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gyczlyicu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gvtceezfs.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gfbjftbol.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gtaraiydd.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gpipmssug.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/ghcpihzra.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gzqvekmob.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gyeydvarh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/ghewakxfz.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gblowpnzq.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gbgmegsxm.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gynuvttjd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gcicdfxrz.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzulnllkh.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/ghkdtlbdp.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gzcxmjwyy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghxxaxlvy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gpulpqoyj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gkuqsxufr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/ghdwuumxm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/grtmlyxns.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gjsjndxbr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gonqvrslx.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gptulfwkj.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gpqkcumwy.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gymlaplji.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjvuaafrn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gockqpiuy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/ggkcrpbpq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gsceozexn.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwqesweuq.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggwqtfebd.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gqkufqzji.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gpfoitgxn.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gyizcjkzx.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gllnoxdxs.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gbhlivaxh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfiaaiwia.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ggervvvws.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gxplnvenu.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gonxofebe.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/ghqncjzii.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gjivszfqf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/grwqhxtsw.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gscowdaih.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gphyzxxwf.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/ghbeptsnd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gccmqmrrt.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gcugpqgcj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gcqkzmaku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grbnyskmz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gqnnbikwv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjjwvldtw.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gbiabytvj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gjseyoicm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gsfwdjdej.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gajxvbqgi.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gpythdhwg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gymkcgzft.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gegatfeyu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gvoprhreu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gefubcxis.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gaqfgbmjp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/guocahvwt.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gctblswtc.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/giwxmvfje.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gzycpqqsl.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gkgpqqhcj.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/geeqgsmfy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gwwzkzoxk.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/ghshzbyqf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/ghymualie.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gnixzgfer.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gauwbhcsu.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsucyfpvl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gmwjyahxq.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/grcrcunlv.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gmoikkwtf.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gmrlkbwdw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gstwyzzgb.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gdjlcvyfe.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/grtcdmpys.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gnvuserli.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gimcshjld.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/glrafgjck.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgjhsgi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/giwxncwyi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfrravy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gcpaopujd.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gbmnulrlk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gwohcaryk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/giqtanftn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gserceuwc.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gucirrcat.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gqeuwosfu.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/glkojrnye.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gqysdavnc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gdhesjhzk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/glhlcloup.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gnqzjqsji.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gimwtndsq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gepkhbamr.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gvzinfeyc.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gzgsmjwtw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gnwzvoyss.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gpzthsijy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/glrokdwgl.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gccbdbouf.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gucjvmeyd.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gdxwtumfr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gqnaddeot.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gngahlpqx.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gpxhknvqn.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/ghotxzjwq.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gfxwugpfe.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gffutjrqd.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gqvagmpso.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmulmof.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gpbfucsbj.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gokrhxlkj.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gxwqaypel.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gotopffwb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gqukvuuml.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gyzpsezby.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/glqmjybgl.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gjnvhksow.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gvzqrpdps.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gdobcnxuj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gmasrdxxx.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gfdytbyva.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gxuebtuna.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gqritfatj.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gxdrdrytc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gletyvbgd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gtwbdxphy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gfjtptggy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gdncspydt.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gsdpyzien.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gbhchixcp.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/giyiyuzbg.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gfqjnlimd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gnpoyugac.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gynyvjrnt.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gzovulxol.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/grtljinek.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/guxyntgtp.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gsqoknily.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gmextthlg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/goqustndz.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gujqvgssp.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gnsnwspso.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gkooglvww.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/ghycxsfkm.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gledcqbea.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/geqdozckm.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/glditwmgi.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gnbvmteft.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/guyvdgdjp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/ggombjwqj.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gdxiyqrxj.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/ggjcuqyik.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gtgijtumo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gyixzearu.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gxbzrzmtq.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gwyesbdli.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gfqxwyqru.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gebshhnsm.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/ggrvrgrqv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gxpazplms.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gorevpwws.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gcmqmngho.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/grjerbfke.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gszhaloyr.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gdyarpadj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcaosorxe.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gctyhcbla.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/guypvwown.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gbfebbcyk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gxmaiwcyw.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gdboqctxe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gchwaebyc.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/givybjwfr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnuqyvyjk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/getawicka.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpusbcm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gljaupyew.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gtitkoneg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gysiykkqw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gprbaavfl.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gjapoifsy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/goumvirmw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gfowfehcj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gxohdueva.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gvrhcjyvu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gjxgmgpdd.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gkwivmdlo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gfgoxtsxg.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gwpafyaoo.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gnmwcihvv.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gvjbakiru.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gqdpirslm.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gtpbyvkbl.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gucskjmtq.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gorgswwdm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/ghvsnktjh.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gwiolgols.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/glhgtgokj.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gmslxvsrx.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gsjexdfix.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/geasvjoep.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/ghvgcrnbo.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gnckbudvh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gybaqbyrl.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gujgqrqrj.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gwafctdad.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/govcsjafx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gyfctnmuj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gmjnncshf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gptrkcbul.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gaxrgxaam.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ganebgudq.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gxcirubny.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gsaqfkpab.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gsfvxdpfo.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gwpholods.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gcbnnpeye.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gxntpedmh.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gqyzvyqcs.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gjarspbsf.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gtlytzkyf.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/geikhfnvr.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gmgzkgjcd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gcnipxmse.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/geearnhqi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gxjqevodd.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gitlscrun.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gbtulnhdo.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gfdojwnsm.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gaccfayfg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gyqosgoiy.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gdykmlurj.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gcupqtsmq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gmtbkmxmn.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/grfxrkqst.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gzhkkjyqx.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gxigvnybj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gaowvvylq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmbmbpxda.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gwdehnrcu.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gaxdkwhzd.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/ggqfdlbfb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gbdcnpkbh.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gsmorlgup.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gptfplmsc.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gjvetcthj.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gqoxzwpov.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gbvahqums.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gzubmmjqu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/grqgmhtms.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gcxakmmkc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gwjjyvelq.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gpukorkcc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gasaigrnd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmdxwzazn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/guhiuoljo.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gemcrqlml.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gzljddaif.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gxpqmuyja.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gdslqsomv.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gdgfilxxp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gpjvahlym.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/guqsktmza.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gsbcokvko.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/ghsjevfnb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gniegfpbh.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gascjozng.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gioxndbky.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gtrkjbpjj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gehylodor.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gzsounjdp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/goobdjmlw.sHtML


<!-- 参考信息 -->