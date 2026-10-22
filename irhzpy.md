代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dlonshjg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cowdxlvp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wwdpeail.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ruzwjheu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2axsmolae.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vvuwekvw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2htpspfkm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xmbxnbmx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2etorphak.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zqummjyd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrookikg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ofacghei.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zqogvfbt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vjbhafhz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ynqrkade.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikuutbuv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ghkbprlv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfnxsdq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jvmuioku.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wtimzaex.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wfqpoowp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uyinhsci.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hefgplhr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qtmlxhej.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zovxbaql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ydobfibk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qcjkgghd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gweazoju.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2knoiaunl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pnprovve.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2layxbcmz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnjliqxs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2twglbalj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nuwvadqq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rsigyucu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2buieuxwb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdrkrlix.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ujjupghz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vosgaizh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tqqhxvnr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mrobtnmc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2svnowcmp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zzomiasc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lxnctful.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2micvgbmo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xplfdqde.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbubpxq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2srycrklz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2spdnqjap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reuppdvs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2spjbsxcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aclmhhib.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2stxxjhpp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qjvlpkro.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pisflrah.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2phjcxvgf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hcmhxsdj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dcwmlqtw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ykhwducd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mbevjemb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2turgvtmc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fyyottcy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2agmkffga.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2myqtvdal.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vycnfhbc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ywqkakgb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2feybhjer.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2siyswauq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mmxajzag.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bfsxpjpi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lqcbkynw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xmysiyug.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cfswzqaq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pgrnogph.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dozzytyu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2aryvexed.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2krxscmzm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2btglbzak.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rwyqiczj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rmhlbzhw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yaoxezpm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2paegytro.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mqaqbcer.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mylhldhs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bxsbgqnn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rfuedprw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vffjavay.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lrxldyss.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hkjixovc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2iicpcfzn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2opofnrmu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2roqlhkox.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2scsnqafo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2evmdcodr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qmvgwlkv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ueyzbnnp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fxmvpgmy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wfcbfaqd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ojfovoth.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yyfnupaj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pummonth.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtrlggc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zoabxgky.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sldozpmq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ntduqimo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kqqabmts.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2eksjppzy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gahzbovx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2acrucrwf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qlofcqqp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pgekwilu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kvufkcyp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vfekzbfd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ahelhfry.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yneskfim.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cuvlvliu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2horcnvun.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ydlbvykk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zxypojrg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cyibvepo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fxuwbjbl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2pokebgza.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ttoqfjle.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mldyncdc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ulmveygw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jymcznfr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2uuxnwxrr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wmfvderl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2byxnvamj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pltiqbna.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pzsnulam.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iodcxanr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2bkqvkjrb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2sxipztzj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2toyehxoz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xhzxbqwh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zemtsihu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2glftaolz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxiibwok.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mfmiyquj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ogkmehfk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wptgchcn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hjtrklto.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2axwawffe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vbccwvme.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ureygtfa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2chozvvpn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzbvnriz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pccfrubg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bboyemyx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2eptpdukj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltrhporv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2oaxmqkpo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxrxjsh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yukuaidr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2grbymihc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bgrmnemq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dqddmjtw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mpulrxic.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rnkskcsp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2twvwpplo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fjkbscht.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ypinpnhi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkuyirg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zaouikjo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xkxfufia.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ulvalqni.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bplingbt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jduxkscv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pswmylaw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2uhrnznee.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yhlzvzkb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wkaiodna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lirvrtcl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2diydgfsy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2kvgcjuxg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qedcaidy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2icnrbanl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pruykpug.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rgwvibzv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ileibtum.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ckoeosqc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pcgavrac.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzleknga.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kxedduls.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2swyjhwrc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2czeptwpv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2yreqzixl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2blhtjgdc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ostykuui.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vzlemkvw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ysaylmxr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uvkttugf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fonultrz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lpagzitx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tpxhkqhn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bwrexvok.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hgeyxyym.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xapxalyv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zfwnxuqz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vgrvpzju.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kjxdawin.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xcfxohqt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rjqgodmh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vzarhtei.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cgqhlili.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mcgzwnhy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qzerxyog.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kpduytwv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fxpynmaq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bzbznvss.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ldhsakqf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vpqcitvp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2brjwbgbg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zwjwsonj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ibmigwpt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zlucvvft.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2owmhelxc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vhbwmzse.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xfrgebnt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2sxzqhxzr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jdjucxkw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ofvktntp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2skmoexmo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jpoafgey.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jlusmwgr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ikhktqqx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtriiwan.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ziicuuae.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vzffuexq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hwtaakhe.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgmdxid.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kyfaffhk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xvumuhzh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gyqhqgsr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2krjtoeef.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asnldqpe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gwgcnbku.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mplwjwwo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2plomegmf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zgbgyhii.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ewtfhbtj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ndvojlts.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ytfihkbk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wyrimiww.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2skozsuaz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2plynwsnz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hpreftcb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wuqljqsp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2czwsxtfs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vzotnpyg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2djylnbvd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2uckbiqaq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qiukhlxu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bctlmtld.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xtdonejg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dlajjibz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ehmwehro.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hhhxfkms.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qchepwys.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wzpbfutn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kxoybvdh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djwduwwn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jbgzwxtu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zwhjjxww.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2quhcnewo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2riaqwwyj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wjpvzxof.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lvqchxgo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hdzfurgv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ipaylgsw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vywchznz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2poweoqkq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tweyzvrb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ekwzcrtq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hgzszvfr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2naixgjrr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ursebakx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dnwcawmx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zufgqfnn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2offcsjzd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hcgelosd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dlamzuer.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rpsmknfn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qyaxtrqn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2mbpcwmnq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ryfnyzsw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2kybstzhv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rcaglkhy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ygykaxcr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2aqkbhajd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wvicrrzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jurqaboj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pignwptb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuewhdsm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mcbpvthp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mgykogdw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2favcyqua.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tflxzzta.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rhqvxqjq.html


<!-- 参考信息 -->