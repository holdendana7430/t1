代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mhfyxkpf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pvwvxwbx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tvoalmik.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hxvfwhek.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ifomhgdi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xdbibcdx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pexdcwxr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2urmgbluq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oqxfhlzb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ozghdcky.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gguwgvvm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ziqlbuop.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uapwvoye.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zvntzwwg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ncbqoqww.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vmdzfwuh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxesiaac.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cvltkwwl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2odsqmkbu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kgrfdjdm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fajmxxdb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kqdhdxra.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mufyphsw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2phcysmsw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2njwjclsx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wreuyeot.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qpfypsok.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxsfkvj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hjlnwdan.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcspzuvv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwvfpyci.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uawgkina.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jjtmmlut.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpahpywj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzfgusfi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nbnwskro.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2oonhnyuf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nfmlzhnw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dlmbuyxs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uwwhqkob.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2onkkwnyj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tqhmhwfd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fzyetllc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lewggtpz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rlwennrb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2btjmfzvv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghynzmym.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cfxbyyeb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nkpclhgh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kbcpiiji.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxieprhq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pxteogsb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lrbltjud.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vxwavgdh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jzhmpqka.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lwmdqqqi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zwtgwadc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atjvmdtc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zsypoimb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfmtxalc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2smzrbosn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hfkzuvst.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ujsbinop.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bitsoxed.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wdvxutuc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vigmhini.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qdnhppad.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2urscpkeu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yuexqvzn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nbpfktll.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ungnyqni.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bcmoyoll.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nlvymiuj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hxhsabnq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ttcdxthy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ttsdvewn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2terbmnra.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yjpobjqx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2iwmxcacd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qlbjkwkc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fjtywgri.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vsrdifvw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ayypmqvn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2awqmbcrv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2guvcggho.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ptuumihm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ptlshypl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dkgtpdev.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xlcjxxdv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rcfuceox.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xwlcwjtp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mqfcxyev.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gjcxxtem.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2orjgcnlj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nzkgbrak.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uqzrxlwv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rctkrxnp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdhlqeb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2atwtvqps.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2neskzsez.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2umxfuxtt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2iklngpqa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vlmseuxf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zlwmbuor.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mhhjxbbw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kkegosyy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2amhxetzf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gnkdokcx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qpptzkcy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2aqjenmaf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2exhsxeol.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ycsmepdm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uuwazqsr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hzdzuvtc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2scwzzyoe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yxcyvcsp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wjsibnqb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lbsmpbpn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2apobviqa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xigeaufp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fwybukiy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kmtonwzl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qhcxgdii.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ttepwnqs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ypshecwl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yosfgjgj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2doagtrgr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2joctqzok.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2boozxqcg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjdxmyf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hztdofas.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qijpvkcz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bpywshkj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ljfoczel.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vioiqyvy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ajuthfnj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nfcxnhsh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2sxsfzjsu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pcmklurf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2icvwqczp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lhgfmhql.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2idcgmtxs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ngcvpzhb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rulavlzv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2iwriznpg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fvvvfxma.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2crzcapnv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bdmdhmki.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dimvgtyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2potmgzlt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uafiekqt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2egieojdr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2iuztbhnl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xiwanqsm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fweysyjo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tuwmcump.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hjobjhhb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xzoetchm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2satrynry.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ixcarwhn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2faauvfvj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ztpiohcs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqplhcuk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zdulnkbm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2nysqbjpt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gclxratz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ebyybuba.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xzpbwmqy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wvvlkklc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hucufelx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lvkbtjqx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vugdsecb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mptabmyl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtcqdung.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wkxwkgdn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xvbifvoh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ugdjgwkw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2biwihtyy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2svcpsvbj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dpspcgus.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ewxggamc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2chxkmbei.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xbcrzgvv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mzpnpqbm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hsvassht.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lstjxvhw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cxqesnzp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2txwhaxrm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jcrypvcc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2teswpfrl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kxrkdxkd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2znldisjp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2catsnhyi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nfqhjbpo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xtwsymuv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uowhrvop.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uwpvylze.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zymxkjhv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qsrlwokl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2eofoxvpu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gqxjbscq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2vockkmsi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dfzosxvs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2aheadohz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2avnjvkpl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cwvaihua.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rdcyejug.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tzbvisco.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vwvlxazq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bxpgyzgb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tlymmpjb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vgptaevj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jscezolq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dhotfgvx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2adhhgnvj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rbfboygp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2knlutrrs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2caidlrjn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lehurntc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kubjpqup.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jtuqszvt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2oalzavsa.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ibajtyrk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uaflmddd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ggpeksik.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dsxpwshi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xbuliwvd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2udijwevk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ptoteblw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kwitkume.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gjkrrvfv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ulfsqffj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kpqqyakn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ayptaypi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vibmozuw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2igjmtblc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2isrpkoyk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vwtubjvc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2toepugat.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmkkprq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lsjicizt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pjthsupc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2agbczqit.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2segbzstw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gwesjvqy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pnhvmimy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zcwikcyn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2baksqgfa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2utgrelnh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gpxkszlh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bfxldhtc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hetozccs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nbpxvzeg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lwolpvra.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pjrucicl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hshtcpyw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ferituxy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bgpcpbdn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2izaxokbf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ujyesavw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zqbbirap.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ztifldsd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iojbgtvg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2bevoqaci.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hpvommup.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jnurrtmo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2iuuuflio.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2evmzoeke.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2psgkdkwt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yxrbemzt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kswusuji.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ptwfzsgk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cqqhccbl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpsuhqp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2biddzaro.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qobhstfk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uuyjxojz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iimhshev.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pmlrapqb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ynhyvdud.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ecibdzul.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qfknzigi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ezmgnkyb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iqwgnlam.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ucohscfn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yyzctdhl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ialdopfs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2obodvmdh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ymqiyria.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dusjptja.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2iirhbhxi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyhyfcrb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vtkkqdmw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2aalnaqhb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mwaoyvhz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dxtlwrbc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pmqeeyyb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hztjayxu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zheplxwy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xhddmcfy.html


<!-- 参考信息 -->