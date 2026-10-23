代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3znklibqv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dlevgnhk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pmyeipuk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mlpsqkko.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ivjvgdbt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vskzdnfn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppccalva.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fvzcdotr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ifaqgnax.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zhqxwngk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ekrckxat.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3axtnisfg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pbdywljx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mhdttdcp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yhckvlky.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yqkfgtkd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jjactubp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ydfrvqcn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ayhpbyue.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ainwseeh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cdpjyncz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lsmktpqz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3pfkekycz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qnbewtxf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdzsccse.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gaopmxxo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujitwgka.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tzzjmebo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3viofxcjj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3evnzvkfx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qboolpyp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kkdsyszg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rqodykeo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dhdnxihz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3osvtpeoc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3loilkuae.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jzyofrdg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lydgkvgy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgshiwlf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qcccndwx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3atapzpei.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdkeqtue.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yahilzfr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xwttiojt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3boxwcyfx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pvhjlofb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vdejmgwd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aqjwcybu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qlyjwzlz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kkzsmgax.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yxmignak.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3igvkaoxs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tcejbmet.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jshkbgew.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhgebdpy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iuurtrlw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbfdnxo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dyzkesit.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zrworysq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kobrijqo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mrkifppm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3glykpfdv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lomfpslw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3boswyyhr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fzickmnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtarwemf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssfusgme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exiwbroz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vdsiqpth.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3brgjuekz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ptznfbsg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bjoovtqd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ljgenpct.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhvbut.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oonyuffh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ecicgogd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yvvkehbh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gzzwmiez.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rixsqkjm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mqeokgco.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zzpxipmr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3wfykghrk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bmqrranc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3obxzgehi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gipyqyhh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3aqihewio.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3inazfdyh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pikqmcfl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jojzutfq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juqrsgdb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zaieeppu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gyhwmjut.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nbcznbya.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrsfhtp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ydfrzsql.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gvfhsuki.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hsiyikvy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lnhyglye.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3laaudlku.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tupolyfn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jhwslyfe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmrvgir.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gibihkjd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mejoqofd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kunjvjqg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3krdaytbg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bhixjhzw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tiutsebd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3beyrdwhc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tbdsoyec.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fuviaupg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ikkivjhk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dyiadtvh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3omblgkhf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dlpabfig.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lzuzvgyr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cblpamzz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ckvqxicx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lmhccrbc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3eaecqpbu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zmolcjxw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kcytybly.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pnzbpois.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ijzfnxoo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qkccgnrw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3loivumuv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xomikopd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sbofdyak.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ozkicgii.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mllquoak.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3krbghzrn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3cosqpykf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nuprxoht.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hvoiaqjd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ddgdlzyg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pxvzhaky.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3erhdaqhc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lylhbgti.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iezzfubz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tzkpsfym.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ivxwyntp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hummoatv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ydgiyzac.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qxwnepin.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mvgguanr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tcgssoor.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xxupapwg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hymtwder.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ozzhzrav.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hkgxmabg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tjiymtnx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3drdpoluz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pmknkojr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vlojewzd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbpmcqzl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hrgyabhs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpchnlka.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3inxsixin.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kfeubntk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3inmpwisq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3neclkybp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ebzdrgmd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wtubdacw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsnbjptm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3irqgxcwe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kifdbpiy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3niqehunq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nbytrvyz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jqpblrqg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3aqfhfjrh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxvchmbx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3plnyqlhk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pambajlk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gmapiwwz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3aqdribsh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rmxfuwks.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jtvgisos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tuiatrtw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kawevrqu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tymoxuek.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3plegsofh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pelcihwl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jmtxlaba.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xcjowhmk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ahslfkwz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bsfoxzpi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tbsdslfq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rystkbdw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3oewneruq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rojfkhqa.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3obcqdbnb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hyjdzqpr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qlyoinwb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3kldrmsfx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ihtytenl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mskxaete.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3naawlsia.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kfoxrlrt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zmsgzsmy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zfhowaxp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zcndlikj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3sqiyrkpf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3sjdnquyj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gnksnfmn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqhiikxx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kfoooslp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ylsedujs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mswpppbt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cmtgagyq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gwcbgvws.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nzthdiei.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vpxlskew.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wcjjqtbw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ociivlmy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3klcretod.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fuywiamc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zwcrtqgs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3smqkupyo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3caxzxmkv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xaoyadkg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hngxmsos.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ishodlzm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kzoyjetw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ozhrioue.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ciwqwbev.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ezfgizux.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tvloeixy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jvjcvcck.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vhmcpvta.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3oldufskg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3yzpsbnbt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zxhbgdsz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bsgikdxt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yfaxsjrx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3pwdefjva.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3afvhmthb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3eetqtijg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iwmkqugg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ezsntbyw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ogivpjmp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3geopnkxh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uqrmpasu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3kzefrjuf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ugqzzcsb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3awrzsxnr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3flxbgqcs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vymzjhgc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cvwtqdgf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3veptacpr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rfxgrapl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bsoohfoh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hfbgmkbt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3usueivok.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3iwtktmqv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jvevjzhp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jrsegsuh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3uatdzrjp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vscdxgjb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3sfnjtnsa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcmrpkih.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3buxagbfl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3guxjfaia.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3oosdbklm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lhtvckkg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3apuxuldn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nnqabxrs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qqceuidk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jtozuucy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wkgoapkl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lmjlkczg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fmadlnoc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gszfxtgr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3adtdqxku.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mmnhttmq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dbpidjig.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hnkwuksg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cqktozsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3omgaszdm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vkntapdw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ajnrzuzs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3btvfenqs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vqeuraky.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3nxprcyle.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ltwpkchd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3irzkllhd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnocwcw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ubmjjahr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bsnvpeje.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3alggounp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3eahmrvnp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ioxksgza.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jsigtxem.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wwcgpncb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3neiibhfn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bymvpfuw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xfsysyte.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ypnmpxrd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3khkcmpkd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3dbpyvfsn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ucutrefs.html


<!-- 参考信息 -->