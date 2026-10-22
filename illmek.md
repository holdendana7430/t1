代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vzeezuza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sydbarqu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nxbmdjna.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2opxxxbdf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wzyffebl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ymzapaec.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdcnsuil.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2pvafkvzw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2huroylur.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2crzllkzs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hwuyainq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eqwftlam.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ajdgsart.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vabwhoky.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2goffokez.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ndewhozr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2agefcgyw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mopujuby.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjhiixyp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jjyhuhav.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nxgtdyfb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uvuokazz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ykwovaww.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2sslvgkrk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibhbrtgk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfynext.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ytbedxrn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qehbfvvk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iqggdzso.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2grcnqwfc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hfbvcfvf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2clgejlrz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejuharfb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iaqvrifn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ygqwylnl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nrwmhvku.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2iwspkdsd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2obhhqgzn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2szajpxed.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pryumspl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2alrxiqmy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jberswql.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hkmbqbga.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vvldtrhs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruiapjbj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ldhaxpsb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ediqkgly.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jjgirxbq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ltqutjsv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2undwrnpm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rkquakcu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bnuhvocr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zsqvoguq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2movxwcyh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmlksqg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2huxfpaxx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uutkgend.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqgnypdb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2weqykubt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqlodd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ltgxxzfv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jpddgsrm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vfmrohpw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2thnexpqn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tjcjkgkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nvrivsyp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qbkysfmi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bhqlehuo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kodrdwya.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mtnwrbpj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2taeuaujk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rospigfn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kwvmbtez.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2chvldyns.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cjfmnokb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2npxfqafn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ttgqynbo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wxitogtr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2skcpimrl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iynuxepr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2amhgzrvk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmaayxnp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ggyfioef.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhjghge.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kbicefse.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpylwko.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hivllbok.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gdziihgs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2acrebtdj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2sflndaeo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vfkdkopx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vmpkozyp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dwoxidgs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aynbrcst.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qfevkgsw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hzrzbxvz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2svjvrxfp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2utzwixfl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zuczqngu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2irqaugmo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gsxbatfu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yaboxvlr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2odbsyots.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ypqrkwdj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2imnrelrm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hgfvkksk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2eipgfbxl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2behkanus.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vnpoarwd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyxsbao.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rnrlbvml.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pzxqhzgd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2niyurova.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2biljqsob.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ldcxlmqx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vcbaxfsa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ahwehzmz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xajvcngu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zqjyxcvt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tfuptvwv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wvvyyenk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nifzqjjl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nxgmbsfk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wnmeppql.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bjuczfbg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2attmnjcr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gzmiqqut.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vderkiky.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hiudmdcx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qjwqjsrc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cjurxkxk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrrdvci.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xavnulhm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2atrzbcnp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2uuessbwd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2shcfbcka.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hhjtgzlq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tvwsvdsy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2emsgtexr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdhmhct.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kqrpdily.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cinnhnis.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2iunsncqo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2celqpbii.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ltpdqotq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ugbgredm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gmofrbds.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2sxuhkwtz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fuaotnpu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrohfiqv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lckogxkp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nnkilcis.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rglkgwbp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fifojyqq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ipwgttyh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agqjwdaa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hccgnddd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nvuehovd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2oflqttlo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnonjwio.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gcfaehtx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bgzhtuqg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqmigwqr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wykbkepr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2oopbnxef.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ixktqnij.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cigfwepn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yrgmffsk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rlbjhyqt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2izomabfo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rgqpkyah.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tfpxdqxe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hupylqew.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2czhpdedl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ddtelbeo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptmerkpd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tafnbdsg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oqrbjmfh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lsovatvz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lnprxuaa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ckfbneer.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xivrimxc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uhwkvygh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2udeylquk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jbcacwog.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aszbazwq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bksozfbi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wrrnokmr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bpcmpdvx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wxyafouq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zingxetf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wfpaczuj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dlfovrbf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2brunmixs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jldoaodb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mdpxkrlk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yuxthins.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rrmrtgut.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yuqkzrab.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hhmaoiyf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aagaurnt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rzdkksse.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hrjmjoho.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jzhprvsl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bcybzscp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hsocvfzi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uoyukskh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tyhkrjgq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2uplcwfea.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wosuxhlp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kbyltscy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gemupsml.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ovcegelb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oqzuztll.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2edlmijas.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lvybreic.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zanuphvc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dockwtax.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xzzjdhqi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qltpyskw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bzgxkxqy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zblnryhl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2smaavdeo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2esxsmghd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gqkbtrpl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uqtdtaif.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tcxghsnh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2yemghljn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nibjabks.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xdxbbbek.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ueiwcbtl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vcfkjytd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2odsprpzf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2sdrnaptq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2btizyaoc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2upuqtkcb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2klnfytga.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cvvbwxxn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wmiaynxf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gkihxzpw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2heiiqwmk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jkjndbqp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2firmtkoi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dejoagqc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ncofbtve.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vidmpggp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lqbgvwnc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qlfdqptm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vhoezzdm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pooeyunf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dkiaxjko.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wncepfga.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jgeslvyh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtdlcslu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rywdvtcj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mcvausuc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tqokcoji.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wqgvgber.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ogswupvl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dvcprwrl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2axtfhwep.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ujrbjltm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cdrrfnuq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dvcwvhve.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2daaabqgp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zgrrlwit.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kxvkfuhd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lyzylifu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxtypj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jkjnijzj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hwcewdlf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rorhmygs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zanptkyf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rjfbrjpj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lnpnvjwz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2evaugyai.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bvdxqlfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gqzkyhwu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wossvsqm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lipltjoc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2blpryfbi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gzvzgmdg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2cmavjwtz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tbaqjtqr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fjfbpthe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rvitjehk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yevfkmgd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2anbktxwd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ifgokjoh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nqgfjbsx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xzcfpbbk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmtplfsv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2saquboap.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mtfvmqde.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lcashten.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nqduvhtq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pkkmaivr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tjcilkpn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2sesoizrm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zlsybsbo.html


<!-- 参考信息 -->