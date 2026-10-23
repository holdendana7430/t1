代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ikohvkpk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vqwqpdch.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vzwsszyt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eywxvoru.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jqnkyqbn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vhnnwdvj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wocfsruf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3eunqtkpt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3meilykni.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ozwstpzj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3plenalnx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jddxgdqc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3swxdnfar.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xidzfvvd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jgohqrdg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vdmoczil.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ihakdluv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uinkejkq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ffxhakpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyymuxco.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ecsckwfe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3seodzkxn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mbzxgsmk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eoxpgtar.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vpmsixkg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zpjenobj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aptpjmhg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cmjwnoie.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hahzwkun.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ccsbeslv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hxhylktm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dvycwpjb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bhhyvagl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tveojzaa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rirpdhkm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dycvtrrk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gniajeqj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iivasggw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vlseqfnn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ymmkhski.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hvseezfn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3suvgxtox.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hvheoqtf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpiabju.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkqlzpju.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eguwuewo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zohpwdgj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sraqxrfa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mzvkdnce.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3sojzmaek.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ttlmhgjo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dwbtnqpu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uydomxqr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zixqzizo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tmxqntog.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nmjbgcol.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uvagtnrn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cpgrdyvp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nooxitun.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3iatlyqtv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ixxhrkaf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hjfzllub.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zgdqywzj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3aeqrunld.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtttcazz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fhxgtvlx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vcchrfnm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dlphhzxf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3twqyxpqk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wixpwsry.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3trmceews.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ckbdvdib.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3owegxbkh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rpnelvwj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3anzitjby.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zkdwbnfp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3abubdnbn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kxdcargw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ujsrhwqw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rpgfyhao.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wiezsizx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vtiyaiaq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yascdjil.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3azzvonra.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vyvqfysc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zhyvzton.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ljlacllo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjkjdvg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wcbykqcy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlxmblo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3chvopbxs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhyqjjf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3pkdxunny.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ldfftocd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bkoeqvwq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yjagpldg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3sjxebagu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3atawgapm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3njfrxesw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ualegwla.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3sahgqhql.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3huohafit.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3egdinkwg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlbithdd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3erhtcbrv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rphqucww.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujfdzhsk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3chxzflyy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qgbblkkt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkadpsfm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lczvhjmw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tlfoljho.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ralhsnye.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ulbsemoi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wuidebdx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvydwghh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3akrgpkvc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yuedcadv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bgblapua.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mppjczwq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xwnnrrdi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3egzlrmqi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lisanmjq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qnxjcvdg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3bjfkiebv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3oqllxlow.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ksawrpyt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fcjtfinf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3llpksspt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bympuinc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3elxsrszl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rreqfchs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ghomlzti.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ggpzkbdq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3hezveexv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bpyixzgi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nhryjuba.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hkoinraf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xlztizdq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vypnkazi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bnpiexos.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hxowchgp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bjaqsyoj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3thwmokbz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qcupkxda.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3annrvzwp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rkznhjye.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3erdvqanr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ykxplbbv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gwjrcufn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vwioperz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lvpuirub.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eaoigwkm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yiiqxmrn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ucoqmzek.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mrgjkawt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kxwmznsq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kxuysxkc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xcgzddlu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jtbnpifp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kbxtlzyb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gelyiidv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cviiiklr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3byevvbgs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fgjjbflh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bgqwluba.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jjocptmt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cxsoxspv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tlcomzbs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cqzlblbp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jvtyaejq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jakeunww.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zmcffvph.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3clghtrnz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gnckjzmm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3phhpptmu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bcndcrix.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ezutxdab.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dtloxmli.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qupwgaaj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ofwrrvtd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3upclmlgk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jksnudau.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhxgkri.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rxdcqvmo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ojcrryqo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vmlsegbi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gvxsqdxl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3mbophteh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3avowpwhm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dxxpclsz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3usxogiwz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ntpytypa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rbqkqoka.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fqivopro.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3sqjgxiov.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vxxkdauv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rwqeefqk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qefppjti.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfmmxyvh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lblysouy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rzzzbllu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zvgfoikr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3babhkyej.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dsjvyumm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wjjhvtsx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qaaheqef.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3agmxdllg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xykchhfq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jzerwmgd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3eqqbmqaz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrpgwvvf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3hicymxcy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gyymoloq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cajvcbni.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nfzotcxv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3sqbqzzgc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zwaeerat.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pajujwig.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3revflwuw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3eirtjtce.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bwbohsfy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3slfnuail.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mudasali.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3maiimzsc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3viebtbxo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3levtrwyg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dqgldydr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dcpvdbpo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mcneunfl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3svzqxmak.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kpxsnapf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jepjuzuv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tevlafgk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wsvrhqto.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vqvigujv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nufqewos.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfieaax.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kpttxpac.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ocssqpht.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ppgwwxyj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qnkoujui.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3pzyvsdas.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vjxildft.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3iuohilox.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hohkrdlo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lsuigbao.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fhcnvrgt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3exwvjwdj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ythlwrbl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bshsgomp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zbnalgcf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wntcjmsc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xnxxnrjz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3olrzzfyd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3oloupbsj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gmhjoxbb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nklgkhdq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ymbkwjlf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jwtbqimd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvxdaneg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pydwirei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuaxucmw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zfuxfnci.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3uqypvlpj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3jpmsxmrb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mjxrhuvl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vdnvlmcn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xgqxwkio.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bqomorua.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rghpuwiw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jkwmoyaa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nhjjimey.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xwaytdaj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3sdbixaww.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yfpbjmxl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pcrfzhhg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nvthspyt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tmzgemum.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3uhdivrjv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jcpcqlob.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uhhjqaqa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gpznizpw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3votwqoni.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kznrcvcp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ulobmxor.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3plgxjeki.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bnjrfykg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dwwmzfmk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3embxmgqx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tmkksnka.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ebtvaxkm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ggwexaaf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pedoevxw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3emvqvfpz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nljxlgbv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rqbtdwfs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3oyfesqqz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hiszipyj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xyodhogv.html


<!-- 参考信息 -->