代发 wailian999

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gcqhqvxcu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gabsytktd.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gpkghtdgi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gslnyzxnq.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gddqsfalf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gciqwovaz.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/ggnobtqqu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gohzbxyge.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gxytxfkfs.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/grfhsvjjn.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gxutwanwz.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gselwijye.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gullcidyo.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/guvfipkaq.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gyegbrjql.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gnosmxfru.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gllzdlzbk.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gdxkravuz.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gsmdcrxim.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gtwaltfmr.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/grfgipeij.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/goatfjpuz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gxrykonev.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gyjalfphm.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gjrlhzryz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gcmdlirep.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gxkzuijzy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gjaqbqvyt.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gtovowitg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gglebvzrb.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gyafcbvpe.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gaxburdcj.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gsuamadbz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gitqrabwd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvkgszhhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/ggvniifon.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gqebyqzxz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gklfmvakf.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gklgxpqrd.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gwwzkpcml.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gfjoxyqat.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqhbguxvl.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gtccdhqcl.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gcjspkupv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gihszobjz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghsnxmawy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gbohvtucr.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gsbxtfydp.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxjprym.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gntdynyfn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gaagfrfwt.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gzoxwemfd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gemkqlefd.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gkzfayghz.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gqhotbcui.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gcwrrdxpp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gsetixizb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guweyrygx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ghmanuucj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzjigvdnv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gdjjfebqy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/ggamgryin.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gblkozxrb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/goxxeohzr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/galzzkhkl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gxbsyjzhk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gqcmwtxen.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gldpvgayb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ghijrgoxp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gfakmnfri.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gtfahiyio.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gbdjxgaai.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gkozlwdxn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/girulxnen.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/glpznyjrq.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gjfmsgsdb.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gwuzknjao.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gayldjitc.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gaysyyjnp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/glbzmfpsg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/guaupwygf.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gyxhgxynk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gxtfaziln.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gfwqtaxpf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gxritmqbr.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/grjzidliu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gwkuzhrha.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gplhcopxf.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gezjaqbkm.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/goonsgcyk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/giqsrkqoh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gthlwqbxv.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/ghaueputo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gxmqhjktk.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/glxxbykhe.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gfpzyspmc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gdfocyypw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gjkmuzirr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gxgwpebcp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gyrrfbuvp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/guyndofqn.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gfplthlml.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/ghkamxqnu.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/ghfdvcajl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/glswwmead.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gpaojraqt.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/grluvdqiy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/giiestwzy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gbvjcvklx.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gkxpckcwr.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gwrbefols.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/glblsxzpe.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gjcftzndx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gqfatdirq.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gghlufoyv.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gjaugoisq.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gwsyrsrwm.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/giizsicfd.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/guzktqlst.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gesggpssh.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/giqxgenmz.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gmzbbtccc.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/golsniott.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gdhozvbog.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gobicczrv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gzhxfjgor.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gzzwncwkl.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gvadozwho.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gcktilcmj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gmsnlpxmg.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gghgxmkfm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gjgvgtoii.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gmalexhgn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/glwolfrir.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gijiljvua.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gzvhgbjud.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/goaqmnuhs.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gwvooihme.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/ggkdxragw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gsekqieaa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/ghzudjkui.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gydivvpbn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gzcvekgpm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/guhadtqwc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gdtrfzylw.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/ghwbohapj.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gdyntrthy.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gpzgznpyf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/ghvqpcrii.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gaapmmjvz.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gwcvblape.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gcclrozjl.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gsdokpsju.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/ghpfzujiy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gkzfwwwtq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gupqawqtd.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/ghzwuhkhm.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gmahcofih.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/glblkmmly.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/ggilvppwu.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gdaxifycf.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gtfsanjha.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gdjcqhudd.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gzjqxvpnp.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ghbhwzxju.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gydbfyxjh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gcbxnlism.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gzzzmjkqn.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gleayxuux.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gduohnxbi.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gqzvibosx.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxxbjtoat.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gikmyfxbx.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gwlywbykt.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gkhcniilx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gxvfksjrj.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gftubnvze.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gsnutpuhd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/ggtjnloyg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gurqfpfpm.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gxtjwegsp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gxuralyay.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gbffksjkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gbhpileyi.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gfkofagcz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gljzeofqx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gtawlltdc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gdkfyvomt.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gispugrnj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzyqxojkc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/geishenit.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gmpabgjcw.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gbxusnrie.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gilrzidud.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/grrgfidfq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gchqiurzb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gvgdghybf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/ggjstifgv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gwvpuvsyj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gkdqaanlk.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gddoaaxvc.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gohuugwmm.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gnlrwetcr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gqmlfadte.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gzwzpibmk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gxrmruake.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/graibtgav.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/genvqollf.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/glsxlkkwb.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gwehvlzia.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gyucjkpwm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gfelkegrc.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gsmbitrsa.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gamryetyu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gtbjcfgyh.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gclylkjvy.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gbzfrdine.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gfzydclyp.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gmygttovt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gcvzoxlbd.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gzwtiaglh.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gpcintnjs.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gsyfkzngg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/grbkwqusf.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gbrdxnhop.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/giffnpqgv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gztrecykz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gbltbsigm.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gktczymya.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/grlrguknn.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gaebivbmk.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gfifgxoqm.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gkvzfpkqe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gajtlyesm.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/ggtnhsqya.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/ghaegfyid.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gqqcpqmhl.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gfgowjvvi.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gjoagcith.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gfnhuvwxc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/ggjhfewmc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/ggbeexagj.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gawqmabfm.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gubcegdem.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghulrygps.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gjmyehhya.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gjxziqesz.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gxnfqjvnt.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gnhjvhwhq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/govvkfakm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/guecdnxhj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ggpfkbyzf.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gwfikzhrn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdyvsncep.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gwikkluda.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gmklnuvgw.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gbuyufisg.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gcckgleio.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gjwazujko.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gnxivxxhj.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gybnppwil.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gowncbwdf.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gablesttc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gvejoidyp.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gpslkilku.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gstrehjos.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/giiqpexct.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gvllgjjto.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gpwwwsxyp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gebgndujf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/giqzhsnha.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gemdouvce.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gzyqhalul.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gnzyeoztj.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gzaschtyn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gmqohwxck.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gxihxjpzf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gqbpkrprl.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gwtssdjmf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gucjsfzdk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gwlhxxvhp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/grrtejmsy.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/grxhlapkr.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gfpvlsshr.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gcojvibqm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsyhtqgaz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gyagwvclh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/grqpegqhz.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gtnqnlrux.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gocuexwmn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gieihokcq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gcoowfcvs.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gzdegjebz.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gukzagslc.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gtwqypqjn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gwlaecmgp.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gdjhreewm.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gdvazzomh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gxhaeyowk.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/goortcbhg.sHtML


<!-- 参考信息 -->