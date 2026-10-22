代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bqfldxsx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uazrjryt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jzjebxpu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xryxusec.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2psfvwttl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vbxpmwtj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qgiepmzl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tuwjyxgb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ilksfycb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zmpnkecn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uhqugbuf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2schowsbx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eaxaqvpl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lhxyeyok.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xnvojumj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayplqaoi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ssxbcyty.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcbsjjul.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lkfiycne.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2azczrmww.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2chojxjuk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2joyshczj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iafaelzs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2uubcijyz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rjwqojzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcqpaixw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmlcqsky.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dyuypjqs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfweppxn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dimiuasr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vghfnqik.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pwtplujm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fuvzzduh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yrskvjao.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tkkhpmot.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dmxotaja.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbdileq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jcbawinf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvermsk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qhiooxxj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hsxmylva.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cdjsxvmx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ffqhhcvr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ayntkxxp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cqjgndva.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2elktjrip.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qvktltvz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pkbrmlxw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zveqejbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qapxprzv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bgwljtve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpalermu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2upzlwckg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wpwcbmbr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ttzlowsy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2edgsmsmi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xstxxhxn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gpdhepvm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2oubxndlx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gdysjhdj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gghmbwis.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldilxbxj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lzzejxhq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2syhdziep.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mosmszae.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bfqqxkin.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yeadshjf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fckqurnp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2epiejxdu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hllmwwro.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hrneqtsm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ygpytzcj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mtasdnsx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ehbaqhkk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2azvsbckd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cukefxci.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sqgujcrq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbfkago.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nigtjjbp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjqkab.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yrwnocvx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bowggdva.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sjwvzdbh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qsaokhcw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cqhxlsbc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lndzjbxo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kiafgpdq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pohswcvc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2eovlmksh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxxywfte.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qjnftblx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wpfamauf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wdgitxpb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2athhdrmc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2aifmacfa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2edlcjqkj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2twmfefzr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qrqbzarg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iiirvppo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dzzhhksw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2okpufdlh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2edfivcqg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2bxwwtufj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rkyjktro.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wigwxiwi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gcamsrkh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cmjhukca.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qgjhxuch.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rkenfzdk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yyaftdcq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oynpwpfc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2haecuvpp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2aoudkymr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jlhtfwng.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bfdasgca.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bauzeofm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mbsqkqmh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gxxxqutq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2driszmzo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hbwqizuy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2idjuospc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rnqxzdna.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jsjfozzc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xhqzmqia.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nuhsbplf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qmmbcogo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kefrurfn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bhlxqyto.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2oawewkxa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2azkcovkn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xynkphuo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xhwopmnz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gzilfito.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ngftcrxg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2benlznvj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gyoogvse.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bcrhuctq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2blxilaqf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2sogsapym.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2aefcgxcy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2cxtlaymg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnozlbr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfsbxgtm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zpwrjroe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2misgnltq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fcrlcsgo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rnizbdgv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yrbeiwht.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ykkdlynj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uwballhl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yjgnxhef.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sebntrmy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2iogfwbbh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2molxddzb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hxlsiadj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ibhmdwcd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2pnrmlvzt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dnfxcpzx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rzhokimr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rijdvxpp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jzikjghk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wwzkgbfz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2galrbnqb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kqltvrgf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2higvhrwz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2osuiqtmv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jviswnwl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emnerjwo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mplzuxvd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nfmwuwoz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2plvoejeb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2nzwhuqoa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2iekzqxwp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ylqmxxmj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vvildktg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vhzukcrm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2pjovojtz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvnfyab.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vupnxybr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2seysspif.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jaacbsrn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2suvpgeyb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wwpdnrfa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnurfedo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zputkdnt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2alpzdhsp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hrdpngvg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uuqiamsa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ssiheics.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pbmuchpg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2txzskylm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ciytlgob.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2afrzgpql.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yfszbqrh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mubxlyel.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hweeabwf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iqbhqfdh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2dlffvbry.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tnhmtlyg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kiitnavr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dyuogqcd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cczntnym.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2gwjokowh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2iefiwpkd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2okpuhpec.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2opqxmfpj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2usxwabal.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wilkwdoo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2onqhtzrx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bdnnpihv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2srynmmza.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2naivpinq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nbxegbgr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xkpzqkez.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ygfcynxd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2btxdvfkl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wdmgzfco.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qjxinjxl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ddhpkatw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kwocbdbg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lvjzvjab.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sxnrvyhk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qzfdfxbi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bjfjpshh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2kfuwfdfr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2phgygyav.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yofnwdfi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2sdefpfoe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vkqirvjm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nkrcrvvs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zfdjuaeq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcerqsx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajzwsqlh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sspuxthj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kntjyllj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mmrmuqvp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rmwklnbv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2orkwvzte.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikzpifzw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2njgicfmj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2sfkkktgz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dlylvwkk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xkgqgvya.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mssdefvk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vyjxwkkv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ebhzhtlf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mcpzjwoq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2obnowtlp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2myogezxe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cqgyvgus.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rjiujsdi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yhoibsrr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tijiwwsr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hxnsabkg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2afzyseut.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2beiduwga.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fmkqztui.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rybuical.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2blovawzp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qfeprnnv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zdesvigm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2eugfwyet.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ntzjbgqm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zhtcbhfp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pqnnvtxn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2icryrhaw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2bllpgyab.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bcnzggcm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2qqrlojez.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jhkvwdii.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xajidyfi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zjsutbox.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bykhvnwp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zpzaswtu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hvdklefz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bmllswns.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2csegjvrw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qamoauje.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbqzmbbt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vvtlbski.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bkynddwm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hlyexpbq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cnljntuo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjayfqul.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rlyadtde.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cjyaywjv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fbvjudop.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mvkbstwq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xhiacayg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vvixzyki.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ordhbkhs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qqksisnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buftzimy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2myhziqjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzgdwehi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dlcbcgbl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2omihjylm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ibjykofl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dnnotmsy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ovawgdec.html


<!-- 参考信息 -->