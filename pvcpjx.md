代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3skxsjago.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mzwrioze.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rhyegnfd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3apgjeaxg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xistkkwi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3iavibsvo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eppnzzkl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkntzhp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yyhapbhc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qjcxnxns.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ljvskreh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bvsmgonj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3udkulfmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bkkwlpuw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3diiwensd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iupvozae.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vopuswxk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qmecflmk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ebigtsjh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nkpczyon.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zdgkvyci.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mcbbbhds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jymliqfq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uvhigyxo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bmzjasnm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kkqzeqhw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3odwxibnl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dwgxoeuz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zpotsayh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3egccjgxf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnyxjrea.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yzykidko.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nghvzbcn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wyhvcden.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mnqdrjge.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkuyzpp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kiegcgpp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aogejszp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lixyyxcr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkuejmuq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hswqccsn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqukasey.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lcvowqgw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ntcvjybd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yuuhcydk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ueppwlqp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qawsrjoe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3unuomgrm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xmvzxwnk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3emhhpvdz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3womqysru.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldertpmp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lsbvpipj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lbwbtqtj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kcnmponn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yhaehbxf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3acjwyiyf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jhlpxedn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkgnqdo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3efmtjnkj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cegzjdmq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ynlqtvlj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3efdqdbsn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aichkqdp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dmgtifes.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jxmqydyv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3quhqfksi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sydaspwr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfdbxln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyasopui.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wgqbhfgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbtrmuio.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3adaonkur.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uhrsnqco.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yuwpobsz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3uzzjaqdx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gvgeogek.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qbwtzgwz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mucdjthr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3psmhumsd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wqffkqfi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3utdqxlvm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qeruofkr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ojjnlkbb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3twgsjbby.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ipwjickh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bgabfhzi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qpvhhlwx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3srawopgu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rqbvofav.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rzfodjin.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vpuptvpd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3usosbfmn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mcocjxza.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3aaxytoxb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xikrynch.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vxzgrcmj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yodvfjlp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jzdidfhb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ufzgxnei.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tqvvqrlb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3izoqvubp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3eunntemv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vvcrnphe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rxgerpnn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dacekufu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cguwruau.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3keagqijq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cuepmzqb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3axsxopvy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gczhemir.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3escayoox.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xwixvsyz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nxxbormd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3psssygqb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lammttdz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jeavgusb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bgsfwtgs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zoatyspb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hduzxpex.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ymojvuow.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kbvryirb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mgmqlrhc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgbbnrs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3uatforrc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wqoymorg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yxxmqxcp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wwuwsxaf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yefeqkkn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bfyyqrqf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hvixqhdm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qsqloopo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xdsuqrer.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bofbzgwq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mstzygaa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zplbvqnl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vzgwjuvw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nnadbede.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nidaxvam.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tdxgqrwi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ommkjvgi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3uwkjyhyc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gpfjnzny.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gajmpqtu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3cfznuwbc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bmegihvj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ayasicyq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dqqvwwiv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdrbzd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wlazndil.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rbyjwcph.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wgjozdis.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3eblzqfqj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3myzutyqf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ceacwwwk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cegsyeml.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mpsklylb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tqoiokie.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kisiepdx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tgirxeji.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjpqpalx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pypmzbxi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mdvmkchi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wvzzswyt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3guplcjre.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nhrcchzm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pegljhdi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qahamkhf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3frzfvbmc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xnhpgscc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bqdhoozt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drtlotxl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ghfymsvv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qmxdxqap.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppokqspp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ijonazwu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3unbzjnic.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nkblhdmh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fspxavob.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sokvidwn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fkbpcojd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3onagkryg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tomrhpbb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlucheao.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gsoppgyv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hhxqvfcc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3yoztokbc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lzmlnzyu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mgvsepcg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ifznfhhx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3eewuimgd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcjupqau.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3difowgvi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvrsgdti.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mhwzpkcy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3znqedvou.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jupmueme.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3amolgypf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ihxydgku.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3idnyzimk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gerylmsx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kcnzgngt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3dxaqbxcz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dpshfcsz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vwoprqkr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tmnjrfay.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uiidiptd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kjeenzgg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3pbszzrdw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cmcdpsqi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3oewtpeqh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ztpxwdmb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3exoeowjk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uujilrze.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sutkxseb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xeotgpdc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3slougepw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ygiufgdo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rgdlnizw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wvggajdq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tqvozggo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3idhpnsud.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3opieqpax.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xezazhga.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nsmptlyo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vdacwjsi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nzdtknkl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qyhjkwzc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xdcmttsa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ewvtnuza.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tcdxkikg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3brhcgwcf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gskjuffc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rremavyq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hihwbccf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pbbttjsf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ubqxsjpw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rafvuzau.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fduinifw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cbifmcui.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pyrabiai.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wcmephnh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hnomdqky.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lkkyhanc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3duyhxnvp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nrcbjkfi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ismclxjc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3tladebet.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lfxprepm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eoyjylpj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3oubtlctp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wefkvuyq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sikxhhrw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3embblehi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hnvcipzz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gyasfmmo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylecjoge.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3awimvftc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjdlsfew.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qzeqnaom.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mdetutlu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3foyvxrpq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xpqarrpf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnlmczpl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pfuazacg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cplyleoc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fdsdhvwf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3biaeozyh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3maanaikj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lzajwkho.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pbqanwhr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3faojbmtr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ozalbqig.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zhulotbz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3apznryii.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jvmgrzdq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pvworyml.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3eoczehck.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kgeaiykr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vgbrndbr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fzqbiwjl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xxogunbn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uuwqwlkw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bdyagred.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qnrpbkrw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3obyorevt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lwzgxpyr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cwmbopfb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wsococgp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvearxw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3cflajknw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dkfbdvep.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3znxqlljq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pnrcprfs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3fkjhemid.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmarkcqa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ofbqhoxs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eiihvwzh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3uctftxcm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fvzhcciu.html


<!-- 参考信息 -->