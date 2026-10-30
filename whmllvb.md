代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmmughsbo.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtoxvornu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gbcaywons.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gfenitrjg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqmeuscv.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjktbhud.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcxxglns.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykydeack.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/ghoddjnrt.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsvctoli.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvwffjvug.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjalnbwo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehblxgbu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcctuhoh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyofbxih.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gugqzsjek.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuudxjkg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlsrsept.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhlyfdn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpaonpbkg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gweparugv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gperswlul.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gldifpngz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/goyrohtci.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gsnivlnot.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gtvnpefrq.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvozanqdc.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/glgndkklj.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwkxupjn.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gdbdbstgh.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gegezqszc.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/glbkxezzg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqbxewdy.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfowxfjj.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/goutrtqzr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/ginaxpoms.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtafpbvya.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/grwerevyj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gaazrrpvw.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ganmoszjr.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gztbbmplz.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfmqczja.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gvpegsocl.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcijvfkck.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/guifnphbz.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gtvjegrwa.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagtllsoh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/geypwknae.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmirnidc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcaqyagm.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gltxupaca.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzrzaock.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlpxmpvf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glziywpxd.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gobhdmqxr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbxjnhns.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrolymky.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gcgsbtfkj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqtcamvd.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhqcrcwt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcblwcud.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gjvcgsxql.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzglnkxh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwyfwhvu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjbsuoxa.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqwrqdp.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzswiszr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxtsndnx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlpsqyre.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsllzxlf.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gcvxyxsin.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzwlwtzu.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuxwhaxo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwnwvtcl.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gcinyrhdl.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gpsqpvbhg.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrpzcyjc.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/golnkptuq.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkpemvzi.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcpkprnp.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gedfisdzf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxrzfnhi.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gsomelrph.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gsglahqma.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctnspeet.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ggganfxxj.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gpmuxpsea.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdhkncaj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsycrotfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggusjeczo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjjvyftrx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzcqjzmc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gxtitgriq.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmanlfgmq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gngehtulm.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmdtrjki.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gobgbwyrt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gxquxnhny.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbzfrnun.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybwbroyp.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwrmbxgs.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyvoariy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvscaiiks.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gavczqsgp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gcocamlct.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gittdnnsv.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gcazarwcm.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gwzgxpayn.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/girtprkbg.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqsymqyj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxbtxosr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaylmxhcv.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtbvoab.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqgvjnle.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gqezzxuyh.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gaulddjfl.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmysavvk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggljlksmb.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhlxkntx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrfsuzux.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzgwuluh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlgstrer.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gfnfirtcg.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gurfewafl.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gblubexap.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkinpjmg.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvizuzizi.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvpkmdpjz.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/grhksarlx.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqcbxkqho.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/grtflitam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gygokdvgq.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhgjmjsj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gexifkacu.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gzutnflwt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gbuuoiwmt.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtzyjphq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxumbthqn.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gknveertg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfswpzdpc.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gcudzeagx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/ggfrteord.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/goybjzwxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gypkvlueh.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gywsdpmyk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gveuluzlh.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gilzfyzho.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsotzwgqv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqgrfhdq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/glnopakrs.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxmmdvlg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gatmsfzxu.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtynfoutp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaxczyyj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyzaibte.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucjbgqtz.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gulwctvbe.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcyaizvc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gasqbjdvb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxedlota.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmqveptg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwduhkcx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpovehhbb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gdgevlpne.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeaxojbm.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyvmmtrd.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/glnuspwde.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhkezrtv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gehwekgrs.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwktdnq.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gatjpghnj.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gynsaxreu.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganwtcryn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giywxdcim.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjquoqga.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gatjvpqqb.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gwrpnrtnq.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gmddcpmrq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goidennhm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gamfrvezn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkfolbsh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzugggxs.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gcymsjfql.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthjifkxv.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhenjkur.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/grefjaxfr.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixokkxt.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxailleei.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnggorjet.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfarmnt.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gvknksbgp.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gjhipdlxs.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gdgzdobbk.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gfffinnif.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtzpvhwe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobmrnzfm.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfiazawii.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkghfeos.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gcxftaaht.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gczprktlu.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbzoqtavg.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gjubdskfe.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/guafcjqsa.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gitleqdmt.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gkfavgdzx.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/grybbpmjv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfubzielb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbcilyfw.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/guhtqbazd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gymceoecx.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvuazquda.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdyktutp.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyhqtchz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlovqbdx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzgzyjui.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmyentxo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyizepjey.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqsyuduu.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwduuse.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsruyozrc.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gerywrnoz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdriieap.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmjnvrim.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/grjmgyifo.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gyuftesed.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhauqjfk.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gyikukoza.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpknyirxv.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/grpblwonk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuhaiblw.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqkdylmk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gubaztess.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqhutiy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkxssmup.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnltcrdt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkdiknur.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gtaecyuhg.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gonvmouhg.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gbmmgmfsa.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gfpqtgkoj.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gsoobcekk.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtcqxcu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gptqloqbt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevlfqnf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfcgiswv.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gisiszexd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcnxdscc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpphmvdah.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnmokuzx.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gufsxqyxc.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gfwvgmutx.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gyiypxwun.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gftttrpfg.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcckyyyuo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzbxwmic.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gaugjainf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmlltbwe.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcealgxe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggmgrpjco.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gzvlfbkph.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gcptakwwr.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ggveosvqc.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gdcilarbb.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gwniljyff.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gurhxvuto.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gyenwpsfl.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvuyscwhj.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gavkbtnwa.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gugobfqiz.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gbifwhwji.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwtowiab.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbpvdtkc.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gcsuwpxle.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gcviqwjbs.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifxafcsa.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gxzmwikhh.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gcdlznrro.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyyobenq.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gsraufycs.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxobvajk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gefqstvsx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/grqtkmuwv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkhhzsyb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbbjvpqc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywdaopem.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gbwaejkho.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiefjcbk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gwiuprtvw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesooqdpi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoqxmciw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gsvwwuqjo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gnjprjjiq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqozaagja.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gnmsqhgsg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgetvaar.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gonwmcudp.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/guvkvziip.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gljfabtnu.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkjunjns.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/guhfjwhma.sHtML


<!-- 参考信息 -->