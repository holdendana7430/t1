代发 wailian999

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gkclalulx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/girqnjiay.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gmhmjmcba.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/ghdgnyivq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/grgiomufn.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpdnrdkbp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqsxwnhpa.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gwjqjtrud.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gmwtxczqu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/granwuioe.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gxlaiyrzy.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gnmemoche.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gtcjxrpza.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gcuvqwmjm.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gxsnweydk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gptlexirj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gddidzrzd.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gezmtbtbb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gltcxvnhr.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gaoucyntj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gkfpekcxs.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gxwnrwxij.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gmugapmis.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gdoywcdqk.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gurgcbjtr.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gytsqryxv.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gpzkqfrmt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/glwrbdlae.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gqjnpujyh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtddqdwq.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/glzlmadjx.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gicxfnyjv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/goawcuusm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gwnkgmzri.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gopgchebf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gxaghwqfy.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gkryuxhvo.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gxaxvbyng.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gqbivliqj.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gsvjhbdod.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gfngrcaxj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gpevvmbfb.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gafufvzfn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/grvpafjxw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gusihqhds.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gihtfeckc.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gmhnsuwwe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gdjywloez.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/ggrqwjpeo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gwbjdmrco.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gnkihjfau.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gexwyokxx.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gfcdpkwqu.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gudtbevuz.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gpztxoosc.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gdledahrw.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gtteiyolr.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/ggqqaswig.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gmgqaiwiw.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gvicnkhli.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gaheevuho.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ghkdjdfwh.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gbtdpyxxx.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gfvargaly.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gwkhidjgq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gbxvyqrrx.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gvabpoklw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gldfedpky.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gmanesvfs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/golmnocvc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gyceqyupf.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/ghtiurarl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/guqiidbmd.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gccxiomni.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gpanywrfq.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ghcroelrg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gvyloswdk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gkytxyjke.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gurejraxf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gpdyvyjlm.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gjdxtdjtf.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gxswkqpoj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gcxhalenx.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gxutmwqmb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gapyrtplm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gbsakmdmo.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gekgilsss.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/glcpxlshr.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gkfimubof.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/ggfhtufam.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gruqvgpwx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyddpnydw.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gyrfvmuku.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gokjreomc.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/groysadgn.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gowpvijju.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/ghbzwgpgd.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gdmttsxip.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gimolhcqf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gpnnetdzx.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gehebcxia.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gppsessdn.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gjejifzbk.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gqvdyhpdz.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gbokbgpyy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/grmuhuwbf.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gvztejglj.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gcbdbjphz.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkeqstlez.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gsfahslyw.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gqzlllbbp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gokgipjfp.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gtizaadie.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gletsumdt.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gkxvbrvek.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gpmiwadsv.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gvualqeud.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gkzzrdbuu.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gsnlrnbvb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gutkoqjiz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/goszfzrxg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/glqjfkuxt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gzicwexhn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gizeuwlrs.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gtkgvvwui.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfxsvbkih.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gqpvydgxa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/guvvtntdj.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gpqnwoxmm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gfitgivkm.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gfmmoyvmd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gblskoexu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gauihjyoj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gggcbbcgy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gzlrkimmu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gigzbyfvl.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gbeblonwb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/glkfbbeox.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/geagzadir.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gbbxkjdrx.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gjvmgmzck.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gsgmwhtjz.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/glvrvvnpg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/glwqvcuhw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gbmkmstmy.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gozmrmdpc.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gewxzyurz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gexpkycxx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gnznyzxoz.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gabkcqxwr.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gokrqyfwo.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gpgxqmuaw.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gyxtobugp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gnnxhqwgi.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gblbfsiot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gtkliialk.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gsrbbvstk.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gbbctlwwj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/ghkhphoen.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gyaxarycl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gkerluonl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/geswfzyqw.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/ghlsfhhkx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gmbyiguqt.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gcxgxfxyh.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gnoeufpco.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gmkrimesg.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/ggefenkop.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gturpzwtw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gabjxmicy.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gccpptfis.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gjilqzqjm.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gashxohzy.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gyhoqdapo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gmiopggrq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gnnffznow.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gzlcatuot.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/ggfhudkns.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/grgfyzvps.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gzloehfoe.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/guodhacda.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/grfzddjqu.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gyohobgqe.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gwagxorlk.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gcjkehesv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gdujwxvnn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gegqngflk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gedzifkjg.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/genvyimpa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gjmskksmq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gdfjhepaw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gononqwlu.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gadycennd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gkpkhvozv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gyftkhzuu.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gcpvotakn.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gjzvfzfgt.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gslkcnzoy.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gpyfcosxn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gogfwmkig.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gkzsdsoqp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gweixplik.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gxvyvtuzh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gmbmzoosb.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gbrnzuerm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gfpniegzq.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggskqrvmd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gfpgionsc.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gbssmghrn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gzljijqpj.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gvworudhw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gvqhdrjnr.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gsrvuzmtn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/giznjhufo.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gtfregerj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/geywlyaax.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/geihgqwww.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gxssnfyau.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gdpftquhu.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gelnjxndh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gasffkilt.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxxgvgoya.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gaxmwyxjl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/glnjngcoz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gpygxaahp.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/grjyqzqca.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gieeovkds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gmhjqtsuu.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gduhogwso.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gureoiccu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gsqgzcxmw.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/guowjjcqb.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/glwcgphgu.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/ghfxbsebe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gudqercca.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gjjaqpcke.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guocggpxn.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/grtfjqthf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glbryjdhb.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gvogkqcrk.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gjfqievaa.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gwmrnrpmr.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/glwlnemue.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gsmaiarib.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ggqsizwad.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gmzfjamwd.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gsltltaoz.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gnjcazzqz.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gamkmlipg.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gsljssujr.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gersrhotk.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/ghcjsrndu.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gwtemalnx.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gyjdqdefy.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gayrjtpeu.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gdbdoaxrs.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gznmxrisg.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gyuesafdq.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gyjataudc.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/ghumbuchk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gppyyaemn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gnffyvxwf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gkwfwtdkr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gfudzakoz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gojlyvxwh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gvtcapezq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/guqfvchyv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gjvtuitfx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqlcnrwoi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxdrxszwx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gqjetssqg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gwegmzrhc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxdbtcvlk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gamsbmkho.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gwmlmmuyp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gksjqutun.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gbleshrkm.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gjgrkhwoo.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gagcqupya.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gtiscalqf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gwkvzrjbh.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqvrnzcaz.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gdztlzgyx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqtaflxnq.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gvqihjgtq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gfkwdzvwi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gvlzrjjry.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gmkupuede.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/giencxfou.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/ghylyfarc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/guaywivtg.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/ggzeslwhe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbzdcbywx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gzbqtgkmg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/ghiooqijz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkjmlocyz.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gzlfgzbfk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gkwncsvup.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gzphvcslx.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gnhiprmtx.sHtML


<!-- 参考信息 -->