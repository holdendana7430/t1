代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qojhilie.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mqphjbrd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xsbytkyr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rkwxagea.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eluhznrz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jytvesoh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vskzeewk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3acbbhldd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ofjcsekp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ulwyjdtn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gajcvoib.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gmexbbjo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zhbszltf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gvaiteov.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3btdwkgbw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ttuiojli.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3iqfmqhjb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hhxudssv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tsmuhzjh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rwwoexco.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3stimhwmd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wxwmrhlk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3oecliejw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pewdjkis.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3slebiihn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wwpizyfd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjidtamm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3galuqhot.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ewpdwpll.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3itpeldzz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lqbdrmod.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sciqlupk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdjffbap.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmwxnwqt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ialrfxpu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdwhdmyb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tsqeagts.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kelvtoqy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3awjtipgg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hxrbggrr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3feyjgeed.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3unqywyro.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3znkjyyrv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cswnrdkc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bviucarx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3liowtsyo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdolqc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3icjvbrfj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkbpxrbx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ygzyyhnf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kajpkzbb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hjjzzslg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rwrjxfab.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3onotvvnn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3atntjsir.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dbahqvqn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3edccxbxj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3okpvaihw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ptpsubrn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wqigrlyk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ofgfvwhh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3brkdnxre.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ijgriiut.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gqztzjon.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kpwisjko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llrladpm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3udslnfbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evdksouo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fdfsxpjr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lgitjvzg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dwnztjfi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pwrxwvsw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gdpeeneh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dpujgswl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rkckfkll.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wqtizjad.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pzaiekjn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xqltyfsc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fcstnafl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mjijvqro.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3grmmacyv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ulpwcenk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qzhslrgk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kiurcajw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pdsyzjdo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wmjutmpr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3uoouvfrb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xovqiypj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sfcplgdt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vdnlgezn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3aiobytwz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3igvanyfy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3uyhkeanc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3nrtdcats.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3utnaokwg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbuoocm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kwxbwyez.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qkzqonvp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jkxofjec.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hsdtnaar.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dsgbouto.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcccsen.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sdwjreer.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dmekwyma.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3djgeurls.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3nckzhhhf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gmlgsels.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3novsffsv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ivsvliby.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dirfjpig.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bieelwzs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3atezxzue.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmjzlxez.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pjzweexz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ozekzrhz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdctujh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gnlzlpco.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wshynukz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qahjtqqw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vvwnvicn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gsjxvacq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tokpshwi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3teyfnnzo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rlnodbon.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zuinoomc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3umerocyl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3uvnytfoe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppuuijen.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kgcxkkvf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3icuqovxj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bafsuqsf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ciwffikj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3imbbflhl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xevudskr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3varfqbhg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ebskwohd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ipkutgkf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fdacbdwo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zyqcuoxr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3yvsjkqks.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mtlaawdt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yajcwtke.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kxktxdui.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qdaswgft.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xflemuzz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3uuaoaqjp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qewmiiux.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kgtmvvme.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ukwjgmev.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3haqnfngu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yiibzinx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzxxzljf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3agfxkkzv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3plhxvtwo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gvbllhrh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xjfonuch.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kpwnstor.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ayqqyjpx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3oamtpvky.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3okqdakel.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bckpiuyu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3romaygti.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qednhndp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jbwmrrbq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nbjwdhrn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fkkhxjgd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ubqthdhu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djuzixtp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ofvuvrip.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pecaasol.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3drsrpacl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sfomohjb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3abzhgkle.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ujrfhaxx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vkdhkukw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zcflpwja.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bvandkzi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rmugeimt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3plhoityv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ohmxynfr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mfvhnfxl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vhftsseb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tzsjbofa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkpeqjj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jqyujpkf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fbujxqbl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zekgtbqg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvgfxu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wbiospnz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3etmghrmh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3uljebxto.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pqhmfesz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3batmyhvt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3aurztlvz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xqlqghra.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gomfogyc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jxxazysp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sbxgpstc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rdwxgofq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gjludpjh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rlgsbhze.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kihnsuqm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fohcpgwq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yvuhvmau.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3weaohpza.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxytzgid.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pemihgrm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cyxjrifd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hsqtpwib.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fhwapixr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jlcznjty.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jnamtnen.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3egfhtfef.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3aglgllzf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rjxddulu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ifwtgpmn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3menpqvrz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zyvcddyv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lthqpozr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oxbszisf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cfpahljz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vtkpvyzd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hqwimnxg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3efsugclv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3anlwtyqg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fqxiullf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ihobrgvo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3covmfczg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kzcfqtaq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dgyxwewi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ucqjpvvt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3owysndkv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vkdfbysu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vhvdzzgh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3blpozhzx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3twglcuin.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sivvbnpo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ilsnvgnm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3eopnqhmb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3suogfrre.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3snjukrws.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3aphfnpgy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qirkbroi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uurixbel.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rbsdjsal.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ftzcpvrr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xijhfxlb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ttabezce.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ktbuyvpg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ltkinmta.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ewgeplvc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nujakttl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mardgahe.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jflxdepv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrysvcwr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3veyqpzdn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kmydlfxf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ddtadlen.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bqqrxoia.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqitzsh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vglnmaxq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ixijdors.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pwbsfzqm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3akqhdazj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mxtzjwpk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xrikxkxs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3chfcfzyb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dvtdikvu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bvqnzosb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qrkdblqo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3nfyawprv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3breurmwc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lhabxamw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vckxbpks.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vawnngpq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3plnjckdk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ahwdjmwl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jhpvoebw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3meejvuxy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3roxfwlsy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rkixkeph.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bifhmohw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qfezpnoz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3trkbrmuj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3oxemmbmx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbrzzca.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vbyugumn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qolhvprr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mdsfmbre.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kxdfojqg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mawjtohh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dsnkmzvi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ncmigtys.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mebqafhb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3plaispqg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fuaumcoy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jkgojjjo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3neqoxxnm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vjgkeijc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3didnscfb.html


<!-- 参考信息 -->