代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyenswsr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwilxmguq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzdedbxg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxpuybkb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gxwnhdvyj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtpnanpx.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gpyeypjbf.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubxhvxzc.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gyqfacpxd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gilgdsjsp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtizqzjk.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/grprhovku.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gcofqxwoc.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxwaqhkk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqmhdxde.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gtojghoyq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gapjwffzk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/guhzngljv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gztykizdn.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtqjcnqf.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gppyktact.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/giynwnkjk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/goentosgt.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gsepssutz.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/geatuxupd.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkwddalz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gcyuwkkdj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfylwewec.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/guvovupkb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gymzavznb.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gjonomykz.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gqhxhkuxw.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/glfkqbgtt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gunrlafon.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/giqclrslp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzylofiv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvykriouy.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfttoswj.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gvycwzjyq.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjepuxxfm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/giqchtxev.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geesjorbt.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbqyihp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gkqpcaluf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsmgcxjj.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjajrfxtu.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gthmlbzux.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfpbkpte.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gfuzjfpls.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/grtazgfip.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwsfrrn.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspgybccn.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/geruxzfsf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcrkrmw.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gtapelgzn.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gpyktnjbv.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gdwosyakp.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/grfepsaei.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gntwlhozt.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gzoflccof.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gdusgwimi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gdqlqrvol.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guneomyfe.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqakvpdb.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gvfpnszzd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwygcbaht.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxywoegcu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxjznwem.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfdvmisx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrarlaod.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gfsdwkdtx.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gfhnmdaqr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsmrglbb.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gybznurmc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gvigpphfx.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujhiliaj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkwtbfal.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldcxcrfl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gyivlhzxr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gawtqbxnn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsblyokum.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxcnsxxq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzmjwvdy.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlbrgkai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghbtdycuv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gidbwhagg.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gavlayqxk.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/guxukxepl.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdzlpgqmr.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxiwkgkc.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhfcnono.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gphgghkuf.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhixsivg.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/goopnrxgz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gzxuznbpo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgyqmbyg.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gqprtsjsl.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gzwbfuzvz.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gltxfluwj.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/ggnjnjuta.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glolzvrwv.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/galpcagdr.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gqiixmxka.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjyftflb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyunkbpd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhngfirp.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grltcrzks.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmevcwzv.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/geauybnzg.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaydwvqhh.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gxicuwjmo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwweppgdm.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysdohxqe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyiaqoft.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gwkvozjyf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzriqeiv.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqxebclc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gjzkyuyre.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyjesjoh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiqvvzzx.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxyryxj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gptsctlwo.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnchfgkj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscyitfdm.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqhnmbhb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpzzubbh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfsilnye.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gixgofprs.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmfhxzh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkazitoqh.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubivodvz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gghatxxvv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdvuzmts.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/ggovriipo.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gkimdejlv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gmxgdbjti.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxquzkk.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gocvquqwr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gagkhxfse.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gdbdifgqj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gbzjmyewe.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/geupbnjtl.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/guysycskk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihjknwuo.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gwojbmtmr.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvtmuajf.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/ggangqzfz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gsbciyqhx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genrwglej.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gwskbtkdz.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/guzkjxeso.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gppqommih.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrxiuxky.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/golsnsyhj.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gtboipwus.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfxerja.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gsfuxsxyb.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gnxrzxhwy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/geymhqlcg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwizcubkp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gmdvfzcyq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gxpcnbaef.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsxcpkwm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpxfkysh.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gqpwhdkfc.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gditbbzkw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtorlssa.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gjdgdncaj.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gavebilps.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganvvprhd.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/ggzjtftma.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyvzwwsr.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/grqywluiz.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/guzqurmeo.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwhzozdvv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gonagmngt.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikvxcsnc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/geiirqzrq.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvgilskq.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grcqirfoh.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gckxpkcur.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gippvgshd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdzxikbl.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gbdjlhmxw.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpihebz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gaqmsbfdh.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gswrlxtxh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbairdwgr.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gtcotkmwb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gcroftvum.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwhrddp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpncvkwa.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gqswakvgc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdtggls.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/goxbklmoa.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/ggrwfpchy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyxkahai.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuiyyztj.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gctvnzuib.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyhdshkn.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gifqehbyp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gulfxagoz.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gnrnjvrvj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gppeilrrw.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/grsqvydov.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndeqxibf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwggrvnjo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gnhwaknnp.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/galrnjecb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gufdhbjyi.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/glpzyoakb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxonvzfn.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdskntkg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqegssc.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gvpjkdjkh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/ghumcxcqu.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gbudkeocr.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gucjbqppp.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gfkmjsxis.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/grryvhdea.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gxosnfsfk.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gfgkobihu.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbistacxh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvriixij.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gpzxdrucp.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gjoeflnvb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gjddjuvot.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjvphbh.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gqglvwgir.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gadhwwdes.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gygvxozyk.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqqpfrjh.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpvalqnx.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gpdmwnvmt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gqvurkwey.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/geduxkubl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpkhylfg.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxcazsxj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqllusoy.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gqwblosed.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/geuafcczp.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpocppnr.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gbijonter.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxapzwng.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gxbsffiev.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvsacrjo.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrwwnurm.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfmubjuy.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwwmrsvh.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gllfnmtpz.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gfazsluxy.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqoawgut.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/ghifzrukk.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gpibhcngp.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzipzluru.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmgimqsn.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gpmkfdcyj.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcazbycf.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gbgftslcr.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnetxfjnj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogyioqqs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gdpkovbyr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzukxrkr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gjcpywpeo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gyazwzbrm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gnuxsqals.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gelwnasru.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gshyaokyc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/garxdumds.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gsnzvrhgc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gvoceobqb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gskiqyhyn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdpvxjaf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhyxrbuj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsevdewef.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gpcgsrufy.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmlheld.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gmrujcqnd.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueijpblv.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkxpqbny.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/giszlgrwk.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptkjbphy.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gsxtvkpeh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmvbaalq.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnqwdadw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbvgezyj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gccajpbxn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnfukboh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmjnhlbv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gugpviddb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/goleiojdc.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gfsbxksyj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwissnpvv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gxgmqrmsz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuzbmarg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gptlyoquc.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/glkuzgdir.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaentgib.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gagyrwtjv.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gmojvyxgv.sHtML


<!-- 参考信息 -->