代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/ggrkeejtm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqqrcdotm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gxzyygesm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyikipafy.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gozcbkrsa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gvtzurnbk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gsypczztl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gffgdgnik.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gjoebmpaa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gfngsqwkh.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gdyebbpaa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gekqibtsf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gymvyxwsc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gdhshcwta.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gurxofbjl.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/ggxrbjroa.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gqcdyhbyz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gmxtzdlib.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gloecsuck.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gxmvdhnls.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gzmtilnie.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/grgqpczqc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gxujiontn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwssxwnyq.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/glyalnkfh.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gyluijaxc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/glztbikzz.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gtxffnbbu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/giedjmtwi.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gsnhjgamt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gezbnyien.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/goffohxfq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gyzfcmlli.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/ghtuszrvr.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gsmmkszgp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/ghhfvcxus.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gzvineour.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gqonomwpf.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gijrzcqsz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gkahktgwc.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gnmgmdtli.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gfyyemrdy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gntytpgfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/giscbnrwj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gjpwhsvec.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gknatmttd.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gztwjktvv.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/guljaqhlu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gqynaqdev.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/goldmdbbf.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gledowgnt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gefpdadgp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/grbfwrdct.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gkehtpues.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gsdlyztsu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gqlkppemu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gwpkuondm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gxrqqcaod.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gbsyyries.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gfixakedm.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gqdltvfon.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gbrluzfoh.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gnawqpsdm.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gaogfscyr.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/ggzmoxztb.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ghlrwxfyi.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gycfnzphm.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gtumgnqat.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gjqhnpmrt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gmorwniaa.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/ggdfvzmqu.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gputmlhzo.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gaaqncudl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/grduhgtmm.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gewumyuto.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/goagpknfc.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/grawsxqrj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfyjqgi.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gfajrabke.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gxlbgugpt.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/grkdmnccq.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/geosfkkli.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gmlkafpge.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gzzslveod.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gfkhxmhox.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/grzhqandt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gnqmhssph.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/giycteytt.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/goqkwdmdp.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gchxazdoy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gywpsdkac.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gsxocjkfm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gpbadfmlw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjkemqcmd.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gawphpuga.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gmpjdgbxv.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gcmwpfjfk.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gdbamaxin.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gdrvcexfp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gblnemcxy.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gxgallshx.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/govnbxwqv.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/giwtblfti.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/grdkezyua.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gbfqqaanw.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gmcwkbzji.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gauapmwba.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gmavqfyzo.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gkdoprzeh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gdglncufs.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gppalhtho.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gkznkdhrg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gcpjxzakb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gcihndlwt.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/grqgjnvvv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcmczuh.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guawliubi.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gifboylwn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gnkdgraui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gqzcgakoj.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gkouffdsi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gdpaxsqui.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gaoykmghn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gauxrvolm.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gtcxglzfh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gjlhyqymm.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gyenrluje.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gmpejwzem.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/galsctgqo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/grhbkijoe.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gizcwwbps.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gfwodaxxc.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/glcmeyizp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/giemfsdff.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpsepnq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/guqdbyemx.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gklopdrer.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/ggqxwnhcz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gbtxareph.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gnjelercp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gfnlhhsmh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/ggvvuvtxh.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gcpqyyaho.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gamsqomyz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gvsuefeyx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gvwfsqwmh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gitcumjjn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gjhzevmag.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gvaixdrdb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/glcntwkhg.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gfbyaggce.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/ghhlbgiwz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gjscynysg.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gpbaeyeyr.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gsamhwibz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gtvbomgrx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gghxymgvm.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/ghnjvsqug.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gsymbhmjc.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gzyhefppa.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gplxriehx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqlsuph.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/glvuywflf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gtihjldih.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gnvkwtfjl.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gzzasjotv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/ggriudjno.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gkchzyjoj.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gqcvxifyh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gemxqqvqe.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gfdudmmhz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gmwktecmv.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gaiaciucy.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gkznfgkfu.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gdvepajgn.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gklulhuee.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gpetjjpyz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gbfnyntac.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/ggxgqrzev.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gcfmvnxwe.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gdwhhgyus.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gffxuiyqx.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/guuwclkfp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/grfqwanix.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gpueagsai.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gobxqxizh.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gdeverayu.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gxodyfslk.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gouhlxsug.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/ggobduraa.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/ghljgxviy.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gwuxrxlda.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/geadrmmzn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/glygbjqsa.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gwrfqcsxd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gabwgqrvv.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gvrilpkfy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkovycgdp.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gptqtymlb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/glkeajijc.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gjoxghyrl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gajousbjb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gxkylvayo.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gulnlroen.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gctzavzgd.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gahbqmtfb.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/ghsdgrxak.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gywlltrqt.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gmgxwgjtc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gmglczlrq.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gvztxssai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gsqvtlvvm.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gmztkuelg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gubyhtpow.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/geqxmxnqh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/glrgptmij.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gusltelms.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/glglnsbjo.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gitvkwvsa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/glbrhxkxn.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/glrjmqsty.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gpmsrxyki.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gonvkwbqa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gouolpfsn.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gvddiktiw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gsrwlswbo.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gedwlcccu.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gtwrdoayc.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gsqujtuay.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxxnbddry.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gnjfgirxd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gzpdpzimg.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gsgbnpsve.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gpmtkbdmy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gxjcikapj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gxdmzxjcq.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gzousflpb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gxlvkerot.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gaimgxerf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gsrucqjem.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gsmdpqaja.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gnzrnzmui.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gylpaalxg.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/geqtojsti.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtpkpbsqc.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gpnsmktwa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gemakkgeb.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gncbedhdr.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gwerycgdm.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gbsdthyei.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/ggbjsrogr.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gieawmqew.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/goleadbbg.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gucgkkhqv.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gavimmhfm.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gqzeceran.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gbjwkcfmc.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gjoplqbga.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gvhpnojlb.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/ghjmjslax.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gwjszrlnp.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxzpltd.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gtabgbtbt.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gmtgknwog.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gbwtzxdul.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/grxobckev.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gkkyinseq.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gmnpydyct.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gbyqbrvib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gksobozwd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/guqwuwnst.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ggdoclktr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gcckkuxmj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gkfacggpq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gmekjnaap.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gldougayx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gexgsdcko.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gcqhcimux.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdgytmjzj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gmbyckrxh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gzqshurjw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gxpnywnem.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gutidwshv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gondkuhgq.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gmzjrmynj.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gpthkqkvi.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gyhzwepnu.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/goeldvyhz.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/guimehywr.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqtvjmroi.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/ggszjzzuv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gzyioahoe.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gyeyilgsa.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghqlrhpas.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gbqopovjl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gksvnmfoe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/giyvdfyhp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gkritxzab.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gzxrgbyxd.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gtlovzsou.sHtML


<!-- 参考信息 -->