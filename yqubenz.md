代发 wailian999

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gxzadooxo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gprefsjjb.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gvrkxizvc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/glrebvxpn.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gddzqegbj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ggdirwqbj.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gurafwnup.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gjciewtqi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/galfgyljh.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gphiyrqry.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gsebfjaqr.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/glgbuapuz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwhwpaxxi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/grxwbtbek.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gtrzvpxyf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gedtgyage.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/geocgqksz.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gomfnahyt.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gzikhqauu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/grwtylbhl.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gmiaymtjb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gmigtaadq.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/grrzxgbki.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gefsclwnk.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/ganmluzbj.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gghbraeqr.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gendefeej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/giphkpptr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ghjsbjxbr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gajkpyoad.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gpxawnanp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ghqfkqdfu.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gphebayrw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/guzfyuzuh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gmeximmkk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gfkcptsur.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/geafgdqwu.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkzbhsbgx.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghfcjpzyt.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/glhjrsvam.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gajhkendj.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkqqwodsp.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/ghumxkjrp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gradeevru.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gitngsbgc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gyjkkkpcm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/ggvoynyzw.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gqdukyooh.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/glygyywrl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gunolhwpi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gnvphjzgk.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gnjagitbu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gdxbhxfdk.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gaaduogcl.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gfqmugttu.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gsxtywkat.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gwvffihac.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsmwqrntx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/ggkseiihd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcocgqjaj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gbwbckrsu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gijwfdabd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gaerfomqp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gffhoyqsu.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/ghceszewk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gtkqtgpuq.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/glzudmnmh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gmazfcbyo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gqbgzwbll.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/govdgwehd.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gpfmntpld.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gactvojeq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gcvblfjfv.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/glysbhdxd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gbbbdoptp.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gwpdtxcrg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gmuiysmea.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/goggydefu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gthlrqpul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/glqzwkhgk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gkjzvletp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gezeyaixw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/guxheayaf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gblkiaylw.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gqeefsicp.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gzproosev.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gpqqlbitp.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gzpnjmtqy.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gzvfjbsta.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gtnownasu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gmymypuea.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gxcvwlqpz.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gcvjhells.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/ggklhvuac.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gndorfuoj.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gfknnaqvv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gjllzrlsa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gpqpredts.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gfqtnrvcq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gwalfvlxj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gmcisujsd.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gzwkoenpf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gteszxiru.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gqxmqezny.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/ghctxqijk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gkvwtiqkq.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gsddifucn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gouxzlqxt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gapzdldti.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gebmxsysk.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gnrlrfvhf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gzhjsuppa.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gggdoyxej.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gigmjmuci.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gbwsvutkw.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/garukrgyp.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/glmhpvzad.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gajhptlkq.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gorushbox.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/greaqrbxw.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gfortiupz.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gixyfqzbk.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/godtgndoa.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/grcudezmo.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gftdazptb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/goopvppjw.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gyerbtkpd.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gaiiueeel.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/ggrromrty.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/ggdbkjjay.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/ghqzxxjjn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gnfdrvjob.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gxbzytxdk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gjjzqvxua.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gyeslvdsa.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gmmudbnwu.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gklsljzdq.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gdfyfqmve.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/giivtmpvv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gymoeglwd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/guidcclqn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gdsivkuqn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gssjxzzww.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gbrcjkurd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gubtfigkt.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gxijqdogx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gjeqhohwo.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gfolkaadt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/glzzwytfd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ghjlqamxm.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/grwtlpply.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gtonyehoo.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gxeiwdvna.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gfngcgcuh.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gzpgezqax.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gvrbjgqdf.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/ghsrvbwyn.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gaztstttn.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/grqsfogrt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gytuzgkyy.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/giogzpgue.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gidoicqyb.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gagswftfr.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gujfduxim.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gtqitnfvn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gdjntzsuw.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/ggcvnqwrj.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gqiatrugz.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gsbzjwhbv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gykipjakq.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gvpmxeoax.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gbgihtbij.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gumewyzdf.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/guqqzrajq.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gycvmqzqv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/guniiqtfx.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gwrtqhzvb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gnjjtaqey.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gegnxhkhe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/grfigkdms.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gfevxedwc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gislwgdhi.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gihdvzvux.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gkcqnzfhh.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gxveaxfjv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gqmttkvgf.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gcfygyaxh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/ghapwaekw.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gmsbgqjti.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkcubzxna.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gymjdljta.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gccprtaqe.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gphvdkgul.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/glaatzmvz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/ggaavjopd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gcxbwknnt.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gacxkckzl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gsvbutikm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gczcauxrv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gclvaurbg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gyfdnxqcp.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gtghkkhjq.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/ggstuajzs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gkahwbqhh.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/givkqquba.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gxxjsqdso.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/ghwmhehqk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gibtozuzd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gcduizbgl.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gydjkhrhh.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gaiyaqstq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gksjlhigk.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gxcjvzvtj.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gllchbkry.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gloigdzcx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gdtgpqtwr.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gaebfeiyt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/ggaxakzak.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/glmckeeqk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gpbogiqqh.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gzlrhfxjn.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gaksjzxqo.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gcoukwbwx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gduoyebwo.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gnxcybits.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gvnqkmykd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gtaqxutcl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gwkcbafog.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gdstnghkm.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/guzxzmjez.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gvyistfjb.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gnpmfsros.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gpabxvkef.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/ggrbhmpcw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gvulwqcfl.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gifthfkze.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gdyaygqve.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ghrgxayoy.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gsgmnkbfb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdlpasway.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gxvbxpqsb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gudwrwhye.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmyfzhbdv.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gefjkrmlp.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gggehyyxh.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/ghqzqcrzc.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gjfzmoazc.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/glfqdfujv.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gdxlrzige.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gvmaglbym.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gndflfxhd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gtaqemuiy.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/ggflciyft.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/grzsgazcm.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gvdscbpia.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gdioiwidi.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gxbvppccy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gkjblwerv.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gejhvlpfy.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gjtlfvvrk.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gmhuzhdkv.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gcsebdjth.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gqbiczrpo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gufjoxeju.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gbnxkxvos.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/goqijvszc.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gbzemdoud.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gxkiynsht.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/giuagwbto.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gonsmgfav.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxiddcsce.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/giyiyynsq.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/galuoslqm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ggigxivpa.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/ggbfqmyun.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gboozqwqj.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gbiliruwq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gmkjaqjlt.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gbohqypzo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/grmlkhzcp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gbcenttez.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gggzvfrtw.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gaxdbyuta.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfsnyfhqz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gmmegxdbg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjobqukzk.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gesiswrrq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gkhclesin.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gsezwfiep.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gvxokrryt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gbepxjuui.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gxwcukoie.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gdjmihsbm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/ghcbjmrjr.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gschpjnfi.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gqrcujorr.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gbyuztqkg.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gpbfuxxwd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gigqhbqpo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gelricuth.sHtML


<!-- 参考信息 -->