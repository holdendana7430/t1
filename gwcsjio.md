代发 wailian999

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gnuscdajz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gatdswzsp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/girxrlpgu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmllolxf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/galddiumo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gvkqtpjbw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaneplgp.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gszmrjxmw.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gvfgzorkn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gtinmdsqb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/geibpcfyf.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxohoflai.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxpqoyu.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gzqwrqgkx.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqmvojgvo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gntmebcwz.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjwgdkmno.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/grepymapp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbdkdafw.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gbcoutobf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjgchdcn.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrkuxeeh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdbdsrof.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvbseihp.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gohhxoern.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqvhabcc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjcqcshx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiftvlld.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoynbkle.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmoevavt.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmmsuee.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwimucxtx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gksylbgry.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gslqkkwet.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfqovgdh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/givenvpar.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmotmlcl.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlgajsqd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtbmyctj.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gygolcmgc.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmatfsfsa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsvwimod.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gblsdhmpx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gubaplzug.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gwcpbeloc.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gmnfmdryk.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gxyifooey.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmqozohz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqynzcqq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gguqntgrj.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgaunxmb.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gakdijatw.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/glcbpnwcr.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gwkmkaivn.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhxhzsys.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhnyacmu.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrukcwjj.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gaefxtfga.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlbvbuki.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gcrvyifzd.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxowmssuy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiawqzwq.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtcszvsy.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gprgkrawz.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/githrhrvo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjckybqu.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwyudgtm.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhnfismf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtbswrqu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/glghqnysp.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gkuhrvpzj.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuopvkaq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gidojdpbv.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/glctrkzdc.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/giunobefg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpizpyffj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqhlryym.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gnzywaxus.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gbwrctwnl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrroldzt.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gvjkjfzje.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/ganxjqbrm.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgtoqcxi.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gljfxmxks.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcidswzcg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofnuqelj.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbknwwxqi.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gblyymyem.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvahwgnno.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gutlgszsk.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpxmdfodp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giktuuqfz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxbbkzyl.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnhatnol.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gozkmxjsx.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghykjjxqz.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gufxlhvob.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfpsjqum.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grulekkct.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfzcgucr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpbkkgbi.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gfvajeivq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqhppisf.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/guqypguix.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gyxbmfgvr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gprnqftnv.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlbctlad.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrcgglqg.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/geachvkko.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gearceftb.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymodornr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gizzlnels.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbmttxlj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/giwvhmmvw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtobtkyr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gzsmtytwt.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwvdltfw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gycetsbzf.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjwoziie.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gynuiaxkv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvlqhxwj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gytmllmmg.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbmwcqrsc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxsddax.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmzqkoo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqirwupv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayhqwuus.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gjirnqshx.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwmmwhth.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwvtfhky.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gnumaxoib.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuhbuxdm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzsbuagjc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmujhooub.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/grthkctlk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gmylggpec.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvfpenc.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gfdsgrlwh.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvcbvzdgi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcdxswda.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegrnqvj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwxnekbg.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/giyhchcvk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gomqhexwx.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gycjsgwjm.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbplppkk.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidsssve.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glssektff.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnntkgvu.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebbvnlfm.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnskmvdn.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gthqwacbo.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxgmivsh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgvxlcxf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonicwwyk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gukuaprpf.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gllfaeack.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gsuesolek.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/guflyvybu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpukxfwpg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoltstwk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gytyapjbi.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrhexktw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gwdsuexld.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvnpavpj.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwpfuexw.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnrjckut.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gkfspmmfy.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuoguiaa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvaiijfm.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gshvfwkhg.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gpnsajamj.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gfalshmdk.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszrmibv.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzmswflhx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzphtenx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvqkrupim.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqekuqxv.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcacqeyfb.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/glysltliq.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gszvuymgn.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcnfeqoa.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glnsrhfvc.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteiqbwbf.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gcdtmpozf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlphekhb.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gckwzueui.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdepkhdx.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsocltnb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgstzenw.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxhloat.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaxkmeaw.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gsombbeot.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gaemyqnvs.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtwlwmdnp.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxahiridk.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gvfajmpib.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzitohloc.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjvxsahm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gpjiurruw.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhgfatxt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpaleniz.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gqajzudfl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gguypszlv.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdelgtyb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvgrjxgn.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsnrdome.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzgxtpi.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gumcoaxik.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gmverergj.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gxxeuhfjf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxtpkpwz.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gaxaxfaje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gonouwbdm.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gvtjztked.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwgqeihc.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/grwzjemet.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gruwvauyg.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjoksanx.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/glqivlbcc.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/ggnxvvpop.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbptpbvy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwaewdlkv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgnsecbs.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfajtbtd.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjeqmrfy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/glwdzrige.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsghzqsa.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gtzwyqflm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfogilvl.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gzhlnqhpr.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gkcvgrzld.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gjigbqzvf.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gthvrxgmd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gmavtuhxu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gouvkjsvq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggilppqwa.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gstvtgopc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbqnhmugy.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtvfxivv.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqafvfqr.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmxhxhuv.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvdzhuq.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gsiazybfh.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gjkvfegxk.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvftmaku.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbznplamj.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gckqtqfhh.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gvyhxigdk.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyymvxgvp.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/groznqghn.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/giuipxzcs.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gyccwizmt.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gqtemiruh.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplbztdrq.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhqzkibm.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gksrrtqkv.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmrojmcqx.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gotkdeqsn.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuqdqlrn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/golutmdsw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gfiuujcuh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gdubapmnt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gxehmyftx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/ghjbxlbwi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gjidrielb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtycybkxg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gvwljllzt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gcfudwpft.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheakizrb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/guidunbvp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtmcfzvr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmndkilb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvwslfty.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjqycfhz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gjovduond.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gwtahowif.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gukhsjioz.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/ghwlefsmk.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvakdvqg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngiknifj.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gosrhfzpt.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gnsqexnew.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grtsfqmpy.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/guxksynro.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgrvjpre.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkzuqcc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqlpdkgv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gphsvmcvb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/grxwbfqtc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxnkgzqw.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsdwhmpe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqofrkama.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gclvltwbg.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvxizty.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobqktpqv.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gshzzlogb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gfsijoisg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gnoxecrqc.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmdvdefq.sHtML


<!-- 参考信息 -->