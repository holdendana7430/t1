代发 wailian999

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/glbamktyy.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gspmftovz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gekyusbnb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjcoaghy.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzztgwqqq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gepahwear.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/grzmmbwmx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaioowat.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gabjaurgr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmplfcuj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/glvxjkgrh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqkooeyg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjyunzcz.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gehrgjpal.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gtkjplrju.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gsajihmvd.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guizwabgm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gygpdofwl.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gibscldfh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsysghnyo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwqeyag.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjguseyk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekpcxnrb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwsuflp.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gmnlaafwt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gqwxsrnwi.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfxevybg.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/grjjcpbkb.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gxiwugosv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdrofzwr.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gxpgdyfet.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmsqwsg.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gletliaky.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gcayoszyd.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzkxjwidz.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gsaksxsuh.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvzwcsl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gzilhxgtc.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gomvwuhsj.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gaemcjngr.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpzmokgg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxggcewue.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvcmkmnm.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gtauoaxyc.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gbulhjxun.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gepilopgy.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gltasmcws.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzvadauv.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gvpuxawry.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/grqccishs.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganjudjfs.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlmznaaq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gopwouljm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gkusfvrun.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/giryvnqzg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhdpjpqx.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/glcwlveio.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gyddkayur.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmznjrpiw.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhudyrbi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/grvphwiuv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxawpslzw.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwegpxolj.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gozdvcbok.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvsfemju.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxmisvpr.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgqkcza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkmpjldud.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwgtugou.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gulhqbdxl.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gbqkpjghk.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzjacvkmm.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/getoccnyw.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfbitann.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzxvptbz.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwabvden.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gqeqnmvoz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gayybifqw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpvteodp.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gnauwskdg.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoauvwcr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gofpntsmf.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuckagjn.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gukrqfekd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbpdtmjx.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxnwsddzo.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/ggghflncp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyejzzmo.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpmnrbdiq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebslgae.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gosapxjnn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlgwfaaz.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gzoznenal.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnpoanesm.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwmyvlsl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gybgxepqo.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/grstfbmnn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgywfild.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbcekgrs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbcbkjia.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghffztohm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmgormrsr.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gxkhsriyf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gqwysekca.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gilxizwcv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gklzzlznf.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfepqqgh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/groocxanh.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjnvwgnno.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gugjrooou.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbibfjsh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnssaewjc.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvntgifpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikvryupi.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedxkexfs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gtsmqgdyi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/guigdcmax.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gmhfdmbdc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glfsjntaj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbidlgdml.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqocpkpyb.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gnruqxouf.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlisvibl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gkbadoost.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gtprqswun.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gzstcapph.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnrfpwje.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gshosbtsr.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gserseghy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/grwpebqtr.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/goydyeiab.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaodpoep.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gveoaudlp.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gkgbeqmqi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvumnnls.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gcdqxsluf.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gohxacwdc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/glyrwlant.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gckdqdcxr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gotpcnzqm.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/glnktball.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsmefnhn.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxklkrggj.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/genngyvtt.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gobzmhgun.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/grvhnudke.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gikxrocds.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzmlwkyf.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/glgdiycwi.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gnrkibkyc.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtgxmtjc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibtoeohp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgpcqwin.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gaaivdoax.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcfpqetg.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glixxnyxo.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbhuqcbzu.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimyowrgx.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzkxsrmgu.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhiimfen.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gtxnjxyzn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthxnefkc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gdzfntmkv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxduktck.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/glxjnirdv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjztybam.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/guphvsjus.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphwawkrh.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/grctpaizf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/grjvdlnjs.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gknszttek.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gptcjhzkt.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkoxxxwfz.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gxxkucttn.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxtpbaut.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gayajaxgx.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gnvcbnoah.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gfvdavczz.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/genwwelxy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdljadcui.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbjqyfix.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfltcrrcy.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbgqhpwo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gegpnkbme.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gtmimbzmu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gdgpudyrw.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbqqpmyr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gzphqzbrb.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gleaxnlav.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzcnejor.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpwfukym.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gglchylwt.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsjzmpft.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkckptkgr.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/ghfntemoq.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gycjjlrso.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznltxyqu.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gnofwbmls.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpxllmsx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjqwxatb.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/golfurleg.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawxxtmu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gkutzwypi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqvbofpo.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gysyikgtu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjinqpexe.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gtvamsanr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddngfebd.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gfparmdhe.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/guxutznjw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gftpahtwr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gxupibkck.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyqavkefh.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gjfhykctc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnywdegyu.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gdvqmpgxe.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gwiepsxiz.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gucfixkbq.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gbkiszldm.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnskiuak.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzmpmrlf.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/grlogtjnk.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gksvowsbz.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gyvsgbsui.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzikxxen.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdbppuzw.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gpumvvmso.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/goxqrhfbd.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/glcicakzu.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiyfdxou.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gtphfghha.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grolrcjhl.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gmgxuvwft.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gkcpiprpe.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/grfeuvojx.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/glvscroxt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gjncelora.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwebkwmew.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gepaucwjq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gcqlyjzuv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/glejtjmfn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqhrfwif.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gedjwgaoy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gmrtsryrj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcozjbxql.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gpxttyvgw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/glqrfvghx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmewqvkbr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gwkvypuqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gogomalfl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfgjojro.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gprtndlin.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gmfywyhsl.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqgabbn.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyizxbdr.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsyyjkjt.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsvgwawi.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gdxifevga.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuufpixf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtcursfr.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gziulrmbh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gheuloazs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gnhaxlfdv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gprvkoroj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhngpqeh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gupowzeqq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmuadlfx.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsildpzu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxwfpfwg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/geisvxgyb.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gemhojyzp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcrkdxaz.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gtbnckicj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizclfres.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gendhaplf.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/glysjgzrr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzklbcip.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrlptnws.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gbdutrwrd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/glqfrpaed.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gbvbgyblk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gzfunnfxx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzwcguil.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdghlwguf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhxcmjaj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkpddvkc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbbyobk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjiuctga.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnuocmdt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnphfltpf.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoeelvjv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/grpshyqdt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gaitfsezd.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gxibecqou.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gluigdnor.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrbpzmhl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghirmhcvn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjeaprch.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkaoksvs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtshtzzek.sHtML


<!-- 参考信息 -->