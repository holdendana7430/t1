代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2clweqdrs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qcmxfvtn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dasmrcus.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rqxhfgmt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fnleuhuc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fkipqnfw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hnorargs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nkxnylzp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qvuzlaol.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nqeizqwm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gdutinoc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2iipvbguz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ckanpebw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fsscptxi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ippvmxpc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2peffnooe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ckdqqvzm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2osdwntlj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbggtxok.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tsmwsznv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwgmdnfc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iagnpvbm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhmpytup.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qnhultdo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zntmcowm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ymjzlljc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2coxichvk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qanrcluw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fqeulkvl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wmboshdk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eeqtthbb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ilvamkvk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wilkfvsu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dlgosplp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xqxsagtc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2stlcymkg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2njdewhqj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rlggdgiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2spgojbbd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ynkfcxfa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ewwxkmap.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dorixzfg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lkqbzwzy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bvtaquhc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2krcsdefy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkcwwmgu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xstejjpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apgrvbuy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ybmviurx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wdimcwjr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2odemzmro.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hoswrrqt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2geylvuyr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lymrabsw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2caatrkpv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pngwqpxn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ijwiyeot.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2geyzclyl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2yikdapys.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cdmulitu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ojlytves.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2btcdtvvd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hfqleqio.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2enlidbvf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qyvvklmk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwbzzkl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wiqlkjlx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2frtfusch.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2evwuozcp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2aogspybe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qjxowfkt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2snrhkxco.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2olyhmpvz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoqczvx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2opbwesng.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vankbqvg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cdfzmdan.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2teywjljz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2aquryrqb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2esytvyrf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ipkpakcv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2eefnshlu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jdnwnnhg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zbockhdq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rfnschfr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjezcgeo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rwmnljkk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rowhpmqe.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fjyvmvmk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uewckawa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2iivfojne.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qcnznakp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2biycvdzw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eidsddxk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lbigbtbp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sudyshoj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tkwbcnxt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fmdjnjzg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lszgzfce.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2guznzzek.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uomkbeoc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pzaaisdx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2irokcckk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ekwomjth.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2awaodqxh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yeyyvhnl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vhvckkfk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kkocsaum.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gvahrksa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ltimsmye.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2uinyxuet.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tqbdxdoc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dxyqvgav.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hywwsbbx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wtzpbljj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcysyuy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nrvfnuhg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jrddcuai.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gaqlmnih.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kqlpefrr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zwsxdmwd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2uxkeclgd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wnurceag.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zghiyjuv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qsuxdkji.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ijrmheic.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hkcxlaht.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pzipptgr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rgfiqxds.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tmlawjin.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bwozflmi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhelzhg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bfhihyrf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2buvfmcpp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvcfstii.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ccqovaia.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ftyqjtjt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fneaprir.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfypssfd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjsipo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gvabdcvp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2szmrtpaw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ekeuyjsy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oamgcrok.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2raibsvzb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vmatlyei.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yqdznemt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vbnenxqu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rxvsgxzq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xlxshuui.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwvglejb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hnskxhnn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2religemd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gynhpkyk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ptfzlabg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gfgchqxh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2acxzcqyj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ornfavaq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dfsergvp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdsgzeo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yornrxph.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mdwgcxbn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ngnkyyqm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bhqvdntm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hihbakns.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ecwfnnrj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2afunrgwy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yzaykjvk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tgjnupuc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hufoiuiz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2svsrfahb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ewyvpiho.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xqsfbdvy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mimdazdm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mkejjmfl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2buobhknr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ywgguaac.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vhrgzeyi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2aconsghr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qcvhzhxi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wsjfxlhe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pryjuggo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wpghqxzl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tyixlmds.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cvufknia.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zmeorraa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qgwbikyc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sayefbkd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cnntmpap.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ygktpgwa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2eicpidgx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lowqfveo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sehribdv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jxdgmybz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2piinzqro.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ofdbfrun.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ybphdfem.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pzmytehj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ljcuwrqa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2galhccqn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2chybuttc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nfjkmjop.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2aqeosjmm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2igoyeidg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hybwqovj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xbzyflax.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qdlwnspf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rwjmfeak.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2szplpydw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bzemtiqm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dngifkkz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qfanfzhp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2srpjbknp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oyyfqbqz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vdpxsefn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ohbpfhug.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vgbxjmvo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qiclxhsc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2juzffwly.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ktdmucdc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fgryzjia.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dbceitsq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pebbpsxg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qccbsrot.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2texpogfk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yaqyvlwj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zttpwmvm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhsardeb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2csppzqdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wxyummbo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qefrrkwp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cpdobzaj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2vdkloenp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lvryzabh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2osmpbwpn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2njwoofwr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uztkdwpo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gfqlxsyy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lwnvwkrj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhufdje.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bgtscgoo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gtxxwqih.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jurrtwhb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rzwnshcw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kzworzpe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pcqwdrap.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2isnjoioa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cryaexsn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fdklvyvx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2upkmehol.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ncrnlden.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jiklapgu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hyjstgsx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mdoxpdge.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xkgetbnq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ghlmyvtk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2sbpqskdm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tumxuugu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jskwpvjr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2aorkabax.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aqxcetgi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iifzpltr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cczjdzny.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dabkyasx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yajohqbe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2optsutas.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xbnqqwfi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2exiupdcl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vttejyem.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yoezpdoq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ofsdttgq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rmzwdegx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zwqfsnvh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wxtfratn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rxgmidwx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zdipqlsv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mpgagxij.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tgnccvuh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tqllhmvv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umvqrthi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fmypvtyz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ifmaljuj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zsurpsph.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2tecixhpj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qtewkrft.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pkiyjbyu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2webxgnmn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vncqhcxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrodxorv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yeyvsfsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2synhtrbs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ypyrwlel.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ddgwrnxl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dzlbksoe.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gkurxxir.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cavfhctz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rzfojfvi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2squtmibs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2giljotlf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2myrmycki.html


<!-- 参考信息 -->