代发 wailian999

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gdqjxtzai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gdjyiboig.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gvbibhldt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gwtxkkuee.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gwihkufoo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gomlurlsh.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gxaarlbdc.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gidyldhwr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gwgdtfuro.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gmcttxiie.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/glcggdhns.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/glcdrjgzz.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gdxjgtlgk.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gbrrunhas.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gtetogtvv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gpvwxsnkk.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwfhjysvy.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gdewxaqro.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gorcmzzmx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhwibha.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ghzuldxyo.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gruzccshz.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gytlzjcdb.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/ggyonwimm.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gsjgahria.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gxkszjehu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvonidqid.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvhgbvhro.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/giypfquqn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gspjpbnkm.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/geudrtruw.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/girbtrrce.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/ghokhftre.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gfkfscogb.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gtsgmemam.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gbujorbzl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gmjvdkeor.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gyddirjeb.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gbvmxiwac.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gdbklnnbb.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gbixkqdnu.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gpgdheore.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/grxcxklep.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gtixlyygq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gannjhgqg.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gebkqffkl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/glvtzlqkh.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/ggdwwpnkr.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gaskvfhyx.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gqctxrzwv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gdgztlvnt.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/glbgvondk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gmfrqxqbi.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gzwttzsik.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grhtmgsnm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gelbarhlg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gtqnxpdyp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggypmxerl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/guemzjxmc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gigdrrlfm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/grgtwqeei.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/guaglvitu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gwivrsmpf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gawsckaur.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/giwehylny.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gbmwhhucm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gjevuageh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gmyuxovxm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gdnnxmnot.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gebiubelp.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gopyvjwin.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gkagwafpe.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gykasvzau.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gnpvglmdd.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gzdqxseys.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gqnnsrmlk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gjwpdhefg.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/ggxestxmu.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gbghalxal.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gyvpjmanu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/geytpamlp.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gvcmemegx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gjpeduwyc.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gxuiybmxy.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gsyaskdhv.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gzuxrgwho.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gjwjdlhtx.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gbmxzzrcl.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gyrqxcqdp.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gvhgylxwd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/ggdbqrfzb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gvbsldadj.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gvwvzznka.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gbjlsaytb.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gpycnitgn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gfhoevwnp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gpsdkuper.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gbbkeqzyf.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gdizvktxz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gnefsgjhm.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gosopymnp.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gqmwuihrg.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/geiqhxljg.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/grjnjodfk.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gthzofwxh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gftgvhzpw.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gulaclfkg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gcowkmguv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gqiyaiynh.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gfpvpxtci.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gzrnzatsd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gygdxacvv.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gyjsiiddj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gwxctvvsl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/ghmekpgpt.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gavoazvyy.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gufdaraub.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gfdiedfgy.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gcpooaidf.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gqpvkxrlo.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gywzdvhmw.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gfhdtioff.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gcibrsutr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gbjndssfb.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/ghpusxvid.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gvjjagngn.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gahlkhybt.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/ghporwqly.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gjwiwtyoe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gvvvvotry.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gbtepzcua.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/grhlvgjqi.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gpnryadtq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gkthhefqw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gbtiygbtz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gpfsvrmrh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/grkcoqfvu.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gllkmbvkz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/galxnmdqh.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gmxidhlwt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gmlkpllli.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gcsimvjli.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gshkdvlna.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gtduvgjhf.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gpfpulsvv.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gfyliklbn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gfrixfyom.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gxezgwsbi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gbsiqvdpp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/giwvenstp.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/guonjuznl.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gcemrxaos.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gohizpmvb.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gsqklleha.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gvufvhhbc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gbtlkljgq.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gmeknmwfo.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gaeobcvpg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gtvrgkcco.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gxkhbbntw.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/ggpscpxrn.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gvjvizkfe.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gftfavxku.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gvxyhjuli.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gpxspflye.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gqfxtgnff.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gnivhxfph.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gjpslxidy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/ghdujogbt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gttcayrne.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gjvrjxgnv.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gzbgrupmw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdbuozslw.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/glmetygbo.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gszqynkac.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/giibnrogk.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gheepojgk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gwatjqqsq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gjuywjdxm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gqjgslfvc.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/ggxejpied.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxylmrvou.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gawtyeadm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gffgpdkxn.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gkqwhhiii.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gbtqctrmk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfmgtklgm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gnafodbbz.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gvyknzhrp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gqgecxtsh.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/ggtxnulvc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gyybttxkb.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gqfxncqin.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/grsoajdja.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gytgemwtz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gnannosgf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfpxtyugb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gsrmfeodv.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/goqtcqkhz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gumvzowkd.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gdntsfnys.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gmhxoixeb.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gblzeymwy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gohcpsdws.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/ghvrkqqog.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gytbkxdkb.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gnrzbwryd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gxsysdgyx.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gmkuaajqo.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gpmmwssjn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gmgtuhuwl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gmbanxumk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gzpqieneu.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gpnawuszd.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gvdzyjbxa.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/greluqkaw.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbpdwdx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gphqzsqdr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gciuudptn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gswcmfyvi.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gpxuiocyt.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gurcshdbp.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gaazzehru.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gdpwsmkft.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gntsyhmfy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gscpppixz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gvxaxgkxy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gcyqlchsj.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gapwnjkre.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gogtxdobz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gcixxdpfg.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/giczqqzxp.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gutpubvfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/grjyausot.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gfttalfey.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gogjxhlip.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gtlxdpcur.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ghmwoqusz.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gzalhzqkq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gycffxdyr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gbcgyvqov.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gdvsldnht.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjfomjvii.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/ggagcuffm.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gruucsoty.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gpmuyvrqo.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gonpztnfw.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/geukyphnv.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gflrkojug.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gutprnwam.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gmfjihdyp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ggffqhttb.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gjqeqzmya.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gndteyzwl.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gtrapaeqi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gwrtqptxf.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/ghqbhgzcv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/goemackli.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gpdtbwhxe.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gtaydruaj.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/glbwtaaqa.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gsewooamy.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gglzqzjqi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gcadawkgw.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/glpcokrpe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gohqwrinu.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/glvnqtbet.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gchzsxnit.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gmbzhlqrn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/grkllbwmo.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gpmphbust.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gmbezojko.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwzpffueu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gtmekzjsd.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/geijbnhud.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gwtbsarro.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gtvagdman.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gtayaesqu.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gwjejaxhl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/glarfoloe.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gvuhosxwl.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/grmxyljuj.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gczqmxuki.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gmrhuzcgd.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gvfnmeecr.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gsivceltg.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gefvrhvgm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/grqqvoiga.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gykxzytyr.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gunbmzlzo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/grwgjsfdf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gnryyppcd.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/guyemkodl.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/ggptgsocd.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gszuqvpdj.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/greiavtas.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gmayiledd.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gvuzxpqfi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gzfxvawht.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gokeydhye.sHtML


<!-- 参考信息 -->