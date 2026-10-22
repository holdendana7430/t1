代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fwvcxbsj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoljtmuj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hwlmoywo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ignjmfyy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iatlcyip.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nmeprdao.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xpwycyzh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nlaytrbr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jkzzvhbs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gcmowqaz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ljcxlxuy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nrrxwcbh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkvitdwc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2riwbfukv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oofazowk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yhfxvicl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvsheqvt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2luscxxxq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iviappqa.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lwugeiti.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imghnorq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wktrqrfu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tkvhqfge.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hmlyhkos.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdnqhgv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eeyjhfsg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gngvjlsy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2moadfmaj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fwkudjmp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jzhrtypq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpgwmic.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kcqxxrlo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ygracbpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2finpwuin.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2evhwzkvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhfjatfx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ubvlvqkg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2spxmvkvy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rfyrccby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2adzlbrma.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vmdlkrki.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pumbuqyp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nkxcvdvo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ijflttfy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bglyujto.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jowkasql.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ghlzeyhq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2yvdjlpqd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2abfadcdm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2umohgapj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iialtxlm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ghlwexko.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tkffifcg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2woarhwgs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zvfkpckx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gwlwfola.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cysyzoic.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpgpegvs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xygyfwub.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wprqcrrw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mjghpdnb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2geyaswco.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2oewrowqg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfmcmfv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2eisiqkra.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2taptouil.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xwgogtkh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ngbxksje.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gpadhzvg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rirymykn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2lzffepdh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jqosmuna.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vriddwxf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncrvsfvh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ihjktqka.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wwypmqns.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rsxudghy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2djflfqxi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wjmzcymu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2bjiwfklx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2glidrycj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ckzzasfm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nidrurgq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wncutgqk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jhcrtsvx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zzypjodf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vbbibyyt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dayunknm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tvpsgjdj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2emwnbcke.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2afetjbkd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ylpzamqd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xjdlpwuz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fxybmgqk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hakdntqq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fzzjbltk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kvykwyxs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2budjxmak.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xlyjgqkr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zxsvlizs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fkvqwusq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jzxjuqpt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lmwkjuno.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2aewmnzvq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uwdzvenf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yzqnewle.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fgnbwmxw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zydmbwwv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pwybvrxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yffsvgox.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ivkuqjqq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pxekkuqu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cuyateln.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2volptuug.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pmfqykay.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nzxfrxxn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2azsclact.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2saolllld.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2owmzplib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2etniprnv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2irahlrax.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sjdegyqu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhmbpcax.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhfawvcp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fowoefkh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2atzblhsx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lzovvejn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dqleivtd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2feylgmnn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kbmsygmd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2afoewwqh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbqcuaes.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2sqxviepo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ysyrrdoz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bxqgszgu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irrdkcib.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zwgixefv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cqwpnzgx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjfyrhqz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wqhkxuyg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gmrnuxrh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vnqvjruf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ktrfzgio.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2veqfvwlu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fxkvybzz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vhlkqpej.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvstgwaq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2obhtbhla.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qwvgguod.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mfeyvkns.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jmbpogee.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uajysenz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xkphehyn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dyhzfuaz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ophtunjs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nsqclmnw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2khgybepb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxpghhwp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lnipzhnk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gknkgtjh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bluacokf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tbdcfuck.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hokebwpy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2irxzjcth.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nvhsasng.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vyomdyem.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vdcvhiqd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2frwswchu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fmfvkofe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fhtlahyu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2odaqivbf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jnlbhrbj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mextrrzk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gpdnnutp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2myjbzzzi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mlxpgrnu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jlorqrto.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2snmcnekh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pwcfpazc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pzmidzbk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2osfzduqj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2wevhhypn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qglwpoxs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hicrfuaq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rgteswoq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dnqyqafd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rsquyypg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mnyqxgzk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lsulxibm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uyqblxgb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ltvcijqu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zlenarzq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ziwbqqbw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2znqkinks.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ffsxjoxg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2smsrbfwo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2duuxtojo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ctulqonm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jkwyhhen.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pulbkdmy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vbvdequq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uomjfzws.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2aqasrisd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zffzirat.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ktstrnmo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hshapfjl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nkmejnsg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2sljirotq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2haxehzsb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2geheyqlc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2axxyjern.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qybautrd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ibifsdwq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wbrnqnho.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pegwddkx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhcodts.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2txvncsaa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bjkxkjsi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ojsibyhl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hxopleza.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dogoztsq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ldbndocw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbycyqfj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tzuyasrd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2aogpraxn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qiytmhor.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vujbbeqz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rfkgetpv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pjapdvae.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mlxbvrpt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xanncuvu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zwxcpeko.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rxuugjfo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xcjftpud.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bdkvlxxi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2tvisyezo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rxupkoiz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dvwrgien.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kwjillyl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fhhyiucs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dtohwlhc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lgfptjbi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dgedspcf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iuhvranm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2uzzbgvtc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kojutshd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aothlqwf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kagblilu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2osdrpfgy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjqorjf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2oucgalqa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2endxebda.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2inuxhqyi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uyanlmwg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nwpspipd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2fbwnsgox.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hzaduffl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2mwkingcr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rtgheavn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bfeuovel.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2iribhvtg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wzpoavtw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ckicgmlh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cwtpyqeu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2llgffvzw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jxdmshvf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2bxmqzjzf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhxsimil.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lagqcuwe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yuhqbhnu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2droijazl.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bcahqqqv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2flescbhk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xoillxnt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wjuchipi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yrnucyiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmitzocd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2iwschrlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ollccpoq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2pvxrrnvm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hzshjnig.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fufxfbwd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zrxbppbd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vrcrsqfq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jomvxjca.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eefrbsoj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hwugrxag.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sbecncdz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vndyjnjc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cijgfpqm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qgpmlaal.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vpareyja.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gtdsokmu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2apiumwmg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bfrlkqiz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zzipmqws.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vcfdizds.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bngimdiv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2pekaszfa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qdbqlkwg.html


<!-- 参考信息 -->