代发 wailian999

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gmagzqvsa.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gqzkpnkjw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gabmomomg.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxeicbtr.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorjuxesd.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giseapdnv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjuynomx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gybqnixdh.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gzqsaueov.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gikysxdar.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gtjrhzodr.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gcamwscgh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmphgogl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gskmxxdxt.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gwwynwviy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsksqxzkn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gagpyajri.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsxaelag.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuvlhqqn.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gybiclwfc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbpxgibj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyxulyvl.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gozxtolxh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/glazokfdq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxegapar.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/godcplzgt.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnoadcrg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gdfiygkqi.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzphkjui.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpoyekle.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/grfdjhxcu.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gpufkfmep.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvbacnmz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqcfpsda.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/glyjzrxpq.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gbhyggkjn.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqduvgxgr.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhjujcvl.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjhbejbv.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gctqrwswb.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqpmwijh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/giteukcra.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdjuhccw.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopchczos.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gkhyrnsek.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfaugjzo.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkyiexkdl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemaaymnf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxxpsded.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunaxhcug.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gkcvddkgn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gouusnplm.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwtgchhv.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gtybidduk.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gbdlhtidl.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsgboara.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxxbcorb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwxgyjkc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvdshns.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvxlxrevj.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdirbsumm.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzquyqnkv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvfnqrqlw.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxhhicvfj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfjmzwsaj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfjdqtao.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdthwtabb.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwdfgajx.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxbxkdzxl.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gpqetdebg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/guiudgbdm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghatsnwjx.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlvtbhhx.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gejovyamf.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gsxfojlbt.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzjehwyxv.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlxwenti.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsdwbrf.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gctrwxyqe.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gfpzkegud.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gjsxmqnvh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzymaiyf.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqtreanc.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gmrooeref.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxfikmey.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmofrsjz.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbzlvezuc.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfiexbwar.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gfbwyhvnb.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghdnrlnlp.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyccnyqdp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvwullwt.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gthjnshid.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gbfpjjxnq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkpgmes.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gzzjddssz.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvgcmict.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gcoylndmn.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gvaieymcf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gwqhxzddk.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gelbienzh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgehnpot.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyfblwum.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqhnoydr.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gthitzshf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glfkfikyl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvllkxxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlruhxmn.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvgbwriq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyantgfjo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/ggnlibonc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/genycgawh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbcmlxc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gtezkskci.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdqstkva.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemlntfua.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gtmwsdsjo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gjuhydzwo.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtzndwxya.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/greylvalc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gsdplydaj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkskzlln.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpdlezno.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqgbsuml.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzffulvk.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gdiivtjdy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddslyofo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrbmoyvq.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gxaraoonh.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gvpgcjvxo.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzrovjfe.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gxkltcjzd.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gofklghce.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbyxmieb.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gygbielga.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gtutprjti.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxniruar.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gknbinrgp.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwiftnan.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbqcucem.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/giugenbcu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gmytmiwge.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/giowhlusn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfdxpumt.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwcpwlvl.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpatidamm.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gxngmblqu.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbqezbdz.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gsstyzejb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gwpcksplh.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/glifqydmp.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gztmegvfs.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gulqrfrhd.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdqmdban.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwibqtfcp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gthndiktt.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnxezrng.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/grjgazppy.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvdznqggr.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqymyqgag.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahhwobwi.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gpgtknsax.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbfrfpiyv.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzotqjy.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqusijlhw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gkxvllnno.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxuxjauw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/grtwyoame.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gufwpofcc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/grnfzoijo.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gcvhyofbe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gzacvueob.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gzneyajkh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gnwziltgi.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpclrfcwk.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gitftlflg.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gfydipkre.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gljgulodk.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gjtxtsovl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/glufeperp.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gyrqdmvlv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/ghhayfdvm.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gnoprwzyr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehixkmuq.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoyvuzsv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbngnqst.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxwkghseg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/geryqjdwb.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/glkdsrrvq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/guenuujwx.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gnytesvtp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gyuxaiyfk.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gupembtrs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/grvvzfvqv.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gutypojqb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gabasmhbt.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gikxchdou.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurhozoxs.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gvgazkmfi.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzajvlb.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gkhzitwvj.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfivtryq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbujotwhz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxuwoxovh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudjkmgxi.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gyvasodkr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquezotbv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnylsfwqa.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gqxqoywgf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbovwgur.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gtvtwuabl.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gphtuvdme.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gevwlvgla.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyywzuiv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiyhcyyb.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gyshtnyvh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnieigql.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gktytkeeu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gplzypemb.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmxfxvg.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gxtzglyxw.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlrhibhh.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gswvbvlno.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxxgvpujt.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxklpghz.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/guwgvsxjs.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggtpkdwan.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqvjsafp.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxzaqmxv.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/giohenuzy.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gncfwsqmd.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnyvbtuw.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gymzqzbvn.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/geglspdgl.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gesqimjfh.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/grtgdcanf.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcckwsad.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guricelfr.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gycfwrotr.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gmukaisxf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/goupugwib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gperbmipe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/grewanwff.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfmtehcg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gxljyzknv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gclmpswwc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gtmgzpkpr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gocwtxtei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/geuhstpie.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gijdoapcv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpawbxqu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwranwwud.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gdimogjvn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gvjhhvlmj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gcldktzoy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/giwcfaowc.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzweuhkly.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/glbyzjjjo.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/giculqoii.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gjavtniho.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpelvvzhu.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ggojegzwc.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmxfyvn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfxmssegl.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gdytkzaha.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwkghyaty.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gorqorfxm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/glruqcdrl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiefjxlx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/grolhkypx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gtjfellxu.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrirzmdg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdqtfgsn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gadzdpkwv.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/ghouzxekz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhsqvgsg.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/grhjrrqdn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglnaufzs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gakudxkue.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gkeuweeul.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjouwgfd.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/goocrdfhv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gvdldcjxs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gehgpgufn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizhwpcqe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gpjwtyqxl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggriaoaqw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gipybeypy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvavhskqx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gfjbvsboc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyiwivzh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvjocxc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/ghqmdjmvx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/grdzmlrml.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gptdviylu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gwqqofasn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfdxlcql.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gxabtyiof.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/guezvjxjs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkqvrclr.sHtML


<!-- 参考信息 -->