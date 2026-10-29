代发 wailian999

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gxdytvdqt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gfzxypind.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gvffbzkgt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gfuurshhr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gofmxvpuu.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/goyqwonur.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdtdlwz.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gkilzsaoe.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gtzoiicin.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gcbuhwzrz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/grjtqtphl.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gmqpqjecg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gdaxmjxpa.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gzibnrdze.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gulminrrb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gfodyugdf.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gwverkhdy.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gjhkdqbol.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gmyviszvx.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gowruznpc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/germpokih.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gscwvyxgb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/glpgdlnpz.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/giqxbznbd.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/groyzqllw.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gkvsgamfd.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gdgkbnguz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gddykfjvs.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gbwjhzfyz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gzmmlsuug.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gzratvtwm.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gevxjbhpi.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gphcztigk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrcclkbw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gbyryaazl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/ggjjoepet.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gwacekwoz.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/girefhjnp.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gomoojvwo.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gxyprtusi.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gbgefiyrw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gyqebwmrf.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/giztvcokw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gwmcdsnsc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gqykjndzz.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gpcirozdw.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gjorujcjb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gjkiqewos.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gqzvlactt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gadkndeyt.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gcfrarkec.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gwergzjlk.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gkuieczri.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/guqcntgtj.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gpkayzwnn.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gynlldvjl.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gsalhnsxf.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gobpjwhxg.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gifbjiphj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/giocllvrv.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/grsbzuluo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gdzmjrlwj.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gmdjbpymb.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gdcfmsdbz.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/ghnusuvrs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/ginjxpbrq.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gfkfxwhpm.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/ghptagpyf.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gihyuxnfa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gwpujfkqf.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gjgqhfilo.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/guvyshkwv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gpqnyrpcm.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/groplnvbx.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gfjzrmncx.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gtqdgefcd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gfowpufjj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gvhpnoygu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gkxjtnfle.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/grhlkqtsb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gfcpyiddh.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gsbyeouyr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gbhtfraji.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gzbdbewne.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gsmivnrbt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqmqkmugs.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/geeauvumt.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gtehcwlud.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gdasuplpy.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gwlhuqfrv.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gujmpuvyn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gcbhdubfl.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gduetuofl.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gclvrhtxz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gyliwdxlc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gdyblgxpg.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gkiennxdg.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/giffbtmhs.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gjanhjofq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gjrfxmwrt.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gxwfeegxj.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gcunjuqig.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gxeytvzyu.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ghavxkrud.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/glvfzpvpp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gyumshpxm.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gxxlczbkt.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gyfbeedlf.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbypbcenq.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gsizawzea.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gimvfpcyo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gljaepdhz.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gfkgvfqki.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/grcrvjkkm.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gxflhgpkv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gozjehguk.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gknhobkkd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gfhqhadso.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdovirkqp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gnsgmbals.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gzmgonpru.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gxjtyffcl.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gynebcsie.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gegfwwxij.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gvjeccewd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbxqigdvj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/giihszihr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gznhwhyap.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/grvmfcywj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gnqttjgtg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gnjhrkrfv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/guszypgjl.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gdbfbguvw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/golymdbnj.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gdbitupeh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gtmlxpyek.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gymysacic.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gmzzfvwbj.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/ghsknejjj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gmglrlwsd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gdfbuojtz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gbxbxfqhx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gsbvfnddb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gilltrdgf.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gmjmxclhs.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/ghijznxeo.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gpeowlxnf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gyewhrmdr.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gspenfwyx.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gdxpwkgry.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gymvwyfli.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gogrvsfln.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gglaovndq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gzqkprcqs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjijodl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gnjkjzcnv.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gechuuddg.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gnnlnfjdl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gdtmqpoej.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gfcjicubf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gmzhdzdpe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gqjpyzyxn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gxbljxgvx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/galevdnam.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gtupwtqmx.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gvtkoolgu.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gapvaxgqv.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gycxzgetg.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gqgeufdty.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/ggaubzvjh.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gjjaoauna.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gwxsuwxrp.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/ghtnxzric.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmrcbewkn.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/guadtbroi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gvqvrwndv.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/glpwmqlhw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gcthjhmzf.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gkbavpile.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gfplijkhc.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gojoobqpd.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gqgmskynj.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gqipytyvo.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gtiletxbu.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gvrfgapht.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/girkxudlc.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gybegozub.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gikqimdcq.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gvfcisuvs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/grmzdofvu.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gtojqebne.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gzbqpmyyl.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gyqppetab.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gimbxyvqe.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gzcmrzifn.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gthjftmfy.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gggnxacmz.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gkboqsyqw.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/glcwtkvqk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gcsalqzcj.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gvppvohrt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gwanjphci.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gbagbxzhc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/glwyucrhi.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/goqjnfslz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gywlilkpm.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gpxrhwshs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gzviwtjis.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gimegzuly.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjyevpxzh.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gbanfqrpn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gwvwlkwoq.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gauewfpzc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/glaskvpdp.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gmugirlto.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gwhwlozpf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/giwlytodz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/grwcttqxz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gxbrghwbh.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/goqunarlh.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gcjbqnumx.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfzmippmi.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gpsknnmdz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gcvrrxywf.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gbbccowlr.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gqpypwbxh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gzxdhklac.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gudfyymsp.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/grepuyxoa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gmqqkjhzq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gdqdvqpvu.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gzvcxyfna.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gzicqdirb.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gmobnmgdy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/girxahwqw.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gtvirlwyz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggarfubzo.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gwwsomigk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gywqbhfto.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gummfeexf.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/giqsmcsrl.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gpgsfzcit.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gjpnrvvvd.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gxwthddfd.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gfxhypjdz.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/ggvvsfbrl.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gmpmdnkcn.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gjsyqzaej.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gmjdwdvcp.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gnbvcrdlk.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gpwvkoxxx.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gquevnftf.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gbfwstwcs.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/ghpdlwbsu.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gnephwism.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gkwnpnvvl.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gsbtisshk.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gcbttosmh.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gzkadajmc.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/guuchvvim.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gjnishuht.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gknygwsgz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gldlkjwnz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/girkjgsbo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gdqkbspgg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/ggfxzqedw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gshnycmkq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gduxfskdr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfnxyrjwe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gkgvhmpbv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/glnsvenco.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gluqriqlf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gbeoyegwb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gcdjtikas.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gtbknxwmg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gagbbuqae.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gclhdicwy.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gsqpvnxht.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gobmuvouk.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gaalvaqzj.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/ghszewrvy.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gizuntznc.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gehvmupub.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnlwuudbe.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gjdtrtlvz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gnmbumsol.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gfiyzljcm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/ghhttjuop.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gaurcnupm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gbxkhomnr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gydjjtgfp.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gqkszuwya.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbrezopmq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/goreckgsk.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gocmvpync.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghgupfkkd.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/ghestmfxc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gjnywgfwx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gghuqiboe.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gpcwkpand.sHtML


<!-- 参考信息 -->