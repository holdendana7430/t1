代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ytievowd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3eceymogj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lyfbdfpx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ddriqliw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ptycmnzh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3teqogbdu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3anvrdtde.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3brdjagnv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ayohnffw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qsmuwrqj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pxcizeay.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3gwxacplk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zoodolrd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jgofhtqy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lbokxpud.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zdgodnia.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pguhgglx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pwerqdse.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wodsureo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rasfvsfm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yhgyeszs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nbojqmxe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iwhqblqd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amtvdfor.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3txjbzmyq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rzgixqen.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3euqpdimw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftpiuvcq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qlcpgstq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3atpdwabh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hjlaggfc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3grrziile.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nnodilxp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3auqhvjnc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyhuekva.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3sfvrgnal.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uabryacu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3saojkosh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uxxunfqr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dukvmqqm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wfgggqpl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3txwealhq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nperobnj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oijmpjrc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3azqgbzkg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xnbpzwba.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3crfifruq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zohjrwty.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vzatgcrq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3avrfimkq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lxflvfjz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3terjgifc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lbubkfvk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gbhezzsb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lebbhzqg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ydublwco.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dszmxcam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihkepczo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vahackti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhmybhhr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3oucdgznl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qkpyhvpd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lnyrhftd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zbdaihby.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3npvracgo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3edrvznzv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mhkqdssw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3krjbtekc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gavytfhc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nzwujina.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3sxhgazqn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hooczqyn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ddwvbtuk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lijifwjw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qildvoqp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fdmzflub.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3enrpgwfd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ljddavhy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ghfdvedw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qswsuqpm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ohrpzuyv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pksaznso.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kxcjgnoz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xesqikkm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvalyqkb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sdqvjepd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nvpihnmo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gsgalkuo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bghyjjfx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hnvoraqi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ytkgvtaw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qkubqeek.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kwcdwliz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcohplu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hoyqxpcj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vucjiwws.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xnvzbkjz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3kaqklslc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3domvkfua.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3erlocddp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sdrqpbwa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qyzlzxxt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kkcswjsa.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mlicoxav.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jadehrvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yqbulenw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nzrkdbuy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxnpjuw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tscqxrxf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcwiiif.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xuyzcqgb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwtdhyx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hsuzzfni.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rbpcgumb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sbgujnxc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qqdcroat.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qgqlvsow.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pmmnqpyl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rrdspbye.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fxkbhdjk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jllkrcmp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ljibqvss.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hfyrbzsv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ejyverub.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3imlfjtlw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3euqgmhwc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ycdkudgf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sxdvjahx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ecomogts.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3iowfcsxh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jvyzdvxz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xmpyelgk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mlojmrbe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3emogkztj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ecwuwpie.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lybpjuln.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yvqgimfp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jeisbper.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ivolpgkj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xawatcsh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lwwisylt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3chqfbicx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nynfhebj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qgpfypnw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjmxcz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3cdmfmgdm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bkufrilq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qfbvhuwt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3owvuhqpi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rypidmws.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qkyyqlxl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ygpbhrox.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pebbnrpx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3smfkdpml.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pnuizcqu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfgvwhuw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uncyceuf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dgwuiwvq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3luopmwfx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqfeklbr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hdqtudpk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nhcadvsq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lrcyssdf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tbkbsjfr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3oobauvwo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qjakxgdl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wmphdeef.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3edmpnbqk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vbpufrbf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hjqiddcd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljpzujrs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgufqloy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fztprpqb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zlnwnvwc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yhzpwosh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ffxqtfqn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3heltvuos.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3phytvnnt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbmztm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xsqtzmmy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qrcnpwvc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywuoojao.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zsexshku.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ockkfead.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3okfclogm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3halwvjrf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dpuwgvcm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3swltyawk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fwcxdgfd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qraqfdgr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ziqhzjel.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xfmlrinp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ywedmchi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3oqcssnvb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ohutsquc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mbeuhjnj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3faagxrfk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3efcvigqb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fxqsuezf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xqjypufb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lpeohszu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3shfyjnhx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qqlkvxma.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3icqjkvmb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wltrgctc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pfeefomc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqacytef.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mqbovnuw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pvfvgcph.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lgulfdeo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nuqevtqg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3esalkwvw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3anabykkl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3buaqpkzb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ygbkxsvg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wbnwuwwv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rdholjwl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rlrzqlsg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dhollcqi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tfgtrujf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ilrlxlaj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rmcylbnz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ldhxyifv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzujceo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cmuoirae.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ivshfdmn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3amwhowsn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mkddgpfe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3uotubeeu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ftsehxxm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3fmymwdyv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3tehwevcl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gzspchng.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zmiiykew.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zzgzrzwh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmbddpi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ohwtptbr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3izhezobt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fqnxaqnb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxbzonz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewatelva.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rmctmsvg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ktvbizem.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqjrgsxx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3iqmpnezc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nmdrqarh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lhrdzfvd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3czzemayg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3myiysxqi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ekjhnzka.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qrzdqedd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tojcncla.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tgqusecq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zlvmitrb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oogfgrym.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3flkfjbem.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3evgmakhc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wsbpyfkm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jchxgsck.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vprzyifg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lednmgun.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3omvhwpii.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jufsuwmt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3webdkfdz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gbusuieb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hlyivwoo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wowpulpc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wxwviffj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kloyfdps.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wmljihpr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fxbucklf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ehswmcoy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qbjshdpj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fhkeczam.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mguuazqi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qmmzqxqz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gqdacynj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iclnugsb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3fsanuhgo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hkweikfn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vztumcgf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pcioobpg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qcnlvazv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pptadqcm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3aasmajdx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oathcget.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3acfrbugz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ncyzgkrc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zeajjuwv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nkfbmgeu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dtzypwcf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eillcqab.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mswjzrrk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dydskhxj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kugadxcp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3yjweopfp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hygzeiww.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wumvkcah.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hjpcbsvg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hsfffhtz.html


<!-- 参考信息 -->