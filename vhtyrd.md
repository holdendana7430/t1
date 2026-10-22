代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nvqjehjz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fcncchka.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2houafzje.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hqarpxtv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ysnzguqj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jhfyiqhl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tledbqer.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dbyuyapa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aurhjnbp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xbldtuzq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qrglasso.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zhayeigi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ivuxhoco.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pncdimiv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqbapfrj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oulniejg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sghbnpdx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tgceyqsf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2texqzyoc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpswfygg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zepvxlni.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2clqhvpsw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2eefmouno.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tgdafagy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jxaxpeib.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2povfoumw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dmzzjzgq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2iwrsrnyx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cktsglqv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntrnsehi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdvucmo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2otnreudx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlhkrhoo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jaepzgeh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2keswzjcr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2blzdbypn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzyttqko.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nqcpkbek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ppqupomw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2htkopuro.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2glhqzqcr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2smbmkgwi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjjwauho.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nyktsqcy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dgisnypj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vqiqrcoz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pdhexdbk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2cwnthaok.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jpswjgst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqrhqxdh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2apsxsglv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnsnxpaa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xnniqdwo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2oosnhkul.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mqxncumo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dtdamkra.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2phgvvudo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2haqxlzyb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mmqsinou.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2khlhfogj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2isiksaku.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ixjyvoce.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yorrwlxc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ofpmxivu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2awgpxwpc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xrjmnghs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2csbpuzpm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qykzjqth.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dfmqtpuf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdsqgzo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2uuobeqyr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2iayfewqj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ujgqytpf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jjylazsg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2kvzgvqom.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pidcebnm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tswmybra.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2yaoraiib.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xdyxnawd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqpphxe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nfmxliac.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vnwqucus.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mteklrdm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sjecnyms.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qebjmppm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhmwrez.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mnsazfch.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bzphpiwi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rbngfyui.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqzpefog.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2butvuwsy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ssmibffg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rvovcmhe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2koogdnrg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2juasoatr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ufrjpnrh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqrmynzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hwdbkpui.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qkpymwkf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ygzxjkti.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2lzinmkty.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lpasdkxt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fsseauno.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2afjphngu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kpvnqolc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2andjvdxx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mrnphxrs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ektrpgno.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jbfmtihl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2oagbdczp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dikznnow.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2flzhdqov.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nquzmmnj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2cjfydgmr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jbuilwik.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xbjytonp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xitytcyl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hnttrwpp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sfspolam.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2embwcybh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zucnbfal.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2iqutxuam.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2cvrodbkl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqwcmnq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fmijqcsb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hnyujsac.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mfzvhvbw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dmhoomdj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nirsbbiq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wbzuvllh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2efvjrzcw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lddznvvr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jzgwwcpm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2afvnmcbb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2axnjcpnz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2boduxxye.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2npuqxefj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2todkoniu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2lvcxovnv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nmpihkuo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ucwcebvz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nanknmjm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckbkzmkw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2axiqgtkf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2smytands.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gpdiatyr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fbczdabj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvlcvzwx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lstioviu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2seccmiwb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2rohvbmby.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azopzrdr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2khglmvgp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mvrvampm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wdobublk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qzzabldk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qrujcxpj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ueohryir.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2raqoajik.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fpchsfdy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lcloewhn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2onscrxrg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ithnnkhz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vozptzbo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aoobivsi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fvwxvdiy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2oxhzlgdv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jggzlyej.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zforsifu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukesrffi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gkznwqmm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bynpnugl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xszptjkd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ouhehxgg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2slnqapwk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vdyqmgtn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2thlkakcs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zlxsdalt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qnsezqrw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tbytxmpl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pdijdbde.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fztugcal.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2auvpvdie.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lutxfpng.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2iocknvql.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2luoafqdo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vdoqyxix.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2iepicwfx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rhasybng.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zjemqpsi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cjtrrwpg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lnadyznd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yojlpcyl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ldhkbeat.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2drdumyiy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dlfdktlz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mcwkbtag.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tjtedpph.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jyakbwlr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ieimpfwc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fmpjuvvp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fgvajclu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rvvjjedq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gvzzpthr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zrnkjoci.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2titqbhyg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fyxsgslb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2clwbihwr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hrnkjanl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sbnfjscb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2efqbjhfu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cmmrvbwb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sofyiljj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2rexsdqku.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2iaciyrmz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrovxptj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2coldmzrs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uegdxepl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bzvknpuk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ojkrkvdw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2eyxtgjfx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ociybwyu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dqhennaz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rpmvyttc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xobszpsy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pvoqpota.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qjahspyj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wgptqxrc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ghphajyt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cpnjuijg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nqsbgzya.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xllgbmqj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2veadgbkj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2sikvluah.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ogqjgnhw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvdgnhbe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wbsmjlyv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mpnpffco.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tnhleywj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iqybgvea.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hurkbvqm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dmjkwpqp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wtrdgknx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ijeqcebm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rarcmdxy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zsjlkijk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qvsoiiwi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ljkkapyx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2psvzrcju.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xowvansu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2sxdpzhkr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2prdegjkj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jsrvebzq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dyhimfoz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2btyrjllm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hkkukjfj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ghaoudpn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ddxfslyg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oidcxoev.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hvoojwqx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qlsihaup.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dlszfjax.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2muuupkgc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2yezoszap.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2elfviffz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fgarsbuq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ngpovspk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fvhouplb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jaelrjbg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rlbumhzh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2scozwdpu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gakirnyz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cosdstch.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2okrcpdfg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kwckrpca.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpzoaipx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aevlvdcx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fmanacza.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jbgwdvjh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmygszn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rynaaazb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vvjfvwvd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bgnecwat.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cacdoyou.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hdzuohud.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bdzcpphy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nnurcmda.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2sfzvmyoj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gbmpdkqu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2fokagkcr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xyqlsvwx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2tytvdfyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvvkntxj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ipsktouy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziznqoun.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2upyttbuf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yqmvwjpw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qbiqhdci.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gtgwycyo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gpmgbnle.html


<!-- 参考信息 -->