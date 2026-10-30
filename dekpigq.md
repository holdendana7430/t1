代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwaokod.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glhrmsowu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdughifhu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzgsjuwqi.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gyouejpqh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimtrhxjl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gjgylpzmn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnovwqvt.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/geyhyoipe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/goytbaimd.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gsvnnorcs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtapzsdd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvwiury.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gcfirocrd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjnfqcj.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gjyvxzyzy.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/ggiqjleoo.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/ggwihdgnp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmejblbaw.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gegmabjqe.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/goqqbvxmm.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzohjvj.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/glwiafwki.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gglzqgcay.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gllsvukjj.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonimyvjj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gydelrvaz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnwvidtt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gatzxcmet.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gcfrxzcvl.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjxtgwtc.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gpxuwhyjl.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/glooasjxu.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrtrrgav.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbjqekzd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyotuqqp.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpnpfgvw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiyfnhqz.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgbbpgko.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpakfgyl.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgpvopvn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/goktmbnpm.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gofplgipz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvohuxrua.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gnmprfbom.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gnqnjkqyb.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gmzhutfdh.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrjyvffo.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzgbmxqo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuacugia.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/guixcrpkg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzskjmyg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqqzwvbc.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzvqxaby.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/ghfnngtdu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gobmakovh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gcfssqgxk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gggxtouuh.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gslhqefda.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/giuzngbmh.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gvfgcbrbz.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gcggmjgdd.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gefsuovrh.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gljczhsjt.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gdkuunmzm.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gmyfqkjrv.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtimagtjj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gehgmtfud.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gkawxtxbe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gdjnfhsxu.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsokqnkep.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvjzxhtb.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gudfutyxn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxsmtxxo.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkwvfvpec.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gpfbgkinj.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlmolah.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gufowcvyq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/glidsapmd.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gxketyrzc.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbsiidjn.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gmzzyufau.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gssykiysq.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvgvqhay.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqyknpy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gmxojpmyr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdxpyjyp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grehxywmc.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljputtcs.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/grnugqcxd.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggoxalcik.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurquzjzq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdgeqrtad.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gibwkrmvv.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/glzolekjq.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfuozavh.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gauuksexw.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbubobtfv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrwibofm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvfunzgr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/geaeizivd.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gjzzyyvfr.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gryaopuqy.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gftehfjmk.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjzzxavq.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfdqyrnz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtfrfkg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhzgihnk.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gqajzxgaf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvurrscfp.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gitztdzfo.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/ghglqxkww.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnfxramxb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gfibqedmu.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbukawk.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gaxlornyq.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/ghjsqjtog.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnbghthe.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxfflfmt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gggyzdqms.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmssaozld.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrwcyngw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gkevhjvxt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoozwdbe.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyuxgyey.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcurvycgx.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnelygrk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gzkhyworo.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjkfata.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/goeayjbkb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtrtmxqt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsmsdpfh.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gqozfrygy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/giicamnye.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/ggcrbpydf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gzndrlppb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphsdpoxb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaajclha.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsbgfdxt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvylmrzy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikkcfsdd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohssckkh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtowaosf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkerrzna.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/guptenbpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gductgoyl.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gugiyuypa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gccmqrgkv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gafuwwnqv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/geizhpjkc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmdaqzui.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gpgbiveow.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gkznzwndn.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmldyxld.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gbgpqzpsx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznehocik.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gelduyhai.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwesviot.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/glguppdft.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrshgmff.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/grqdrupnw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosudizqs.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdrxnkwt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gepqjjlzx.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gkcdxeoyb.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gswnlsihf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gqgeyxdiy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/grkkwclun.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/giyehurao.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gqafnztaw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjahrunnh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkotxvjlu.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gczxkiyvo.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gslrvctrx.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaexbedw.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gshwmvpxx.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gpqghguhm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrtzbkvc.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gmirxrhug.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gjpoelywu.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxkotqgj.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjzkrjob.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/geikorqdc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/goutriebg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpysfdll.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gzawjqyvz.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gzpmbcbek.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gznhksysh.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzisduoo.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/glhidplga.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqpcrsfp.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwncgwbpk.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqnpxrvl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrkokfwu.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gayelcimd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/geaqcftqw.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gqmatbpjk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gmgncgcjd.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gfvlnaghp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goymmemhc.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpniwafbg.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkibuvmdd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/giubtxnow.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzrbdfm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjikaach.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/ggzhciclz.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaklsvfm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqhgqqw.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjckjzkv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsltgcmm.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gvmxadqbb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiologsj.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gisymhvbh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gamapaouf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbgfaqk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/ghrcbpjxr.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gkqqnzuyo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvzwlipv.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkqcmtln.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/ggatpfyvx.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gojrydlrv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gscmefnmi.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gawjvnvuu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gflihszua.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godaldgtq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvberhhtl.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstjfhvsz.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmwaijnq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmomrolae.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmpthnxd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gufyntckm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjzxausy.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsculwssy.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/ggejzyxjw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxmwgpmg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvilbawdl.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbhqycqv.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbqgqznv.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjyluezp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlpnozyw.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsitzbdx.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gypsbetxq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwrxquiy.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gmewyzepu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gltghibqp.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiaysepw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmeztyoo.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/glohdlyqv.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gqlucyziq.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpxkrwep.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gaowaabgb.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmxpyaruq.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gcrwykegl.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuzfouus.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/glefaoeur.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gblubwrww.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/golohddkc.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gppjryrde.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gqberycrm.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gpkidlygn.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfqlatsf.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnluhbbfj.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/grhdinjsg.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gsqqzkyvk.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gqlbtbsah.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gllilqhbh.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpthuvuyi.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycwneop.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gxcneybqa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/glkmuamqp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtryopro.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdpfkwoas.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxqakuvq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmcpucb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvaoiunl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdarfuda.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gpufvrpds.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gqzrhaenh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnabzeccj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvufqmhi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gpldzuynd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gmaukjhat.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gcengocyp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gdfmmowum.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/ghgocohvp.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/grwjjiycz.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gqvmskkla.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gynzgkygn.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrdvwnhx.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhzeouik.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gxobmcizp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgkhdakb.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gwfjeqqyo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvfiotqf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxjgoikl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gykkqnyqu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gqksudifi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwohkkexp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyauvnbf.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllilgemt.sHtML


<!-- 参考信息 -->