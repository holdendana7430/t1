代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbutsjmvy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcleakqqr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmuwjnccw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywiocryk.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gfcstbgjl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gklnfmzjo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxctouiz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggwyghkpw.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkdpkas.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/ggpeiagns.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gylbqdyhq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gklwezhvv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gnyqocvpd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbadnngoo.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gxmboklaq.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gqwtbzluh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonexkshj.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvzihcf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxgchke.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gtdwlznjh.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gbxnkplfo.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfqaxkdw.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqpesxkch.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsufzamis.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/grveiovtb.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/goemqgjms.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grgtlqkcm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylrkudkv.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxabbwm.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohkhjeag.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdmazbop.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnuuqjng.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gjfqewxrb.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gbbuvznhl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkuldkbz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfopjkgt.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gftcthavq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaevthum.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gugpqflwt.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gohccbkmm.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gensfeokv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gchoayxei.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/geyasderz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqisaagg.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gpkonseib.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoijnsxl.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmiowglw.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/glqjlritf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaxrfwfgm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gkpghrqot.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlurlmkk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/grggpwhqy.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gwyjrcqyp.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnpmcxsn.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/giahvczri.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdvaytlj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwipnrrs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gldlpmoyx.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gxooepysv.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhhfmizg.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gasguoklg.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/goefmuooz.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gwsbufjeq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyiihtby.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/glmfmidcl.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdjapbma.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gofricoai.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuztwvfy.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmllgbdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gmouibjfc.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/glcgkbqxn.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnpefybh.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfugamcuy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnletpbf.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/giemvuxqm.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gylddjsqr.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgilkfea.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrammaxq.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjvrsknwr.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gwwebzyfs.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gekrmxwln.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosxvtcpk.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gsokffqui.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuknbqwq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvamozd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwzaqgve.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrxykhjn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrypufyi.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gliwsrpkv.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gwevsrezn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvylumte.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmhygvvd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gqinmviqe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdwlylam.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbcxasrdh.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjpcwsvx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbrjcyhd.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagnxndqq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikuhtroc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gukzzquoc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzdxmcww.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gktwlwfnu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpawqqrp.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqvzucfvt.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/grzdijwgv.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gvbxggozi.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gztvgasfq.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gdjoczrvw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcglyivo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsziiyerx.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtymenkb.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gizhqptbk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfscfjny.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifhirsmf.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxglepwgb.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjibbqftx.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gepksavfn.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqrxlbwy.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gqfhsjbov.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjzxswn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrrbtclg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxbmztqo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gakuxqcuq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebykeobl.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxolrssp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdifceahb.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaeywrls.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/guggjdnct.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gieeutrwi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkqpjpub.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmtufeimo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gubbgcofp.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcicxusxf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggnfxhrhq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gtcjkfnds.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gmarhtclx.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gbtghlzxy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gteprckks.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/ghusidobl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmunxkqek.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gltiamdoq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvczyyyx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gukvnpbpn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gmqtwdlsg.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhpzgldd.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gcixyszxn.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnwnkgswv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjotawcb.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/goyugxzwr.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/grhxytoav.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbnsdrrl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gmexlwion.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gsxrvdomw.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtsdozrs.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gnhsfmxbr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/grvjtlyby.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikctpuvo.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllvgvmtr.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqlplsqx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlaspvmi.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfubgzsw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gwndmhtxx.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkfkdpv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbancialw.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gyjmsydjj.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbeqmbjp.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gmibcvxfa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmpsknnv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/graeyrllq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggggngupz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giubjwlcq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbxexiqs.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gtnagwwld.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gindfrcew.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/ggffgdgmd.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gcliwmytz.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoeafcih.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptwpzpke.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjnvgitr.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfdruspk.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gblebthxd.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/ghkacqdsp.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwpvsnmr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqkfamju.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtjzrvki.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gyxysrrvb.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gyollmvxd.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghikwnhhh.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglrfdztg.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwvusvq.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlsclwp.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/govwyehjn.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gnxhkjxsu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdijzyr.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gwesxaqak.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/geoafkxov.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkfnsvgx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gollknujw.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtquyoxa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gaordrqll.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gljxczbdx.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqrcdcbe.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmtdtvs.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfuinksx.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlgrrwct.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/ghubvqsej.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/grlshpxgx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqmvthcl.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/ghxzxptmj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gsytsklyf.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gguqkobeb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnacfxqrr.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gzjljxhzk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gthvdhdnt.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyzpaiho.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwnyufks.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzrmtgsb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfefnkuki.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqdgnmvn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmbprvxp.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gezojexjx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gddxjpolj.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gowvhzqby.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweimwxfv.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqszxpab.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkofxnjy.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnrljhqt.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwupmzpbh.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/goqfocluu.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gkpcmagpi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/giczbimqv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gogqfuhsb.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliipsyqu.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnsyoast.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gjtggokbt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmzsetplp.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmscnbvft.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjidpuqt.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgpqbfb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/galupypbk.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhtlqwbj.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gdjbenrkk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gcdillvuz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gavtqteag.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqyqihg.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gzslxdhrw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsrgrzrdh.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gmbahogyi.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjpfbdni.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkhfumiq.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gltzcbcxb.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbqpuyubl.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gxcfyogxp.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkngogmu.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmagpkxl.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/ghcvxxtym.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gaozavmys.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgjppvcq.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/goqhrtfig.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gqvifosvw.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqbcmmvr.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gqssfakbp.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtzgjfve.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevvcotj.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gznmiknel.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gicypuswd.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gbzmybfyo.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsqjldrf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gesnevqcx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmxtdwt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gtdaomdga.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjewsdjjz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gwblttjvq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gsduwpndn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gbobiucgm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsnnjhbh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/grisejzuh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjxlmafi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtavrnuqk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpavoiahy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlhrzxzm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghucykuwd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gwqihrans.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcbbwkay.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gsivdfrww.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/guaycgyuz.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gmknmznji.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvosfgvak.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxjatgap.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gsidkksbo.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goclurqqz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gunfzaijk.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxzpxgat.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfmztklad.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gyskhpdpw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/ghcjfkamg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjphvkbp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gumwrajtz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gplnyhruz.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/grdjlmeln.sHtML


<!-- 参考信息 -->