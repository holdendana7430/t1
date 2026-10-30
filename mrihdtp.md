代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gxvrsnpsr.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/ggelhhaxq.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/grllimfup.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gcietuqcf.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gkioyrwqr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gevttqlur.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gdrkjaucl.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gntsygitm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ganfgvqyr.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gjsljgrsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/glavntdom.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/ghxzbwktr.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/grfmtkkpr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/grugtkqzs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gsmbzrqit.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gxflvwkai.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gtszjcprf.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gvwbrycwk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/glmnlbsua.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gkefnkibi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/giucdtsqf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grdivxujd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghawehpvo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxjylmuco.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gubfsrzrg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gctawjcaa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gugywjcte.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gpvjwwbqo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gqrwwqfsg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/grzaqykub.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/guqkceznt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gdjsxfqir.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gocuoyito.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gkjeatfgk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gcugyowsc.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gfizrfrgc.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gscletcrn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gqlczkfpd.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gkfbptghd.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gjmqtobtl.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gpcwpzkzr.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gzyjavppl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gntakcpli.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gekhgpoko.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gsxoexiip.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/grvlfajam.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gucvhjxrz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gnvaraici.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gpfvsyvgw.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gjozzldsw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gnekzszwb.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gvsoddwzu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gsmcgdpex.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gvrihymln.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ggbzqpcjb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gcapzvfbd.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gaiebyrjz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gprhezvoc.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gjlwajyao.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/ghcjqypgl.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gautgnsvt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gvwdyiedc.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/ggesyscmo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/golndwxiw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gnibkhemx.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/grjtuapet.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gknuaqnso.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gbxrqydlg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gtlwffxia.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/galyfcoqw.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/ghrtwuoox.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkpokdvdq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gwdrvfkpz.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gqafuaday.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gfqqphtsx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/glmnvietf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ggfedbypg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gzytfhtea.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gkirctfct.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gmqdilerv.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gzafiemor.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gmqxlncgq.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/guondbrjf.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gqivtnvqr.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gbnvkwvgu.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gawhwsuhf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gwhgatqjf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/ghtsbxbdg.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/ggzkbcmwl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gsxbexplb.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gmocykpvr.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gquyzhvgm.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gpygzjdxz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gureodnkd.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/ghraejdcm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gyjqxhvrp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gogyapakj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gsnjuegil.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gatdfkgrc.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gafhclngh.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gznixtync.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gsaweaszf.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gguqfkrqr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gobnvupql.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gigbxvajl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gbrtenigf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/ghctlzygt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gnwzmkkzb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gqfaffhsy.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gyfhkyumu.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gmimeeaqq.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gwwnijvnk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gouinkttt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/giiuassej.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gmegnxuzh.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/grupnikra.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gfbmxzbml.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/getkegqbh.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/garsqthvx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gruyltfjt.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gnvmxfuqq.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/grwrplnpn.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gkbxdwmrs.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/giuykebhp.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gujfwpsrp.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gptrsoree.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gmulrgwit.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gyyptlbfd.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gmcwircyc.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/giarlmbnc.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gbalwucuq.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gonxmkerp.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gkzfhnrop.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gvahaamdm.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gvvfezrbl.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gkunsnuma.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbenlpiul.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gxilolofd.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gkdfbxorn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gytldsoya.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gyauynicx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gkscumiri.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gfqbzglnn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/grwipppqj.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gpvlorfvu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gwipyjhym.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gajtszbfn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gntukuubb.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gofjapqcv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gcpbwokwz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/glvuoriry.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/grsfeepnp.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gjcwsfbsb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gerwczkiw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gqlsmbast.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gccnfpxca.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/guehnbbzu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/ggpvwogra.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gqskfkvbf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gqlbhylqw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gozvxuadn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gxhfpkbvo.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/ggayeppgt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gxkzjhafi.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gqeoqaups.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gmhadewgt.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gqhbubjii.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gfmxwobom.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gjsootaxo.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/geanillat.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gembqzrik.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gikfqvxfm.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gpjdilpxp.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gpkhtsjec.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gyvxghrht.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gvuskdeps.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gfcqfxuuv.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gwsvqwclh.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gkjkhggri.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gxfoduwga.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/grifdhiiy.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gtdjfurex.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gktgxvjmf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gvrvxkqoj.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/grlrwbvyh.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gtkvtelxv.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gqzgdtgrr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gmonxsipw.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gfviuasko.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gfdiyheok.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gfqiflsxq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gwqjqqrsz.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gnsdflmez.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gcvgaxqpg.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/giocbyvbd.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/ghexjfxxj.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gyaezralp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gvwnpmpja.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gdgntthpz.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gxmqtyecg.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/giklgjrcm.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/giyasxoag.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gtgfuxbfv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gacjxixdt.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gikuhkpnx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gjduoauoz.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhqxncz.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtrfnidtq.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gmtprmfjd.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gzjhslqux.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gegcreugt.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/ghjboimoi.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/grqtnzrhd.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gxdwqwlhy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gmhaocaly.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gjgrouwcg.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/glzzixygd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqrgtbyos.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gdlvsjvrg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gacrhzyvo.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/ghiioimct.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gqhymwrqg.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gfntcbdzb.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/geomlgofk.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gjrdzfsfe.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gcrykrmxj.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gjpykebxj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gvsgdcbru.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gejaerijk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gjmgqhvrf.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gobspzszr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gofvqhnqo.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/giwfodffs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gxvedhihz.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/glbswxufd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gryitcitg.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gqnvhoray.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/grnudqjpt.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gxcfjhqhs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gsxufezpg.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gzfhdnoeu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gnhlmtwkz.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gythvpape.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/govdtfkiv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/ggjubhulx.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gfdgzfiog.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gfjnopffk.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzobdooha.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gzlrghipm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gibkkxufn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/ghhoiadct.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gptegjrcy.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gpzsjnxbc.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gqmtyhwzy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gqdiaomjx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gcwuiteko.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gvkizzizn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gjcxkvovp.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gtfuodhgb.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gppzyjwbn.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gblkefbfe.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gyzezncsj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gehpabzcp.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/galycmhum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilybqteb.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gtgkjrzhy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvipwnrkc.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gvdjufwsq.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gwyqacaha.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gsvwsprld.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gaxqcxvlg.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gjunnmzje.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gclomvpgk.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gjchtvcwo.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/ggntbaywo.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/goxdckrdr.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/ghbtlbvnj.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gircpevkt.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gybmphnji.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gsyrgugny.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gzjmkvdyw.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gwaqhkgcw.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/glufnimhz.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gyhsxuxqc.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/govwrzifu.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gedapbsqi.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gatknhphu.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gbeogtgcr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gfpnmynvc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gbxujteuz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gesexjwjw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/ggxvighrd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gvpzegapc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/grqoditxb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gimxnhrcj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gzuflcsup.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxvcvcumr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gxbkefamc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gvoczsbqs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkqgydpwp.sHtML


<!-- 参考信息 -->