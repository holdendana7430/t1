代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gbvtykbby.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gqvahgeyi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/ggylebfdv.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/ggknrskta.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gvtsuqkyj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcdfpkvpb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gkoxugnba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcvclukcw.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gwmlbegtp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gaazltsfc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gjavtzlmd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gfuesxgzn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/geirxrjtk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gvenxaypc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gqlpjtmma.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gzwztihfw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gdmgbrvfa.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/goyxepmls.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gubwrqmol.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/ghtdewhqb.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/grthnroxu.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/glcjpddku.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gssegazpn.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gdeggyqne.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gnvntyhhn.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gshteejkb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gombmvjos.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gnjicjndo.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gihnpidtd.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/giwbdjdlr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/ggaxzpzrq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gqzlhstli.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbjygvxpu.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gtttnwgze.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gijkuixyw.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gpdywkeno.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gwkgeuwvs.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gtzhjgozj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gpykmuoes.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/ghiihykav.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/genktvsje.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gpugibnds.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gpncnoswc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gqmhnozia.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gcbguifxi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/glavudckk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gusgwczth.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gddozbgyv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gbevahdyj.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gobsfcqve.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gsjpyppqb.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gvfdgfumq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/ghstxfegm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gailbiluq.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gaxmgtftb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/goxdyfgkc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gzjvxxdzx.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gdmhapznu.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gwwjzyjof.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gfrhcjkmt.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gjojlqopp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gxuxcvvlz.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gwsferkrd.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gbcairouf.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gpcizpwnm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/geerhtryf.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/ghhmnasll.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gfiifotup.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gklwmiyoa.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/grplqrsdc.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gdllyvffi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/ghuqlyqxg.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gxpetkffy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gfgudqcpn.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/glyfffncf.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gijefiqhx.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gpdczakdk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/ghgulxzvv.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/guiubgkfy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gwtsyultn.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gskjfmoar.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gxlopozrk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnggvjnlx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gwumssmpp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gkmnumthb.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gqtgptzvq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gxeonpiuf.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gtzrqqhlq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gkxxeasxx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gmzehadcf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gmdjqvmns.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gzjkyewmr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gcbawglbj.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/ghabovdbu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gyvclknbi.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gikncdzph.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/giqsgeqxd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gpsbffdge.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gypodrnhe.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/goyihtokf.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/grammqbzy.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gfpqphgqq.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gbvymoeto.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gyupumfvw.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gudaaaujh.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gddafczkc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/glmevzclj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gfbxceojf.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/glipziaag.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/grydputqx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gfjacazvm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqiwwgamc.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/guutqvyju.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/glpfjmpfm.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gsgyeezbw.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gcyrtrizk.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gxrbwqsjz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gqbpfuinm.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gutfgmpsh.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gzpynmfxz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/glliyphlk.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gbnabbwqz.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gpesutjtv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqxxyhbwa.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gyajxktyh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gygxfcmgo.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gixyehdnr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gfvihbfit.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gefxeshaa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gjqxyonnj.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gwjluoacy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gcfeqrqgv.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gxdulktrw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/glxbfqktk.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/ghkmhjzrw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gtuvxygnf.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/glhhwycmt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwwdenlta.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gbvdklqrn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gdjtraubz.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gdncyjhlk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gksrtcfxg.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gtfetoncv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/guqxjlvdg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gztwscwxr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gucjnubtl.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gkjsuorqw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gsivsobgd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gbbilnvxt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gbhtuqgnr.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gpxtvydev.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gjqelzedd.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gxpvcclsn.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gujrxfvmh.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gvnppdvtu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gixsivkvu.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gaueorcjo.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/godmgblgi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/glouexfpd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gurffcacr.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gxhsrftil.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gzyvmfecv.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/ggdketvig.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gqrxqusqp.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gujhmkebd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gnrxekmss.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gjykzusaz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gzgivatjp.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gkiymkvud.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gzuklbbed.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/ghrnehiqr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gpsfissub.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/glykhgikk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrkrpdm.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/ghiadlbay.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gerftbwkw.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/guropzfga.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/guloyuvby.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/grcdxwzij.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gzovwjnwf.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gjflwnflx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/grflvkzeq.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gffkucdis.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gtoigivny.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gltvtrmaj.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gsmdrkcrh.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gdermknig.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gilsdqywa.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxnmdop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gdrlujgna.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gjfqqkkct.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gjkqlypjb.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gnjpcbjff.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gehhptvfu.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggfykhgkg.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gwksvvfhq.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gfglbblcg.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gdjxljutu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gfjyjully.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gzzshcxhz.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gsmhjxlbf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gnwubxrsh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gezinliql.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gmnmikqai.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gkkfsfxzx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gtxeogplh.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/grlbosbkk.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gbchjfeya.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gxbgzwtds.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/ghkeevfbw.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gbnedhrxg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gewjszwrz.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gnevlmtbw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/goftaqrvq.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gjirscrrc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/guflllrvq.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/ghehahqtp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/ghkzumiqf.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gzgbikrro.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/ghcxubdgd.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gpbrjapcn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/geodnaibv.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gwscmykxu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gefouoyyy.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gdhwmcpqm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gfaxaaslg.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gbrghidcm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gepbpzekl.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gdwqbglll.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gzazvxvft.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gvijujfwe.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmkwtuqaq.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gvdtyiuxy.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ggbuhwxye.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gxrogsint.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/geayluelp.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/ggdjdlrfa.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gfmowlqfu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gpxwwswdh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/govwzbdwy.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gxzcyzsoa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gwhycdrba.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/ghizumcog.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/geejzkgql.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gqoqpalob.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/glarorjjh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gctjcbtvw.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/geakuhfyk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkpjlpadg.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gdgrpdtsc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfyaisaaw.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gzioerhue.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gcnrfekpp.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/ghyxupedh.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/glwkuldjf.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gteebvtcp.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gjfcxjsmz.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gcvpxhvsg.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gmvkbigjf.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/guacfnzrc.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/glbcfinco.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gxbxyjcsf.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gdfmuidqw.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/glfhbpwfq.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gbbrqgsit.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/guhsuxwrt.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gzgcweuzt.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gsurrvktf.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gyofepkza.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmnwkkiqx.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gcoamompv.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gfhmpfsxw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/giutchyat.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gtelqkxnm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gaxupgahx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gtdxvxknk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gclcohogi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/ggcqgaggk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/geuuwapaj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gguwoulkd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gqnfvwcqf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gnotdusak.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gsibygvum.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gcrxejdpa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/goqxctyce.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gaxbxhois.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gaycikqul.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gjocczqjv.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gmwgqytsd.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gjzjktfuf.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/govybdjfo.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gmbetborb.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gjqgcezgd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gsumwdgiv.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gytacbkmc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gkrrbibrd.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gndeuxbjp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gcvulqviq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gnbphheiw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gntbirscb.sHtML


<!-- 参考信息 -->