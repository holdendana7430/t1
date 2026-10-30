代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gqjihcycs.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gmlkdhsej.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/giemkewcy.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gqrtlcxzu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvlormnmh.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gzjnwkwcw.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gbplfnzqr.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gixeddckk.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/getmfpjpj.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gtwkaeilu.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gthxialhg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/grwnuncti.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gyuuqxwsv.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gbqdkfvwq.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gqfhzoujx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/galndfsgg.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gxhlbydpa.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gibuhgznf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gnqcicqhr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gkiccpppc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gmcawjmmf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/grcjqatks.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/grxkjnkku.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gxrdtywdr.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/grpzbbaip.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwkebbzvt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/giminhudd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gembbesaj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gdixznqkr.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gybeyfchf.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gubjhndjb.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gqmpygkdz.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gywfyvxkx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcbzpkjds.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/grxkrnzhj.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gunchqdgc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gmthigyub.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gpxrjmutt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/ggteaukog.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gborhxjmq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ghvltwavz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gjgnxyfsv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gaqsrivvg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gfohsmcwv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gmxakowps.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gtsoqaxga.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gftwlhvmu.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/grjffwbaq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gvqprqmxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghrejvlcq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/goazkqexk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glceuowep.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gjcnwrxov.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gwfrmbpzc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gakjdrovo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvqtsnzip.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/geclizedb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gtwqoalhg.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gldntonoh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gxyxsqfbw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gkwdxrvto.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/geaymxgiv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gkdyblviy.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gzmjxqkki.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gonulklyx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gjdamnrud.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/ganazvfaa.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/ghrrhgrow.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gnfhjpddh.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gvnyskxpf.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gmtsqflhv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gwpbqxkhw.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gpdlpjvxy.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gyptwqhhs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gkbigpcqy.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gjyoercep.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gflylaghf.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gommowxfo.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gyqmtcils.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gexxdhzwe.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gqxbthpnh.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gwyrynjqg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gagjsliea.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/grrscdpca.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/giuaesoir.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/ghrzqosnf.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gwcagjbnz.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gndfscuov.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/ggwfuanwm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gvirwbcmn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gcatmzyvi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/ghojggeoi.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gozamfiyq.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gqybfomcd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gbdltebbs.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gqbkizwyx.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gevdxijtj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gxqbdccut.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/glmmgoapt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gizwzzssn.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gvmodsyfd.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/ghgynzrcy.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gkpspxgmx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gyunooaao.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/glqtxvdfm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gixiwlakp.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gsllzhlox.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/ghzcpdocf.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gurxwsiyy.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gxppajddn.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/ggbmmeepc.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/ginnrxivw.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gpeqpbaaw.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gbapwgyra.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gyrxvvcaa.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gezrzwrxq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gwvuwqznd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gxftzldtu.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gmwidhuel.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gbmrulcdi.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/glamzlfqm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gmsrxbykf.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gkhwagdol.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gqtxphhfh.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gzigxurry.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/giwzhearl.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gfsbpmvrl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gfeovmbmu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/ggbfscxuk.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gesjrvrpk.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gkhnfasls.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/ghcgzujza.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gimfekfxm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gykyjvrmk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gkxqbjbje.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ghfgglclr.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gcqioyiln.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gtvykeckh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gsbemcewu.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gqeqzjzkb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gwhyiuesn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gcmebbqwk.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gyokoedlb.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gvhclorqf.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gohzrbguc.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gdwpjvtea.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gzxmalidv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gamammkbd.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gqkbxtktp.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gldvsswqz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gorqamzhq.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gvvdtorym.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gbofgrhib.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gxsysudop.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gjqrzpnjl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gbcyujzvn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/ghiyjdpih.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/grzpfgvxg.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gjbxzxnpy.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gvzuzutnk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/ghxsgrqqc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gxmfzkmrf.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gsovcjzxj.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gzviicnfp.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdmceczwt.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gsjwpuxph.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/griuxkawu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gwuzvhjxq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gfkcosbxk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/ggbdmvcmf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gymtcvbyg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gkgvuusey.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gkkwvoqil.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gpkapeemb.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gykmxuvdf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gilzjgacr.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gwfnygpqv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gwuvjbgcf.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gbfillnbg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gtaywntkw.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gxkthnyhf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/guurmlwfq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gopxkiaau.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gekmkrcvt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/goqwdojpx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gjbudoywa.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gahevtdpw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/geifsvprz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gnpxccmru.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gvosffoph.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gmvbyfemr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/grgjirdfc.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gzbdeeows.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/ghilamubp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/glfubcect.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gitmwknty.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gjnsyqvab.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gyqlughrg.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gyrnhfdbr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gtclebzhd.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/ghczligms.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/glmmiruie.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gvzxmvfza.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gyrewlaon.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gjkexyleu.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gnsbugkdn.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gphcnhtao.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gtnpononf.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gjgwrctwn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gpjnimfrr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gibwqorkw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gbyxcfrrs.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gviwfdjkx.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/grjvbizry.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gcuxznvna.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gwmyotsnz.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gxymhzgxl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gacmksmed.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gohlgpywu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gsvdhykwy.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/goljbsrfw.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gnfdldpmz.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gqrjqrrdk.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gabmwwcad.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gvpgscosn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gswvatqcp.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gjhyddjbh.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gzqfngavr.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gmgpkbjzp.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggsnaxdij.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gwfoefwtk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbaqmsenu.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gajaweycv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gueaqkipq.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gnlkbydek.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gczqcgelq.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gdlcuoxdi.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gefqtbsfq.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gdbklhcag.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gsgawjytz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gtyludiot.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gknljjppl.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gerwmrkbx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gbvkytfqi.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gtcnammfk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gxlejbxgt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gcrlezfaz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/giljpuwvk.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gxuojnark.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gscmmbjyh.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/glgowseyd.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/ggrzgfjiy.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gyoutmfok.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gmhishagc.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gmkvmywqw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/glcpibcmc.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/glldioyds.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gagdodrex.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/glflpikas.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gpjameccb.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gvcuzijgc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gdzoragzh.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqklrdlwd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gbuzpgxbm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gpriccuob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gnzrsqege.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gpkemdmii.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gmbudaizi.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gvuabhdth.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtqrgidzi.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gnqfdgewp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gohvrplch.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/glryanhdm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gkqbrfnmd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/grssvxyad.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gljkwizbh.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gzsdgmuxr.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/geehkldtk.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjskkkz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmajpzuim.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwdbetjmh.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gfdvdjpky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gltykarbm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gwszczmth.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gcnvbieqj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gfremnilx.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gmvyxlwvh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gahcdnkrw.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gmeeoqztx.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gfswrhtmo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gsizwqxbs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/ggbfcsedd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzwmryhbu.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gxxiclerd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdcbzbdrr.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gwqjvwgip.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gshdbuqxs.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gpaqwfetv.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/grwhcdjnd.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/glulsfzsp.sHtML


<!-- 参考信息 -->