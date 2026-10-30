代发 wailian999

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqwvqjwv.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gnkctdmjp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkzxwdzq.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/giqkpmwvi.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/goemtwvcv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gnjlerlpe.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwcvfybs.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gozigovxz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/ghvpvanwn.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsznbkmb.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzxwdpl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/grlfubrdt.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/grjxjvoei.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmgnxjspy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzggtelfy.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgplxuqi.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfruqrxsh.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicywrhzz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzqqggix.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gdsdxknnq.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/guqrgxogl.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggihbsgmh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmnorrvw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjuijrbn.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gsbsiisgy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxwynjoh.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gzviajiah.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gykfaortb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gfttvgucq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgezuhgy.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gyekqzktp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhbwxykn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gampgtrqt.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsfylqtd.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpecavix.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqauuna.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guirybxvq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwhgqczgh.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gvvpksnpy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gtcvtirnc.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gjnnzbssk.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazqakdyp.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/grmlsnrqm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrzljghx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/ghhptqhgg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesktkwis.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsjodque.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghggkhaxk.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuadwnzs.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/givgtgcnf.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmtklmts.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfrhrdz.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/ghidjiiqu.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/geenhxtwp.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvjrmrkkr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gdevzjzfl.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gnthsyaxw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/grlukzspw.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gffgkpwrq.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfysvgzgv.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gayvuoona.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhgnhtsg.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpokjutm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/glizdextt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzoycgt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gxgevxlan.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemkfbjby.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/giumedobq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjfkgjny.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gukqfwbsq.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gfpjwispz.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcatwrbd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/godjabjzn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqkigrq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gzrhwotfg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhcuqoan.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmneeiqzo.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gfiaxhnkf.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxessdsoe.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gocpwbjim.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gywlyohte.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gopzkaxvv.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcaobhdvp.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrclhmmb.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbrughwor.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjpvncyd.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyfylomfh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozjggkrv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnztdtgmq.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gnecvjsjw.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gfsjbdxlu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfnlxvvg.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gblaozlvn.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/goxnnujfv.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpsazgkv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/ggubhqjta.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gfucleclr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjpwqdxe.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftbtjjp.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbecerh.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqraeplmh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqgbuqwo.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbciavqbe.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gctwheqmc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gurcgilfs.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggvvyccro.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsdjjcvm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grytwhejg.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbjxvsyeb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimnmjwtt.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gnfeqprpy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/glrymvfkw.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gorrxqweq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gverabtcz.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymyrhowl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwfvanty.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyhcnltq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcjoyfep.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxpmxlrnp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gvvdfplka.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/grdkppivu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiylptkb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehifaefg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gecjzwzuy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/glkitznyr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjxcpjit.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcvlhgod.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/grsozdhva.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuuqyuxq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/glqdqnkde.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqtjkqfsl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gerqljypn.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlfjwvwh.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcetchxjs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gputxvbsb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtfxtvo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdogtbicr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/ggstedsxf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghebmktkw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/geoeskkhl.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/geujtxkxd.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/grzndrncq.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gmzjemvlt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gfjhqszaw.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/ggdkajpuc.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gdtbjmvgp.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gldlcyjdv.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gujjvjlyp.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngckaxja.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbmfbcaw.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gucxjmvtv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gbrzqthwm.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbekdsgou.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhbangkm.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/grytwzytm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdhuctnf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxrcanhz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/geizfgwch.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgolotdr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gnpubhvwt.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/glkgnezbb.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gblzpgocr.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/goxyehoik.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwjqxna.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gamgnnywd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gurxpajcv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gerywrmcf.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvcheooy.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuittfib.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gwffmxkwe.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaolypwyd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrytmyob.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrhvpbo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfxgjulh.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gpcgflnqy.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnzhyocm.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxoqfsizt.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gtjcplbom.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsertchbh.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtifortia.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/glsxtazfd.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/goesfqujm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gwipjvuhi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gokafphtp.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwctdrqu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/ggzwogovv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtszdxrn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjciknegj.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gnsfdgjpa.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gudiaestr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdopkqkhx.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gbtuatane.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxmixulj.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gisktarmo.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/giloqdkku.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gxaarxsdr.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gvwpakbyf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/ghloyhoqx.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/ghiqatzex.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggpqxmwdm.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gvhuosknf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/giezbbgkx.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeqaswhi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsmikwkp.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gtquigupd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntvqmcio.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzqetcjy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gylibtojm.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gzdtitbfv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/genuyfdei.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxvabob.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/giwdtyjag.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gqxfrnqyl.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gofgbmejz.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbxnijfz.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjppqbpvn.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/ghuligiwb.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gliwtauku.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkbkmyqt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gzxgbkbag.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gogfburri.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gpzezudqe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gyuhfgmgd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ginnyvnki.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gxswgtjhm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghybgmwi.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gaodukuxx.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gnsvybpgj.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gsadppxte.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gqzglcuav.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsikbzmul.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/ganutbnsu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjpdmkdz.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gvwxyixll.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggjvwyrhl.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/girnfwmws.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gxpmoidex.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbjlzpom.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrlmbhlv.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvypile.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylyznqfr.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqeflbqj.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gdqjvmqwu.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gjzugpkve.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gtroqfatu.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzmvcdzk.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwlpinxy.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/ginelhaoz.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/giihvgxvf.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmkfeuej.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gjjzjldlv.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gziepfncy.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gcbamctpe.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzbyhlov.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gwccfgmhz.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gicxugbvl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfhypchj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gcbefrlxl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gnorctqrf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqspaxis.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/ghknylose.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gkervktyt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gydckwxzp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuwesyar.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftjedipy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjbsqngt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrpfffpi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gsolrmlgy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/geiwnlbuy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/goqikqwic.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrgjunan.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gunzexydd.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqozhtu.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjaruuhh.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gguatcxui.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gkhckqqoz.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyfecghq.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/glhlrkpod.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gaygmivrw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqxxfsbks.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghibbkppv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdhaocu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gogtmqxcy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gpstisdig.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gtodbdfvl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gwtwlksay.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiciesgb.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelugjyw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gobmdpcsr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqtqrab.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gonzjqetd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gduaivgal.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/ggpknyibs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gwweefobh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlvtebnu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoauhvqd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gbriqqnrw.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrbstbxd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdafsrtwo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/gpdgocnul.sHtML


<!-- 参考信息 -->