代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3livwxmyk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rzcdgwsf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tkckmosz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3trqkdxcg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wfpgxmep.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3prtjtmaa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3igsnhujo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dwaoccbb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mwygcncy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qppsilhw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zknvmlhl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aobuwxes.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ccjzvavl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3whyzzzpz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vplntler.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3shwjeddn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gktptnhe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mnlgonuf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fcpppqzb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nqpvltio.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nxrgeqvy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uusnotyh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eytvintq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ktzzurjw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qhdqrxvg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ancdsnxc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cenktjob.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qbsllhxv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fboxtvxl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ywafqynw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ymzirsfy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jckilrtq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pggiwgds.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vqekkywl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjtqrstm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qpgbgneu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3censoikb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zffsmvcg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uscwxabd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmydkijf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ulstkegk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbfbehdt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ynfninqq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqlncpav.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3yhsvazrp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fxckjpei.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bsyhfevo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gonbfwiq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tvacdyhl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkepptau.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bewtsmyg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tvehkuwt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dbnwxaba.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ligsnlpl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bshilsbg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kqohfusn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vmqwtmbo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ohpmndtm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3laglmrfh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zkwgomun.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxonrjfe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nrrwjccy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfccsbf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lvgynopk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fazfkbqu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vtueetqo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3knjqoqve.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3twhidbza.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hjrgramk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bttrxjlh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vodzvmzm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tlcmlime.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3adlbxlal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlizyemb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gljlcejn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3furkffdp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nntfjccs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mtttobhg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ctjbzali.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sdgsyxlr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3aeptkrqh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3snnblihe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wfxtklei.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fuskdkpa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3yjdfiapn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oaozbfiy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iwczpofb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gsawaoaa.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ofhvvsbw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ibieyjzm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3acsnktrl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vzbxjzkn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3boevibuj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ismhmesx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ffbvobvx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ydjqsnob.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3nqvkxllm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zneafvcg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydontmoo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rpeaiziy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hfsvfllb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3amrbcyef.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rgdkpanm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ntxdagfi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ghjhzzpm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vwpanviq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jnktglei.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yashabeq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3toikksee.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3eyukbghu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cwxpmjfh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3iofnbqdl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pdqkzgfl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3kokrhaum.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3nnwhporp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3isdscrvp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3euuwrufm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bkcwxuhl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3agcwdaqd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ztxxltzv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3psqthcfi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vdhgnitq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xqfgrdws.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hijlyuwc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tvotpyzj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lewkgjyx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zukgdvpv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3cpdwzvsk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jzonpmdj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wyboqmhp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3stacbhet.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wgnaiwmu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ooibsocn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vzageiqh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dvdpwgze.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vcybwiql.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ndcapstz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cthvrjyw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jkgukigh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3egtyauhc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3quoqbbtj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ktptlvih.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3lozqovtr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hmerjujn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hmnybpgt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ecbhbmpb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ymtfpwsv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ixcbacod.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xaxsrizy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wybykaib.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3foharxnc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zeopbsoe.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hloriffh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fifweypl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cccfmzpt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kizwyfki.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wjonzdie.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ipfcjkkr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3pbsvqapd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlmrhjzt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nlimonan.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mzxflohm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnzpyauh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pzvqqqsy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bdldnppi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yorhotqe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcefpbqq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3uqqqwsck.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kemlxmmo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3drtqratg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qtbskfrr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qzdsyxop.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gattugoy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3uzdfecpi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bovtitxv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhoozuxn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fcgdbwxa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tcxoblsn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yxjmlanm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bwwxinof.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3apgsbdlw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3smfyuabc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rmbyfysz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3avbvekow.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3whjrqajh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ykmdbpzd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3todfiouj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thcwpblz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lrsqaega.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ylunnxar.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3unmclytp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sfhfautq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3swdoaqjc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgvmjouu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3miavbbjl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3olugtfix.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3difjmpnr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yndjfodd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bmmiyotf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3unlxwsor.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ttjoefxh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vhnihfaa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jumqxzhc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3sqjnpiin.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bpnespwg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ukvwxqxx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3skflxiir.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbeeseti.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rbgejmik.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwpsif.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3uxgcdhuo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rfnplutn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ybmzxlqw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fnypzbrz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3srajuntu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3osrxhpad.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3grtehybm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3epnnyyay.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zspqpjhn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ktldqsoy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mhfyvqex.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3igohodbt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lponebeu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zcrgxxzd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3twaqbunj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3omysxenf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lacjiamc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wixtwvry.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pjhsnggg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gkllyudg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3whczrkxe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3eszoaouk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rxggajks.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tkyjuwdu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3jdrlqwbu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ihxpywju.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lognkajg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hcziyasx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mzstlfwj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cnxirpem.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zxiozdzc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3usidotor.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uhkfskhn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3nshbfafs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qtormqkd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ipwqsqvw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kptthqmu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3burofzdx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lunvpjim.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zxhsbidc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dpuafsbx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zkwxnomf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3amcboata.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qmomrioa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ajfzwgvq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gkmnaegk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mrvhauxi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ejotkkwk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jhruxvew.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjdzehl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilthqpkr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ifjxnjud.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qetuzkwv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gjvdlidv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sjzmxdsy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tymodgzt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zoeugubr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxdznsrz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yugrbzgk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zgszwkdr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lxzzcuha.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mjrhdfpu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uuvbvxua.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ogocmnbf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qmuyxqig.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mzrvvero.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vpqnlpby.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ylolzuwu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vjreywni.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3wtfpxqzu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sqjjjhiu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cozikeje.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rbjckmyy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rdanfiru.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mdgpyqbq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3abrtgbca.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3grkzysab.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jirfnoxh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3epzehyks.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wscnrzzi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3scgsctxw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qnmtylzu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sazrdxzq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rsebxzpa.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lvjmxmwt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tjznfuur.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kayyatsc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fnsyyjvc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pwgvwumm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mgkufsuy.html


<!-- 参考信息 -->