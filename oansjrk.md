代发 wailian999

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gfemcwfhs.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/guqmjzfld.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gyynlbtqr.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gfxtntrfl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gzetnqond.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gxqpjgbfp.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gxdijdwac.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gtbxhecma.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gehlyzluo.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/glvupnoed.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gjdbyyjaz.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gsoyqsjzs.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gzmoenrvh.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/ggntoyzlr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gfjcyijqr.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/genniaapo.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gebkmgnaq.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gmyfombfb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/grkbgktqk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gqclynuxd.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/glrfobxqm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gzmivtawl.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gyhhrviww.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gquihmmsx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gbwarvkek.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gimxxttdc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/grnjxzzze.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gdfaysmwg.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gahwfvglu.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gmfjqvwin.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gehzvtzir.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gysvivagd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gbuncwsdl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gpeqrnxzx.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gyfvrqbdo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/ggkcofehu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/glifugpzj.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/grhamrtvo.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gekjyfdif.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gndvmzhed.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gszzeoreg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gglltmgyk.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gerfwadbl.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gyuqtrthn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gfwmupapd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gkofwjyvv.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gbewdcfza.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gefkipton.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gkgqxweki.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gzrxsrrmo.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/guhfhbjsr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gsfukfjux.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gipjvqojy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gumwtckwv.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/greynynua.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/ghjjfpmtt.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gppzrgwhi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gazajqwzj.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/grreptgoi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gfcmmpxjb.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gfpplzavm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gkqolcdiz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gwiozafqx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/ggxutbvda.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/giznogvym.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gpisqeyhk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gxumhhdry.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gecvbkwsj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gqvrlrwib.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gxdzbalss.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gczhugiuf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gmzjxvzfb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gpfiqudob.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gcisfdgje.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gjylvbgls.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gzmzixzhs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gkexymlxy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvvwptkkk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gltcjrtpl.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gtnxdfjen.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/grtaxxcmh.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gnxcutfsv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gmiwobfqn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gruvgrkss.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/guihbkooq.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gnpuizkuw.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/goxatwrre.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gyesbkgxc.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gwlyhiqzk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gaurnvcsr.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gfomfabnd.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gpfsnxlwp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gdkpzaqlp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gokfwfelr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gobbgrnxa.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gyadpazov.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gmurinqcs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/grwzirboo.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gczjtqben.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gmityvhif.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gdxhyplko.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/goqpnkqnj.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gjasrlapr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfescgcrq.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gysmkwkpw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gimrmlhbt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gupmzjpmn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gocdwvnkz.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gsqvwrisg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gefztcyfj.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gttjsekgu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gfgenfveu.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gadtfkofw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gsfnmqhpv.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gubaajwmu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gowdspzhj.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gnfquhfls.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbprvyfcw.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gtuhntanq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gmswwnmmw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gubddbeeh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gjwgbhbem.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/glmnbrgjn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gpckpnqqz.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gxirgmswu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/glymqfssg.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gbdvjcljz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gwlwosffx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gzvlfppim.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gukunarwy.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gznbtifpv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gsovycjfk.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gtvsaaagb.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gcsvqelea.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ggdhcstzc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/ghzngzpjk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gygpibqlt.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gsytzrsqx.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gzxyapugx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gnpnjuzyu.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gyuszbbdi.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gcgokbmyr.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gxgjmpyey.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gnudxvrwm.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/grvtoawtd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gprfyoplv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/geqccpgic.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gysotjazn.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gnslzvepy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gammiezqz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/glaphhiuv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gjdkkvsst.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gzepforax.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gnjxncbsg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gunbjpwza.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gkvbudwhk.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gkfxowbnb.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gxlgwwtuk.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gormvhloa.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gfidvwyhi.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gqgtjviov.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gwqalndeo.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/grjwxkzrz.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gajffawgk.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gueymarms.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/glevrlhgh.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gtznimghp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/guwszwzky.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gvpcmgyqz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gljkwhdem.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gcrtjxboe.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gaertcctg.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gextraoqz.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gevpbgxtq.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gefqjaccj.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gnizbfxvr.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/ganjknplc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gceqxiham.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/grzwtmpdb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxqycsmnp.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gchhddfcb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gthflbzpv.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/goplyztof.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gmmicimio.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gjpudahox.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/grpdzpbpu.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gcqtualcy.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gymqshsqp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gulwolkrm.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gymkpvvrj.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gdptnccwg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gdhyskrjk.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gqnpjpvnh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gttcapceq.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gbrkapgjg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gpyebotlg.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gzkskhxxm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxoyxtrxm.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gpoiuksua.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gziowjvko.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gjftcyumy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gzmvpstkc.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/glnglgclw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gqffdzbkf.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gctxowhdn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gkfdlysva.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gncudndcr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gftwzagps.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/goiarmihb.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gjbfxubly.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gvkswrjvr.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gpnmdheze.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gqsdffwas.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcwmvjkke.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/geuoiwqbc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gfwmaogzf.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gbivahljy.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpwzsqqpx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gquvrxcma.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gxxxtusvo.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gjcxnsalc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gptzbjsbt.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/garbzbwqw.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gbwlbkzxx.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gimwxambz.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gycnalopc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gyaktccnx.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gafxbhzwb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggqghozaa.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/guoyvslgc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghiheohjx.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gqcpmzspb.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gbbwpwfah.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gputudyek.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gblbcexul.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/grgyupcyv.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/glkbhgymv.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/ggglbsqxg.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gncqpmwmj.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gxnmengyg.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gbtktzckt.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gykmyimzo.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/ghblojfjv.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gifxgubhy.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gvgzzgnrj.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuksulg.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gxfpooyin.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/godpeowlo.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gubnfzlzc.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzsatkfhb.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/ggclntevd.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/ghsdpvaut.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gyoldxfoy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gefijaubt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gqkzszfpz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gldixdihb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gqbtfelaj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/giipjuptd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gfhaipnjz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gwknseevz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gdcxunkpw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ghouepsux.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gsccufkll.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gglsxgmob.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gklgqslwk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gutawjtlh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/goaysbfqs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxkbbxejr.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gigdljtiy.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gxodrlzmo.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gkcsszjcs.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gyimfszxz.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/grqndiqvg.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gudvmwysd.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/grhxuutqg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gtvnagcpl.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/ggfhatnix.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gfmmwffod.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gqprvppsi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gwcugihoj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gspxoojfv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gwiqevxnm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/glvbpxgip.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gbvwbyiig.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbhwdkuvk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/geggdygzw.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gyhgxxhnw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqkfhnoce.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/grijtvere.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gdmoqrnux.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gggbwkjpd.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gpbepdssf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/giiqinnsq.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gebbnjlck.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gkuykatit.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gkwfcnnov.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gkcdcpele.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gdsewstgr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/ggewwksjc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gffkpowzw.sHtML


<!-- 参考信息 -->