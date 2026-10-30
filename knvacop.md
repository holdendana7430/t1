代发 wailian999

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gimjmefur.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/giepluyqr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/grmnwtpty.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gwcomxsxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gbzttiwew.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/grqptiilc.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gekwbjkos.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpusdymdl.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfrdnmgz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzxuwgat.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggzqmqmnj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gozsypgor.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gprubhgpf.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gygieigwx.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwcxegsq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztkppdpo.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumxarvkx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gpxhyiigm.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqomhlgfh.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gojgfvzzw.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gzzemshat.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gmfiyesho.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gkjitrkcc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrgcebva.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcoonfos.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/ghuflmjmx.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvzvaguli.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjwrvqde.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gutknhwnk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwqvcjcw.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gymvaufei.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gxuznyuar.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtvholay.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gcjwrolhi.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gressrgpo.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gslxcireb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gllddtkwm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gskknwntm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiyevwsy.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrpemdc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gisqgyzsj.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/geeeblrfk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/giocmvpvc.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtyvlqah.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptpajauo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gsblbhfrd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxkhdyyk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/grpjpbmqy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzotnegj.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfqyauzg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzukpupkt.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuoyekyq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gogiilwyy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/girihgrkp.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtswhemva.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylkbousa.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gtulfbnot.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gvzqdfpnh.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtokypgz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaavsrqje.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/ggiqcpiys.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtyxxfvm.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gftwtbzmr.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzjzhrwng.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeaxegxp.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gpjrggirk.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gutowyzer.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gacuwaaqt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbsynryz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gjjpodyto.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gieevomfw.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwziwtcn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsghvqhm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtbmamrb.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjifbtfzq.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gumremkva.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwvbxmis.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giwhmdbqv.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjnqazuk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/ganmultaq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gknouqqkh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/githlfags.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gzioevils.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpzvpnly.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqxnnvbs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdbdapum.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzogwtjh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfvvlozz.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/grylgsktz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grijjvkul.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvlakpun.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfsfrkxv.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/ghknyecjd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnisdiiu.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gyrqttfxn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggzgyznuz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzxmbjap.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gwcdwahrf.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzpofmapp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpqgpyxs.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/grbnbwvhv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gukhurkni.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/giompmmre.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gzwutlgvn.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayujfzfd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gqxykyuvu.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/glgvevftc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gzvgrhzys.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gjytxtdzg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gyonvyrsl.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyjgyfaxr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gkyccxzkq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfdfevol.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/ggyhalmyt.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gfdjzygck.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/glvskhqek.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gbxhsckgc.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbjcbxuq.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gpwlztnkt.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gmbdpblsd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/goybuwgvg.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/giidmqsay.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/glckieibs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhscvxr.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzoregqa.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtvpzkv.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gekmndohk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gvemlvxnu.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gipcfnaiu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/grlaiooxb.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gpcnkpnmw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbazxkvht.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/geskmbppy.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcuyxijg.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gldxavixs.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmcqrvjc.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddwysnq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gjnukfenu.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gfgpfjwnh.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuhdtieb.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gsepjyrvz.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqkjfgqn.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitepfetr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbphyzfv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqcndtqu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkdnmzdn.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/giwlrqtnp.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gexfeezhb.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdcbpbsg.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgtzsctm.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcqqmeyco.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gjhitzoca.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdfrrlw.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gfebmqbca.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzdzyzfh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/geulttpik.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/ghrfokjtk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gtwgmwnlu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzphounpc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gmcbswtld.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gfufznhii.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyddxpaf.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gaibyilxh.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsybldjaf.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzjjttjog.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdbvqoxh.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghekinank.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxcvygrw.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gufzfnbth.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gloixiqxe.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrkfepf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdcymbhf.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gzblndkkb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdcowrovn.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjerjqkws.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdklimqw.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/grfbcsyzr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gqswzkltg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlkyooxx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gycalkffg.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gbszerlsr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybplltek.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gsknpofmb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglidfpef.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzhwarsm.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/grzavmfkn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghixvcxmc.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gilguxitj.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gegvfcsnu.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gtcymuyhj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdvuswflj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwusxjpwf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiscenkc.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gbdpyvyib.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gacsbxhrp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzwmyvqq.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgfpjrww.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjmfcmd.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/glgvsfsqr.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqxytqd.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrjbrtme.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goisnvqqd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvfeaaec.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmfbmho.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfsccraf.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhublrdv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsburerwv.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlgwixwi.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzuzwyuu.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjghigq.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbboizaf.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gtqhiysew.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxrbwzy.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gosioiliv.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvjwwdohe.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gamwppdde.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjwesxry.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gavlwgqdy.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gyltzliwe.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gygkmjqql.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gziryontu.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gtncdojsk.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/giptyofkk.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/grcyxqxcu.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuxbmvqp.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpzydmx.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gvvgogyml.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gxgnlsyyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/ghfjfxsep.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gegyzpemd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaykmzet.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/glzzffvcr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjbnuick.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyuaensq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowraurv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwiktpha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqidgenz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/glikpxjrs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqyowuben.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gybckrrus.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gushheymz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gsoafjapa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/ggzomnfzx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glzqffdgx.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gklhesfys.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/guiitxvqz.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/ggssffdyc.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gwhjjaqeg.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdoebulo.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgwcijlu.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/ggiqswymz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstmrtzwn.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gkietzysb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjltqxypx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgdcufce.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/geunarscp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gqigimqty.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gfmoatvse.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafmvprql.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeeeblus.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhwdqyei.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyaaouxg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsacolag.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrdnzdw.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgdktgxo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gtjexcdxj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/grqvaaguc.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchscxoti.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznyxbikt.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptnbvbwp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/golaxlwxp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/goaoeygds.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gnrmpowfi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtkobrue.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/giddlzsor.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiufmncg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfigjjjsc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gmxolywoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxaquhxx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gbhvixzsh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyolfrbea.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghficaviw.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gvliluhnc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gdjueuvdw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gprzpvgoz.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gaexnmsqh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfyzfqvz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsnelbvy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giqxqkcaz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grfwccrex.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfqwtfkiy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqjokyxod.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnirfrdsp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqjmmfpq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuasyhru.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gijhiwjll.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzwoifcsp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gffjpvsan.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gauntqvwb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghahkehxk.sHtML


<!-- 参考信息 -->