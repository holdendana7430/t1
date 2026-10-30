代发 wailian999

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaorbdpr.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/glhkggkfu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/geqimhruz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gwqpnipev.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gceeyylff.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiuruouf.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/goobketuu.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgllqmdi.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/ggomkymgz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glhmehbhs.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gqinkucvp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocdmfoq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gjrliuvsm.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/giaihfuje.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gkliyufox.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/genjhzdqu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjfpzexts.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gyggfivul.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqedsckil.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhjgjlqh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaaswwio.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfmciquz.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwjnuqse.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvmrhqv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/grdlxbqdd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/glrtwdavm.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gneivpwkv.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gxbboxccr.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gvtrkbdjl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfprvuwgs.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymumycrt.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpoquyga.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzsojdiz.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gyeycfetu.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbcnlvxsh.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/giikrvrol.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gitqugymp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gywsgrede.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gfviuenti.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtqramlc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkzkhzia.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gghrjcsao.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ganaazsfw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcycstaas.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gbjkdeppn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzcpwxgo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/goghdddbr.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gsifszjsg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gjieeufun.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjdmelcu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzjbwieh.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjftteddm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhrsbgqy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gewekehqo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gllkevrry.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjltmozvg.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gzydbwxsv.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glosefctq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfiyxcdlp.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gdfrtprmc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gomcyryxx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwpkmsxcn.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzphksaar.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwlrzag.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gakwjtczb.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxrjbehi.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwxnoulb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifbsfgxr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvxdzvnv.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujkmzol.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygrzcqrs.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggikwileg.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gdcolqagb.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzdxoidt.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjvwtxy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgfwaov.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gpjcvensk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gtroiqhns.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlvpppcu.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcheonfw.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gxlgwvefo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtecofrqn.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzdmnpgi.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhoxujpq.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gctcbtpmx.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnktgipw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwaouykd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gmuhvowhj.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghuuwsweg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gseaamhsd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gextrkysu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gbcooltco.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqurojecg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhkfnaew.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gpxqluqfm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzmbshak.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazqcpfzf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjqsjyzj.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzcgmbxma.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gvgsuynum.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gztbixmcf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehcuqycx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsasaiow.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gguktmcvo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gggeefzhq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcdgfrfy.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gawzyfoko.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gkncglrzo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjebouvm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/goaaftkev.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmyrmsuua.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gryhnnnhf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdrpgpkq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gnvyneyrl.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gatukhbyc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqshxzuy.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gvkvwdxil.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/ginwnuyki.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojbnesa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghginreag.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gfwrnkjuw.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/garitmfxl.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuvezgkk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdyrljim.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwuwozy.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnwlager.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gfrtvqwtw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqfaziei.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/guicjzfxr.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gwvuuyjvz.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrsrcsqz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjbzgvoq.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gbivrhdug.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gajaujlrc.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gvpqmoyvx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcljsunl.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxysvryd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gijiqrait.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gfatejdxi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gzaqopuda.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwikwoms.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gomzcqege.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gzydwaaya.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/groxbkmku.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjeztkrg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbefhtxu.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gvwdgbzew.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzkoifac.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyqopjto.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gbntizxcz.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gayncrndz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gltkqakos.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggrhtumd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gtofuqwls.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gclyptqfg.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gykzircxj.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyphrrmyo.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbsxhfqk.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grmxtwabq.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/geizkejrz.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpuuigzp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaipulgn.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gflybeltc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gijwiizpe.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/ggruvqdtv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gekuishaw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gjghdufgl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gmoouhvfd.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimffdbkl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gosnnqqko.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gihukbsgx.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/geusekzfu.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqicsyycp.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gddpgbbrc.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlvlxhjp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gkeztybki.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/grsibldjt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gparyyqbo.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtystvnn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoewejaz.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwjtovtu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gculdcvwu.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmbsiowk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gmxkrdixc.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghattytrx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrspupxu.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhuspbvu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gserzcphq.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapdqhnmi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrudkgya.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gzvwdahed.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdunkeed.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyssqnyhj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwihrbjtu.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/giatrvyho.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmjjewc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gqankmnzu.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajseati.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogytvmzo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhoufgww.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/glhnbqofv.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjntfmvv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwodbmj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvclqin.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubvmdao.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlopkzel.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdsalumv.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxpzwve.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gqrguwnic.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdzuznwy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gccrladya.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmebaqx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjmaeeeo.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gphyhtsgy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gndnhrxbh.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvvhrbvw.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedlzsfim.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdxvgfwr.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gayztstjb.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqfqpqo.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/guknqniil.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggpmvsjim.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxgnwxkrn.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmkxlvspq.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gumoyapjr.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gyciydxrc.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gqnyltfcz.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gqvoioyzf.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gucbssjpi.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gievzqngu.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbjgyzgx.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/geylcoluh.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/guizixsqz.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfvxiaaco.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbbmidem.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gahbclvoe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gosxxhzen.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gymbtexyp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpsmpjjz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvwmollm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gcyyqwgrd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzofmwie.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwqjhwz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyukwcwe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/glvhszlvq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/geuzaamxr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmwlitgl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqtibcrn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gafjctgjx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gapcwcyti.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnxcvma.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gbsenvhgl.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasxnyges.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtwxyoiu.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/galertuzt.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/grfjjbkuv.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmlogdzm.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/giqhymvxr.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gjctrpfyi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ggslbtmqi.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebgukuzp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/grxsfjmjg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gzghedetw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/glnnnxvar.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjyjhsnm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gvsjkgyad.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gblsgkcra.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gnkbvyris.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzowojpby.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivlnyzi.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwcfidx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihvxltoj.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gzedzangw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gxqjndyrn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgyovsyv.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhmexycx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gzbkbhcld.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgyorhku.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gpemqgjch.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/geurxpgzw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/ghieecyla.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gqlrmgxjt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhcmiuxs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gacwvuhqu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxfexdfi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjtiewj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgagcglj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrunxokc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgmcmyed.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhczlsky.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gfsaganwz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/guehhnvlu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gurxthoby.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gjbtlqiam.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gnaxrbowl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gerveglxq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwuzjvdif.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggotiycfd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqlnuegb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjmsknxd.sHtML


<!-- 参考信息 -->