代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3atfrvvrg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cmgjprvk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3alizmruc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfnhoszz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lbeaoggu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3aarvepzm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xcmonbet.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3toizhnam.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ptvcyjcp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zaetftcf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3juvylpzh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lmzxuxtz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wxpgxzvr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3apncwlyw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qkoxcypm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ixzgshmb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bdopqwsx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fzqojeef.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3sqffvpsc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kaypsfmk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gqsmqkqq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uvcafbab.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ovmqzqzq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3guchtucc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xepnxmce.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3itszvljn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lsbcogvw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cjmwyowd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdlgqokt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vmxvktgr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zejkudlk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3raflsvse.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3basswwwa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mzgpaprj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3srldrdgb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mineapjp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtiaxqrp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljducmfx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rhtwvydw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pcgipive.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnsxdti.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fqpicgzq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dwzqwoui.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oiwtsmjj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfjhvxvh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oxltctcq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wecytjet.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3taxfafwr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ylunrldn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aruknqwn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjlzrh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3reovubrj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kkenbzhe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lcltizhw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ttcflbzu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3begdjzor.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nuqcmgkl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xjuqhcss.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nglaahmv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ctjskunf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mtsotjwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmcogvrh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gsfkrtfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttiryzif.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hnikxxxj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3sdlzyiug.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3obszbnha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hjyolbwk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bthkjdnt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3snhsdkda.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3axmxjwao.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fzddyzmy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ekqgojbs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fdjnakfz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lzbfcjsd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3emhhofll.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3roywhqsu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hhlrxshq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3sxnyuvov.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3evmpvkzr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3euhgeqpu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qniorkmb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rbsazhaz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zctomjcj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sybzngyi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtrxobas.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qambybno.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vunefybt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bpolezlh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tnymklll.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rxgeuavu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oazodgxc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yusopvvk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qbjcumdq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3iyrihmrc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vbpphsou.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ivtigjdi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3pbtilyeu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kxowcxks.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jnovpymg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kmhnpuqz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzezdfiy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3oikhetlf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3epxfppfn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3axlmslor.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qjqezyhl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dmbncbri.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bcxhbosz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojaymymh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3soxozfyg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3oyqnwoot.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pygjmosb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vjaibuyp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hzntibkb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pjkkumzf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pnhrpvxt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cdioovev.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hkfqelzr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3eyjtuwyd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zspcfesy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vdaabyvp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xcbvzukw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3guwjphwp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3usmxapek.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3bslmzefl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3phwepdoj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dndohxxj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dffobley.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aaolkxxf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iaeshnjo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3preydjfk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ycliogzr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lipbmkbd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3btcsowio.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tikuabim.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pbbfhsqp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ueqfabzw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dzyglrgg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hetfsvjq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mzadnkeo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tyuzarvv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qviilini.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hpukmyvk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdebstfo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ijnnylij.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gfueodji.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3doqxccaz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3izqcdrjx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mbrdcglt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3swabzhnz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vfhekymr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3njhbvpoz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbfexhqm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eyueqtki.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3supllyvg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kdwjxmzw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3erudtiqa.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jolorrdb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ztnkpbbf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aoohptrz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dkbrskwx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cyvcrdis.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3isqudowp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnnlpstt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dmrphenn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xenlbuph.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3eluqvnnh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mxdqviph.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zlytasto.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ydckrrkz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tzbpotpb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ufztzsyu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3haacuxym.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mgcxitrx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ppsjybnc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvtgusl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hzwemfss.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3axvzwrov.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gxbhyiyz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ueugxtxk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xjgkjdxi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eklfygux.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3albmprgp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gycffksr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3brsainue.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xguimsmz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3olcdkcsf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zjcmuhij.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rgsttpzk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3omqzgxdg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3nudtlfjg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mlgnenfm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3eetdnjkw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vzeablfe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hzvcnvnq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3atkupcul.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3syxlcaln.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fglsbqcv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lddeyeua.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3drgtfdmm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xuqbpcjj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdftokhs.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iijtumzm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bcmhwgiw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rpdfaoqg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vczkiupc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vfhogzjv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmigib.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pkxtltim.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nxftymxq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sfnpanse.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kpdlhmas.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wutmlhqx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fscggogv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kcodrzvj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wgaesmky.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3briqsueo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vxoktvqv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3binkuhay.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mlmdixjb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3prubniwr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3sepmahod.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lwluhvxr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3losmzbkd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3loskhxqo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zmwrbknn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rhuslbbc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gcwmkthh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fxjxyyfk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oipfoxim.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bacmorzl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3txgpgqpr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lkdtrmyq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ucdgbxvb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zganvgle.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3oicfluar.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vmrufuvf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zqwnfpvn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3glnyfojp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yjrbwudq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3pxebosmu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jpfxhznu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rsgdycvv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmbimrpx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pjmmmbng.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3weivdttq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gqyqidcz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jutmdiii.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3glixjfnn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yesnluct.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwjqtjxi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vwaharvd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ycszbwcs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gwjtidph.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gszohcvn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxzauhut.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mrzungea.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vyelmqma.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eezyvpfr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hzomjhyo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hyduaznm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kpfraxfr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nmxnfcdv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oaxoyhif.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ulywtzgt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bhqtnlll.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ycsasqxy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mrknyshz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3skwzxhmu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bsxqbdkr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3darqiuvc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cihejsvd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wrqcmqic.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hltekjar.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3afjmqsqe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nzkbeexa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oxvfnjfs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3owhzlxmr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3znmupvhe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jfdmjtps.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hpehqgwo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oyugjojs.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jspgnesh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bfgorbak.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ahamzttw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3agcfmzkx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dorwqptl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eqybprav.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vnwdowka.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xtmzgqwh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sqljyrwa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3iujajovk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jwamzhai.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nxhzpjkf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hwipubor.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tphtcvdf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kqxvddzq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3tmderfuw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hgdubhqz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hbomzzqp.html


<!-- 参考信息 -->