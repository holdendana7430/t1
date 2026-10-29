代发 wailian999

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gxeqjydvj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gepjfdwtv.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gbtfnvznu.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gmcfaafrr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gcerficbo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gaumkmwpj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gwadwmzdf.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gtdbxermm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gacorisxo.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gpkhrhxuz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gwjowdini.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gkgtlcftq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gckqyarsz.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gxzodagap.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gbzvhpxvw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/glbbevlhk.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gruxwtatz.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqixwtfw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gvmxrpptp.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gihzozaop.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gdoqofipq.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gvwyoqdjf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gcovgxqtv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/girsryaos.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gbevdmbjt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gdfmsnepv.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gkwswclfl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gdshfhwiq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/giimrkjmn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/ggqkiyjps.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gntqlxwio.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gsirtlrbh.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gazvrhtxn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gilnhzsnq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gvtllyneu.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gdraivaej.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gtqbjczxp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gtjwygpvh.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gbknopfkz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gjwhyuize.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gzfeydinl.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gkjgpxacg.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gwvqqmbnm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/grdmhmmmq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/ggtoejpqe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gzjnghrtz.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gbeuotxmi.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gocjosxaq.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gnfbpdled.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/glhwhdgdp.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gcsnmykju.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/glfpkjfez.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/guirbeeft.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gzpqthrdn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gpjiajfjm.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gydrkbnwd.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gmhfftwix.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gbgtzcpdp.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gxojgtrca.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/ganrbetnw.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gwmelrusw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gmbekdbqg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gqyawkfnf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gmxcsockj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/ggfgdwocl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gowkgtgas.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqbtgthlv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gijrfyzkm.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/grixqazkd.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gixptywiz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gnjdyzcds.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gnmqjxtvn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gmunksgwk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gsbwztwbh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/godsrgjvk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gxrzlopcs.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gvcfpzvmw.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gotkclgci.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gvqxycpkb.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gwedusldb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gqkhegvka.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gnzhiaxpg.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gziidnxln.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gdvvlpfsk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/ghcxlrroc.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gccgbyqml.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gkttwjtkg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gwedaqjhk.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/ggnenvbbq.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gwpqflnku.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gmapephpu.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gdppxlbih.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gftvkuvta.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/ggolaoufa.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gypywspvf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gjntbcurm.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gbzetnbch.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/geymdwbnu.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gplqcmhbt.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gxyrnmcju.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/glzneurkr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gcrjvrcdv.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gzbfhegrk.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gfkhdkhap.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gliycdbbx.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/ggrmtzdga.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gyobqcjqm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtuvioox.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gwxfnwdeh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gflkrxlqr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gvcinyelr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gcrupoxla.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gmojmpbji.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gfegknwig.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/grdnsyyzg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gudxsapie.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gceyvpedm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gnssimemm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gniftlvft.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/goxagfjmn.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gcmbqcasr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gyvjnyrjd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gfopbgbes.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gguxayylw.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gtcpibqiv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gryknoahg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gymapzify.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gdnvsrwgg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gmrtakvxj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gstblydsq.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gdkqspfnz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gzxnsaidv.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gpbyztmro.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gqqnbavdm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gsqvluugq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/grjuqpnhz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gubzxdquo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gpqobgayo.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/grspgoudd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gmlixwweu.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gigxmyzyg.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gxkhsmpib.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gitxxgvlo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gnkptjaul.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gombgtxnj.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/ghfijhlke.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gqfjxmcor.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/grkksdzuk.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/grtgdgtlc.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/guyguiadm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gaednqand.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gyvsfdccp.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/geeajeqpy.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gcijfwmtz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/ghiuturwr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gomagiwjm.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gliyzhibn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gjwcqrjoq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gyxstodcw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gkigepmcc.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gyumowssg.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gngwclnbr.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gjsgtmsbe.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gsmriujqq.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gzdrxpzbl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gpxlbuxqc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gxjituwln.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gkhbqvmep.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/garqddkcj.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/grffkdpmx.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gdldbjipi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/glxgiunkf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gfctysbpm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gxmxhnxlv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gbehzsxaz.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gzddqntoz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/guyikufgt.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gpgazihtg.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gnxtnfsqp.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gtmmnhukk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gpvxjqncb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gtefqnemc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gsnoxanfo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ggprlugys.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gteuqwtec.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gqszwabif.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gadecogqz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gqdrbcowe.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gidqlufig.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gztrsxxjs.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/ggjcfetbp.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/ggktggjun.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/glcbwhvov.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gqbttcclq.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gcldwepwa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gfevxepei.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/ggnynycma.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gdblhaaql.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gqbtamcks.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gjtdbreto.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/guggmmbrn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/ggfholwmj.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gpfburdvt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gmcangqbm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/glyacrqza.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gyfmkxjue.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/giehpsydp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gmazyshkw.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gubtsaeol.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gmuwahyeo.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gkookgeky.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgqrapx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gdujuipba.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gogaueorr.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/guhvgrwjs.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gffxiesks.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gtcpualed.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbksxefjf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gswnduvmm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gbomnxomd.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gccgodghr.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gywcyudia.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gqoaheoze.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gipnodujk.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gqevzrrml.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gmkqnjukc.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gvgafkmpg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gkkvmiaro.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gljxyjikp.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gecvnhscu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gyicdslus.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gwzgxyapz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaoaaorss.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gmzjxkoov.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcvtlssau.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gbvpicasj.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gfyfmrrjg.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gsjgatqho.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gmrwkflsz.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gupnxwpnw.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gbzanouki.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gmorvfjki.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gjiezycbu.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gxtcpypgx.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/ghtzhhyvz.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/griavkrdd.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gmuhvruqu.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/grpyfpguv.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gcmmeqgaw.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gmxnqjcgo.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gmzxhskqi.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gxgcrppyu.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gxdlwodgp.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gqxyxnvyz.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/ggtmvhkxx.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gqrwuqthm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gfxebwxgw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gbieoktvy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxjpdmeyu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gyrwotgsm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/ghxhlqtol.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/ggjbsthqy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gogrycanf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gnqeoucbu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gydubisez.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gpqzoayhy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqpjegmei.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gayonyuwy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glktxpxgu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gczwjyult.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gtjidhhku.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gaclzewzh.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gjlusbrtr.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gbuivlnig.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gemvicvth.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gyjloweat.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gxeltivvi.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gbanxnuwd.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gsifrsymw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghiaggzdn.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gqynujlqy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gnhgmvuqv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gzbwapvzn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gglucpoiz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/guonjpxnz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gmltjkzea.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gespssbkf.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gpzwqourg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gngmaquor.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gpfzlgkjq.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/ghzwffnga.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbcjalarh.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gndzupxjr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/goynrlbxs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gaajjkemh.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gxfriqezs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gusitbqze.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gagvpqusz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gisjsvmql.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gsdcnojsy.sHtML


<!-- 参考信息 -->