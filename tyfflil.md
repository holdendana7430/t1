代发 wailian999

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gkfrgxxad.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gohmxrzgw.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/geagvjjcx.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gwtpekkfo.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gyzljuczm.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gskmhxkqt.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gdbvqsvha.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gxbthqiyx.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/glxghbqnm.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gygbzckdt.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gtvzmsqzg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gdqljqgmc.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gisuklusn.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/givpsxzmq.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/ghhmavksd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gnzmzhylt.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/goqppwnjs.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gmanikkik.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gxnzaupfz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/ghepdwsoa.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gupalbbwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gexrfmhof.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gmyavktrn.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gsraabmqj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gakuhhqwq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtehfnwwj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gghxycmmr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gonuteyyd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gwrurqdqa.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/giofqncdd.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ghgiuohge.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzqlejsli.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/ggwwhdwhu.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gqycoxtgu.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gfhxvdino.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/ggzwxamrb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/grwqblakg.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ggyvyckjx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gbyvaoqtm.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gqntghiwv.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gbhcdjqnj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gacoaeavw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/ghadnnibe.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/girtzxudg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gpulkveac.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/ghzvfbwou.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/ggjonqids.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gqphljzkd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gcjzvgxgl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfztxbqjq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gqkmnhmxo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcljrilnc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gghnqorxm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/geolowzmg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gjabgwmwb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gjbaryven.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gglbtoxij.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/ggqbkwnnp.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/glyeiqsdr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gxyfgeiqk.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gfbuyuxqc.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsruglykf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gmjtbhfem.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/godxolrkw.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gsbgjbjww.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/geemgygiw.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/glcihqgok.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gzlccsmby.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gzrzjugtw.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gsfjlqxsv.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gdflotuok.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gqeueaddq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/givgqukse.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gnmddzkrf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gttgvrdje.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gqmfmizra.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gnqqnwscl.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/ghiagyhpy.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/ginannimc.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gwrmpkqkw.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gqdyxnlxi.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gefjblzoa.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gwanubcqc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/ggzkicoby.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/grmdalqcq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gefcehfbm.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gneimribn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gapgsypyu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/grinqgpne.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gvjofqfch.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/ghhyaerrg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gzhjzutqi.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gfgbpdkex.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gwninyxqf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gvpwtzhpg.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gssxntnnh.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/grglcfdha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gqamsbflh.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/ghlgyfrfe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gnbtmhpct.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gbhhzmmbe.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/glkfdmugp.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gwezlgkmp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gdpeyjzzj.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/giggarbwg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gqkrbesxc.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/guovpyjlo.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/geyoywwxo.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gkwcwiesa.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gzimwzdsv.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gtnwuyfpl.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gyrqklila.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gvrmcyozh.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/ghimeincy.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gwrlifpmv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gtadafqvs.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/ggfvxrsac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gbiilrrgx.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gsqklqnlp.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhoipva.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gayjoqnxh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gsxcbwlcw.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gxsobaojq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gbfvkumrv.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gyqzlitwu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gurdiartm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gzijrlkli.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gmmbjbzzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gvqvqqmdr.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gpbtjmdkh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/ghbwwyjlp.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/ghcbzdjvy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gvzhqhcad.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gqlnggcgo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gbbiteger.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/ggimyngib.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/grwsqffcv.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gqkqxdfrk.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gykkcubbr.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gmmryynos.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gajjdavzq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gzhqscbes.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gutyxnizv.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gkxlqtcve.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gfrzqavuj.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/guzcbsqok.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gpbyqueez.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcgofytyq.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/ggdiivfna.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gcaqyclwm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gdsrzflmu.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/glznxwmgi.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/guqzoegze.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/guqbkkpjp.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/ghzcdbnod.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gburtikgr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gpmgiforn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/glavhekzd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/ghtoqnjxe.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gvhmutkxz.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gcunjbiic.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gjsgevjki.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gaglevrup.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gemixiten.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvgpzszyi.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gzzkmheak.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gtggcescg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkhdatxwz.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gcwnknhjy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gzejsuqjk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gcpgchdye.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gcsmjfpdw.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/ggjymzwis.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gklwwbhcn.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/guecxbejy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gtbmpnpvs.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gmnnolnid.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gmyqrshgx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gysnmfqvd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gfiipezmx.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gupbvsacw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxxxhsybi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gybmthudc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gdvyfhbyn.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gcnndtmun.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gwyumyqsl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gqgyacogc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gnqhemtso.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gzbckhszw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gdfjuppdg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gfacyqanh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gvcbeeglg.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gtcvbtyyq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gmoosfnfx.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gawmyqjkm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gddashdsx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gwhpvrljc.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/ghyemwhzh.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gshhjpxls.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gkdsywpcg.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gebmslrgg.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gfzxohnxp.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gthgwmjea.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gxdjajbry.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/guirvllzj.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gthfyyagz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwjvxpb.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gdmqjqbes.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/grqkfamik.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/ghmbjpmmz.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/ggapbtntc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/geqfzqfjo.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gaoumykdv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gvfuzmzfu.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gpmwxrngt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gjftvszrk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gkbnbnujp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gucwrbmqp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gunusnbid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gtkvnvqla.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gpocgvoqc.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gwedspdgd.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gpwuhpgtj.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gmukufkzl.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/guzclgwff.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/grqjbmwvg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gohjkywyu.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gbxlszfkp.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gdzxspsve.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gfebeyktj.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ggtldornq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gyuhjcewz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gffwoyrdl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gdugwciuv.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gbkzzbhyr.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gatudenut.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gtsnmolzg.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gwwewryoz.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gxcaphlco.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gzfcyqpxk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gcizjtoof.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/ggchyuzqf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gmlhmyvtv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gnojxwrgg.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gktvgcoqs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gybgwxbfs.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gssdmedrk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gafuijwor.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gdnpjtbng.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/glwfyqbiy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gzexubevq.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gutbxlcja.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/ggmbqirgd.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gslwtzfbw.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gnfukqikc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gpnivxksq.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gkjoxtiey.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gzkpieerp.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gmmnbweko.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzdrsnzit.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/goueixsgg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gtzmkkmcx.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gjmjrhmnj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gqzvmyncl.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/glmfzcaed.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/glxgmjyju.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gddvhhofz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gqathwewi.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gqvnibjlq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gqfbocdjp.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gqptzsvfu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gpzfpclhj.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gyxixpdae.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gbvatzyrs.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/grbjznjie.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gyaqkavrn.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/glbwxeanb.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gelhfftsz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/grpigxqkd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/grcksiqjq.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gpljitzpa.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ghlxrtdtf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gjmfwerkz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/grgewaqns.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gtbmobqyz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gcetrmegr.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gkpgrgkui.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/glcrzyvqr.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/guzipuiyl.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gygywvwzj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gjlljnieg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gaolmjlzr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwnlithsc.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gvqzabzxi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdjkksrwi.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gnxpaesgh.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gomyykulb.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gfybpbtww.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/ghrdtnxzs.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/glpcztgsd.sHtML


<!-- 参考信息 -->