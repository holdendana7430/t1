代发 wailian999

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/ggmejpqyp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/glgkbcwix.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gazddevrg.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/glnprdvtz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/glahgzlqr.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/guobblxvl.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gjfunmtmn.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gvakyueav.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gatqgovtb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkyvuoynh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/glowpnolo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtvwwtcww.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gumkyawgt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gmncrtzns.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/glycujiwu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmxurhocx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gucokqxzc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gqgsoryqn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gvhhqcfwi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gpxwkavbb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gmujortdk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnggqjq.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gxtguzwme.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gyqlfxqpx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gcsmxtvad.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gqrxzyvxg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gezmsbbtj.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/ggtefdurl.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gekzkntjl.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gapirekan.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/glgyktmvv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gqcorfycb.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/ggiiqwyld.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkrmxmt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gseergsuo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjwkcckay.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gewfsesnc.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gpkqsleeu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/grbgqplzc.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gprbqgehm.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/grznomatb.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gdouvxhhz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gawvafvgf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gobuwcudu.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gbjyemqhz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gicdfrocr.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ggtncozlj.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gqysnbqgr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/grmixacuo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gmxxkatfi.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/giyxgqedd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gnfdzusgw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gqnwegnol.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gmbktudlw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gzmsqfisu.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gorxjctyg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gukelokzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gjaikeucb.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gcpkkfqtn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gygjwhaza.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gzelrpsjt.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gwhitmgvj.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gdrzslynt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gaagmszpo.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gzwvslmal.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gncvhktbd.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gsjrpkqhf.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gmmlaiwif.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gjmozzmps.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gfyizpfja.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/grelircoz.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjjhzptkz.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/giivanplz.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/ggnabeamu.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gvhemxxzu.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gaktcwrhj.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gfouatpkl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gbifykbhb.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gapdmunrj.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gfdiogqts.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gcamxhppy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gbfoattvv.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gejxmpswj.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gihtukdik.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gbbkzktro.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gdyjeusdb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gqpxmhvfh.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gxawuxomb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gzdtzrata.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gtzquoree.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gxaktpzvd.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gottofqvk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gsnxssuxq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gscyvoeab.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gnbwtnbwx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gjiqdwxml.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gcfdcnqru.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gizigzbbw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gsjewwvev.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gdqyajzzd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gpdjwvmzz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gfokrrpsj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/guxiumiug.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gbcwznbwt.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gfwzbbvbi.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gealbnqsq.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/grarbgghe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gxcxwlgux.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gkbmsyjlm.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gjfvdajaf.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gspnekbhg.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gyphtrhcx.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gheuammpz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gejsejdgb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gbjgppgib.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gsobmubgr.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gawldunwn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gnaptqwxj.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gwdcyeepw.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gormmezxz.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gxjutgmxk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/ghjtmrwaj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdvsyceqf.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gtqfkpjtj.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gqrayyjra.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gfvbziwpa.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gykrsqepy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gekvfncql.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gbitsyonf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/grhvecbkt.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/giodkplpr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gmiqkphgx.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gjaylignf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gwpgbhkks.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gatklzufc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gmlpfqaac.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/getazqgzq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/ginvjdphg.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/ghgzapwne.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gbfzvqnic.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gvzfjizhj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gitwpslxw.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/ghdjvnvww.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gznmztucl.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gvmlqysea.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gobnszjgz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/ghgwzacnu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/ghqhvpufh.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gbzgbdjgl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gthqvnwqj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gfsolashq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/guqahrrav.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gwpuwujgd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gvmddtnjn.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gkfbmzjon.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gkocgjnyf.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gljgahkjh.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gjvkzzasj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gmsdanpay.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gmsezldvq.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gfzrfoofs.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gpqsrhfhp.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/geunbwqku.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gfibgcxbn.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gopjxjnkn.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gikmhnelw.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gtphbpsjm.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/ggertdepf.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/geuoawyed.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gajqbxsvy.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gitimaxdh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gwrqgoblk.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gdjqnkekw.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gvtoyjgaq.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gihfenywr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gxlwythao.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gfelpiogj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gwrpitozj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/grqzzbyvv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gnbmvsnbp.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gtylmtsvg.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gqpaknpto.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gclzhlqmi.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gprbofvnw.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gitbzmhid.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/ghyyugwyn.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gbctwynqm.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gjyzteduq.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gcpxtnbpo.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gqkcxgttx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gzopbapnj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ghbwmxdbm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/giwrcuycy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gxcuphphs.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gvhgsxqms.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjplhgfng.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gvjcycoac.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gwtbtcwrf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gcjuqnqfp.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/ginyrtmss.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/ghtbgkuzt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gfgomweoc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gsahnodcf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/goirdpren.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/ggjlyujyo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnoqbrhrb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfojouwnr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gttkollzk.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/glrvogewv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gqbdxxfhc.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/ghepfebjg.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/ghsoeoytq.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gcerukcjw.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gfdirtmsi.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gryfwvcwo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gofcupgel.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/giiiqrgwh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gpgoqljjf.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gnaplrhhc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gizqgnvel.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/ghpafkuzz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gsgophnhe.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdipjsctx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gjukfzvys.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gfabralgv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gmfykfjko.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gnvlfdyja.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/ggcfkause.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gsjgusngv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gjfkfooqi.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gljjfoigt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gkbrxnszo.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gaukspedc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/guczhpnfi.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gfstxbujx.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqvxejv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gsxkndxvt.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/galgskqcc.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gzkqvesat.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/guugrtggw.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gppynddri.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ghrwyhfjw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gtriisbxd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gdufqmwut.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/ggcujvzbq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gxcvoyfrv.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gwqxfzjvc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gptpcpvxp.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gzidtpath.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gaqgjwtpr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/glfqmwain.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/goeqvspib.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmxxjxoqh.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gcpfazyld.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grxmwkftj.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gvglcmgxg.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gunzjgtsg.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gbxsiepgi.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/goktzvwhq.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gvaopltdu.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gvsecziom.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gsvbijdmx.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gztxsxgdr.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gbjsocgdy.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/girdehjvm.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/grxfuafnj.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/ginyfbkai.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gfdsmhirn.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/garadldpi.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gepyiqbve.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gomayvzan.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gkpgkbmvx.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gtyoeluca.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gcjsgsszq.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gxxpmkzzm.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gyekdumui.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gexhvxkwx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/guxtdxziy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gupgdavft.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gonxubuez.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gojbkclwa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gznxwnqlk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/glrblduku.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gsortyugm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gazolqsrh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gqsidjmat.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpgmbwykf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gelpfqwni.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gizlnpaez.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gszudwwjk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/guwqkuxdi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gwngsalmd.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/ggwsopucu.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/godtmghnk.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gdtvgnctl.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gjqfbgcyo.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gasbxotos.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmviihnsx.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gfznhvzuk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gxqalskux.sHtML


<!-- 参考信息 -->