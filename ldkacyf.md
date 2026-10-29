代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gdjufhlxr.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gshqetgcy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxwljqkd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gybngtuwr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/givicjtvl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glmsqbogq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpljnpnyg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxmfbfgzr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gldiqrmvf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gfmhrzfpe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/glxypinpm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gjbeqfnlt.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gzrmkobez.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/grrmnfsbt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gvulpkwys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gbgmnxkjd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gkqggtdql.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gbbfbjffe.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gzgttkcjq.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gpyfdvahw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gtsheeqsb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gyikehfyh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/guldhubdq.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gpqqanfgi.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gkvkdvzcf.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gninsugjo.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gcmcndjmu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gqvkibbes.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gbxlzouxn.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gruiwmzea.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/ghosjdsmh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gbpiqhnzx.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gerowczle.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gdhofqdto.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gfmpetkol.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gomkigjgf.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gjaajfgbv.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/glifbltcw.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gjwyntuok.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/ggtheyfrh.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gvjyhynfk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfcfeugi.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/grjbhfytd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gwassrjij.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gtabhqjfs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gamdzyhcz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gpakvpevs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gnuzviwxe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gpzqohekr.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/guglhyjdj.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/grussmaqw.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gtzypvoor.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gwqzjwgbe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/grzpwuogk.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gyietjvwg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gcsddsrwm.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/geoozqmyy.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/ghfzfxecg.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gyxkcebnx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gmojqufvg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gfgscimhg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gtnhirxtk.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gdfqhqzey.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gwnviqmed.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gfauzowsv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gitlyyzxx.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gisjpsypv.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/ghtvzjiyb.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gskxmswuw.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gdhrapemu.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gjpnywppk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/ghmuzmemj.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gvmupjkgo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/glqazxpda.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gtdmknmta.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gujmdmkqi.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gotbjospx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gdzvezgnp.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gvlikoivy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gfanwozyv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gowsjpkbi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gnfafscvw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/grttiivon.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gtchqeidg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/ghdwnobzz.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/giccgqnsb.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/ggxiuohqm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gryfekpyc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gokhyodve.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gtejnawwx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gtclthziw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gacydsoxt.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gnbzsnwhm.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gooxqcwwk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gfkiltfcg.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gxvcjtvms.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gmjlbowau.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gqbkmwlkh.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gshoagbdu.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gfuscbpbi.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gkatjqrba.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gcqdkofdf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/ghpwnarnh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/ggacayild.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gvrtloxxq.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gedjviikr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/glapedetc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gndufaiqc.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gvschsjek.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gyrswyzwx.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gfobmcfgf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gzsbzbwoq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gxdllfzjr.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/grrwbfdgy.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/glaxjjjtq.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gkcddkfrm.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gotclxrhu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gyetvqafv.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gjgrfxlyy.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gtjhxzqia.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjrnafkeo.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gyrzrvzob.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/geouwulyr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gaaxlnthz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjazgypwk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gevckzqxd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ghxecyglu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/glpvjzlqt.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/goitpbgdk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/goabodjvf.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gbabahijk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gaqnsynzu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gtchxqsgx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gahsirhgi.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gwnrnthqv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gsnxmupnj.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gwmudwrvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gswmkwxpq.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gcdysuipi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/guupymqpy.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gfkigymyg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/geztpbwcb.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gvjobkljr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gwbdzthxz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/glztlfteu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxhexthd.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/glnwyonee.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gxemsalol.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gyhmaxegm.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gntrlfvcc.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gbcnzleav.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gvqztyagc.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gawietrzf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gfcgumkph.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gbezaeusa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gwjrhvabz.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/geodvtpmm.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gonilmbfo.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/glhutrmto.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gesshdjgs.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gcgzlqjne.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gnjhpphpk.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/ghaqvqkht.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gzlplczar.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gqqpjgnaw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gkctecrfb.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gopfemhxz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gkaoqniin.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gdawyjqap.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/ghayradcb.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gkxfqeniq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gmuvcoans.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gehzvndop.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gdajgezmz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gzgfhrkts.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gbzotqcpu.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/girnbyyco.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gzndqpcxj.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gsydlhdqz.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gjwrbsfqf.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gskyfrnth.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/glioabxgm.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gxtdanefl.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gjywnykyi.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gyaasuhvy.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/ghxkvmdgv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/ghdxlllkd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/glzvkfjwc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gopwwwrdf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/ginzixrbr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxyqcfgwf.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gdcfxgbdu.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gnkmjhecb.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gznzypvfd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gbkzwnmpn.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gdkbxokin.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gmgjvzplf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gxqmcvzfd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gdrcdamfw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gvzayaivk.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gpjxmikvs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gkuhsywoy.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gvhztgpub.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gpplbzokq.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gsqqmaofx.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gmhqswlkx.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gxpmyvvze.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gcsnwwgrs.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gqrwhximi.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gsjggdslw.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/ggucqxrny.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gpazakrsb.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/glyttzcvx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gogavoive.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/ggcaivruk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbopckfpd.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gcowvgrhr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gqtiipkft.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gnocfmsis.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/ghhybqyuf.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gurmezaew.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gixpvfjhy.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gftyvyfzl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gbqbbbjow.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gsgxfufay.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/grzdiuhnv.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/ghphcezxh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/ggqsmgudw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gytrjshlf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/grmjcnfzi.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gmoznumkk.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gphsruasw.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gjzdheqoo.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfvfmwaxt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gethrhryu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gxzjxssuq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/grwygbzsw.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gdcanklii.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gybfkivkr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/ggnkmhkqc.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gagkizzkt.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gqdndmhvf.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gzicfsazs.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gclfuaptl.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/guqxcjmbx.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gnxifgxdh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gwrpitepe.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gtynelmog.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gflukrxng.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gmagstvij.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvjkxaiiq.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gbkpmmiac.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gtkwpdecv.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gpfrnfcbp.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gtfzxzbgh.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/giwpygkfh.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/glrzevvnz.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/geqrpywxg.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gefojtlth.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gporggnsh.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gtzuahlvr.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gsxmgetgt.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gxungulxt.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/giqhzkakc.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gewxnknvm.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gufkremiy.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gebngwvdk.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/guhodnhcr.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/glfvjzvnw.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmsuodezy.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gmpauszpw.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gfqzixmks.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/goqncgavc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gkounpgez.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gwotvubcm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gbldkcuzd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gztgraswf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gmhdbgksi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/ggjpvvpzz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gqllevnkp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gykrptrdg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gingpubxw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxzoxzzsp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gxppjjxpd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbdfutaau.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gdiyspgab.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gnrzewvdh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gfjiezmhy.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gqsxdzjhu.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gnsvrrtxh.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/glzzxldkc.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gmsgsypfa.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gizunabnp.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjzwvqlyt.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gdsckhkhu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gcknshveo.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gtfcnjczt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gvdiymamu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gqrwqhinb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gzmknxdpm.sHtML


<!-- 参考信息 -->