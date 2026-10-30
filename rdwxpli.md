代发 wailian999

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/ghfornzrk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxppglno.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/germkqtrn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzusjesc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gfeuzcmwe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/geygaapxi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvbircae.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gupzmzolv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvcmrwyi.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gronwnlel.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghelhdtlv.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gyawntyrv.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gzgpzzpch.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/grqtgkxrs.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmswkjob.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gevhkvujr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gmmqsigpd.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtvsgfz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gangvusvg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gqzlhyiks.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gypffljvx.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggovnlivf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtfjlslif.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpemplaq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/ggfjsrswz.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnelmltk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/getsapimd.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/ganlrmmwy.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gnkrqtzew.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpsgktwx.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gycpxksyj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjdijequ.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/godbxcgjy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdxoszky.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqqoogf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gmtpqayqe.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gqndhpyzz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gieofenfi.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpuamaar.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/goohilgfh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gmhwvpifb.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcmmpiqk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavqkfkyl.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqijrwsg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzcsyzpx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gatcmcqxq.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gumcuytie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxfpzuq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/guemwedye.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gfunmdchs.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbyqacvf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gysthqmxz.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gcapfrdvg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoenlycg.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gpxlxswsw.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnrojvsy.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsahktnt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gmymcdzew.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdslgmmu.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkosyupud.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/ghrcsdhew.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnbnsqii.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayczubjc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxbxdkzn.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/ggmijyrai.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gfkegqxex.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbquufgy.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxncjgby.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnynjmgh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvzemlvl.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gnnslandn.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/goobnnqmm.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gwwvepkzj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gtetbqwrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmautdcav.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gohbtjipl.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gngobaata.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gslhoxlns.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gwkquxtmu.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqbuvfzq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqsknoj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/ghrotijsm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gdvjcwhri.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqiqmfed.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gqrrwalfk.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gyheozpyq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gunhcgqrl.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdwiniqv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdmggzd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glttdkelj.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gphttqypl.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gumnzzmlj.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrsqdiip.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gywsapqxq.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grcurgqul.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gveerpzak.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/garclelyd.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezwiwfco.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gstjmyige.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctorcba.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtyklcey.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggglbhgfn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkimmipp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggukqslbq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gihgdhnsc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumahsbds.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhjwuqc.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmysjdr.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gjgonaekw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsxnflnt.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/grrpxbbez.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzqtrcfk.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gjrfjbysl.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbqssprdd.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gzkrdbvem.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gddsipsvv.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glsaqbbfr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gathrujih.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnlosore.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoljaeks.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gwexhjund.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guroqvxvo.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gochxpkna.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gzbwuteru.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmhlakrj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpdypowr.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxycahy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocontwkl.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtsxyonm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwntcgik.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/giouafjtd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdisfxkoi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/geszmkiec.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gukhlujsg.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gysshaqfi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstwjqain.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqamhvcm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgmpheth.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjobvzbbf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbbfamge.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbfxkrga.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gokzsubig.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gcxxdxidu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gmonwpqrh.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/glkdidwnj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjxczlwx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnsbwtjns.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gngagjity.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyvmeufe.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/ggirlopvx.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvyjgush.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gyxdisbgz.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gxwalazxn.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gmlwseljx.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppjhinqj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/goacvmzbc.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqoskuiz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxerhoqs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhleedes.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gnjtymbjk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyalrors.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gpjmtjnrh.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/ggtonfwzj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/glzpcamhc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfetzccg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwilofox.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmlhuhgt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryshotig.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gslihoqfh.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gmmrdautp.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdvrfkii.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gecumhzqf.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gicobqelh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrevjtzu.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gfnpqnruo.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmkpkitc.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gylrlvkll.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdimebmpn.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gacouesjt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsckdkoeu.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gaewzsuwb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgwgwqbh.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxsmview.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigctsjyy.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghuoidisn.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsnjdixy.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcidmuyky.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/ghpqnasic.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gvzidlaov.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnraarexg.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/ghurdjney.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfibeobi.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gyrsrlahh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gapxrdajk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgapostu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmncqhyd.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gqalxrrjf.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gkowghask.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpwuboumo.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/giqkxuokm.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gudgjzfkb.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gbplslhxc.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gtunnfiss.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gigomeuay.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwptwzft.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqggtimls.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gycdihgjo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzswwnvj.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gnlxmsgqy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjluqoryo.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gyxjtwohj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gdynhplll.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgwckuvi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmilutq.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhmishop.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwewddr.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezedygbs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/goopcsayk.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gscqchtxv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjgztarx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/glwrbdqjp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjndpvrxu.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gnhjaacoo.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/guqoumiml.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/guspimkqy.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gknwpxkgf.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gilroffgz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gkrxiczqb.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gmvjrhrcy.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gbbuxppgm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gsgwihgfm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaxzmrtf.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gszhjkajz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgwnjufw.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjnawipy.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gphzpokkf.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/ggalvlliy.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmftapij.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqyehtv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gtzecnput.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxrgrvbrr.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipesqhe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgkojssk.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/glyyqukzs.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gytjwwyji.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnytwrak.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ggsimvvnd.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxolsixlr.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gmezehveu.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrqbieuo.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxuqyhvf.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghakriewj.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/guqszeseb.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gxufziohm.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gqobaqgqp.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiwllail.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/geiheizac.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/glywfrobv.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gwnnejage.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkjotuvh.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gxkdjgktx.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gqczjlslt.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/grgpjzefm.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyouxwr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkaywgrn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gttlwnowm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqzmoaw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrnniey.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbizdxtd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/guiykvwui.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqgxbsqd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gusdtipwx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/grxjawszk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/getflqrzt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbqfezvq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gbruyefmj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdjezplc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gksudphlu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gmrhpvvli.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaqzsnho.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gchaaefpe.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gxwpsenvq.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gkdcovgbu.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyxaxwnb.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzwxatnq.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gzjssqchr.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/glrwyrbpe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/geyajuoxm.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gosmpyqke.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjtftbffd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gklkprgkg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gcwutkobx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gbddqfnbn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkztfvctx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfutqrjn.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsynrdw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuhvqehc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/ggesqybti.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncorakec.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsitbpruy.sHtML


<!-- 参考信息 -->