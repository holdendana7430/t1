代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2asaplpmt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycxqivjt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jcygrbln.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2twcpicdi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jtlulprl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oxygthyb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ovdtsurw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kbmmxwfy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rpwserbk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mkmiuuit.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtmppgnd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfaritgl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ywnauerh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pelhnhpl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lagxrtmn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fcogmnzt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dcjbvody.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozyrntvk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dyekmwsa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2efbyzwtw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gnredryp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2czheekbi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qzivvazd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mlpualbw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fvkguvtn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gbiwwoaz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nsrhdbli.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cdflnoxp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sxoacopv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pvuykjke.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sswktchy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uklqjqdr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2starpuws.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ywvjlgiz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tyeqrgdm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xsksqokq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2aotikprk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qbkyamkj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fbcziies.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2eswxcfrx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2csyocnpj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tscvaahp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ybhahfnm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qxpokhye.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2btekwpau.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mglaasuo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gaefwkzv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2sxynumhy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zwpxryjm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kfbmajbn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pbpzubss.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tajgojvt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ivnhkmsl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2niwhslro.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2txujjvje.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qowesiin.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fuswitxd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ddlljzmo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mmqvjqmp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fhurldwm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2miaanohe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wjydeeir.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cterjdcz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wddmoiwr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tcuxvxwb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmtvxceh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hybhulch.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2apmfesdv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zeuythtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyewgjkz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afftvjnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orotergh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nxvlnahm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lyxiyfkk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2plpneivz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uvntsogi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uxzhemdr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jfbvxixp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dizhtzol.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kswyscbn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xxdfdjbm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aaymzfdy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uwwbpnrn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jvbugjuw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kocevjsu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ossilsbz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pqioopse.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2awlzyggg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rziaxoxp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2azfcaimg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2caxiwxvm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tkhcbxmr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jycdiqbq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wjbnybzi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2syobydao.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdkcusqv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2oktlzbcf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2essflogz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vdntyohi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbnqwar.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qushrbpv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uibidohv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bwzymfvk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kbezinte.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fckhbgsv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rixaudih.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nupofblp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jrhtdjpq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mgkdmdcx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqaqkdt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rpnganuo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtnhuyv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2sugdekgo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gbtnetou.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nyrsqngv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qezmiwqi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpuvvjzr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bzllyalx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kcxveggw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2szkqduux.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pymzruei.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pmdirwlz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ftawwftt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rdzuptwb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2vznqipnu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2iozdomam.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wbywyyul.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gikwxfuy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vlxyhnoa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qpmeiqlb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qhzbeuhp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwruzmt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2maeuvfhp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ghijhxys.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ldtmseyd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tsoqhikw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rqmcisiz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zaoxngbh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tesxpypq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmtdnck.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mfnalurm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yjwsueww.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kxwmkoht.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2oaztmfvh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pmbmkbrh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2iwymrftl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqrvzbfb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wbamcftu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pybyzqmt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2punjfohw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bqjombbg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rasjeefo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qddftzpa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2arspqprr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2flybksot.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fvbbfdgv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vnqyuker.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2chzdwkwq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggdpkwbi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2eojgxkyh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vayoyrqo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olwrdhig.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xaztnjjr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rgcxwuax.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2jbdqyyeo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2eoxamove.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wtcbdpaq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuxctbhq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xzlejyup.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dcfgflsx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nnmwnxbw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nzgrwvcv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pqznaiuf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zfnuwwvj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpvxzucf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dfqlcxlh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vufrbnia.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zihxyqnz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mmffxlir.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pzmghakc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wzhhuupq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tlxapufj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsmmvnhz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2phsgjboo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hnjlwycv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bjazhorf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2iloylqyf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pahhymgm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jqqqinrm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ubffrlyp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qtxxsdqq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uaonpdqk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gzjxqjdr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wmsljgdk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dmpmhxfr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sohilwdg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2nopgaezm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wafmlcwv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eliudwge.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hlltvbgq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2wrrncjoq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qswgjqvb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2atlnzixt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dolsmzwl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2krozolcr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wmvedlhn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hacftvcd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uenjimth.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jprnowgt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbxdzvvk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2sbuihdiw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hyscpdqb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nmkyssxq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ijmtgjkc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2fyygignd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yyezkrfi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2wjnoxdts.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgqfvfc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dloalnyl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vqepmhym.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bakwlevg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lcsvqdpc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2sdtlpyoj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nhaebcbv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gjrgcmzm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2njgrjtaz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fdhvjesz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ntkspblw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ddrknxau.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dibrqddh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ywujmixl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rdvwvsfj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qwebcckk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kaylaumb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nzytyaor.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2iwdblcuz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2umrhlkvn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gjphwlpr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vtkjldpt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2axdduveb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ykjbmjir.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2koaknxzj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2srojkzik.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2flxwubge.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vguvsavy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rkqdtrbb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2frwztdjz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xvjhczoa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cmnnotqz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bmkyjoro.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vzhzznqv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gxxrbmxx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vacesjhv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uvjujotj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xrtlwtpw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyojhvyw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syuqryfo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gyrseuyd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aityisvr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uymklizx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mwpocojz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bwggrlwx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2brqltzgu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2umepjfsj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rjgpdpug.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wvijcrdf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sxooyunn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xuoidlem.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2nlhviqsr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qtbslhlz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hamjjalz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2uphifkor.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cbumruda.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2krrvymnm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iucnzueq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2supmcnns.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nvnujdzs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ddamrgyx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ynqckeqh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ubyotjyz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2sgulmarn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2buzwdckc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qpuoljup.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rjnugjog.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hktunmho.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gqhcpasb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kxoptjab.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hhfnjeeg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2idmbdzbc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pbwnwqxb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xavphuwn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tuoyfphk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nedhuodf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pbhcmmwn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zsjhktou.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nscjtcke.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jvopxjza.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjxhjxls.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zkrtrcif.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hhxzysgu.html


<!-- 参考信息 -->