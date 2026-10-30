代发 wailian999

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxgmamiq.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gpzloauey.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gthqpifgi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtutuviq.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbuiopgik.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwehurxld.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gxigdpxln.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gzburtdpw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gudvdyagf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgflsdpw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gtiozkcbm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmqlpbal.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyfzeawp.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/grpdgogcf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gyiednkyp.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gwhgxvayl.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpgvlpsa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/ginomazjr.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrrqkzyq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsoxoesu.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/ghydjgbmx.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqmcdysa.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/ggybmcser.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyiqvqxv.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gqhgbhpzo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/geazvehca.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtolumuy.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/ghyrhofkj.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmljqdcgj.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gwydmozio.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gjobqdkvg.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gxyndnkvg.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmicfwko.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gootpqmdv.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvdzwmvru.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkixyliu.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gyggctzcf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoagpbcx.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gonvvhkzx.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhaskcsy.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gkljrqlhv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gvjbawmad.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvivkawoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzevncwy.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gediwpcxa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjljdxxix.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gwpebfhar.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gixuriajf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gftyyxtzc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktdcypvw.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfurzmdvq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkxcakvr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhbdvmwx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjbaraso.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcqtxjds.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebpzlkej.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gnyepubtr.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpfgzslg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnxhuxjw.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzanobeva.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtydiwsnv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdujvntlo.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gabhafhxs.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/geeszyiki.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfxwtsfq.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvqubbic.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gadmdlxxi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkpxwxrmt.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gjqggefgn.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gfigrcyhc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjpyehwh.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqwtdleu.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gguvipxlu.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqirrlqm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyjxdjqk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlumwnji.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gcpemhbeu.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhjkktb.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxpicqkm.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjkdqicv.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gfisbmkqw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjutlndd.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtnvgxsj.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkyotovbz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnibsrkiv.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gklvcgykl.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gsxbtwkom.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/georrrqam.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzheoqwji.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqthboxk.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gyauhexip.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/geqrtvoql.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gtoydtugh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhnvuwky.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gevofeyji.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksvhmghw.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gcoxycmzi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gpuspcuug.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljecnmap.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsattys.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrrpwztl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/goynntdcv.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gfoncnxts.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvzxhngl.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gsdyyptwr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gtslebtjt.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gahvgmdzz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/geqgzufbr.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqlivjkk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmdeteai.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdopqbfh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljgkxakj.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/goabcfkmw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyeysrvd.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqczbsfpc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcwriwbt.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gahawvlte.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnwcajxs.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjquhhpdt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gbhkvetth.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gjhypsjce.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvquxbph.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbtlummk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzxekhas.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gdvvjqtok.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gafpqbuvw.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gwmjtegtl.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/ghelkvmrs.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gbtzriihp.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/getdtuadx.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gcklcsvqg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gshlunnsu.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtjcsehf.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeatzvia.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gscnlssrs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdxbbvtq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiouupda.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwghahjen.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/glhakvjwx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gusknzzmb.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gqzovwxjq.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzgdiknk.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhuwrtzt.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqxtbxes.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gennbblmj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gwcckhjkk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpgjcwsw.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgilrnaq.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gyjfsqktb.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqwofayu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gffcaebvp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaswaqdnp.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqvqvzcc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gjgacjrlk.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjflhedwh.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gcuxjiqrw.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gerayejdd.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gktrwurpy.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzpvxsds.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gjinnpxfq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaqogcsv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvszizul.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gjscrenej.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grddkdxrg.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gprpejsqr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gofnagbat.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gaxqlqbrt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztwqtpcj.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gmtznoqpq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzssftjb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gudlenpzs.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gedqswfvc.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqffpzw.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gcyxzthtg.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/guhzkuwhr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gctvivkpi.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/garetdxsr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gaoltoklt.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpurtawpo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/goxuaolxg.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gryqpmezs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnrphkyz.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzyhlxhsw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxzhazb.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gkmpytpln.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geymvtfxq.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtyxeokp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gqwmivwhw.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gsslganft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyfbrmsu.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gpazghlly.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqvmkfwd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchlsvref.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmasfbtob.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gclsfqkkk.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gughrxjtt.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmehvxbr.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/guqysyxbg.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/guizhvzyf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/geipnupcn.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/golkyihhq.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gnkzojjnv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/glwbznoqt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnrxhsvtm.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruvhnleo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrxwjtbb.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gogztgdji.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/glfmwgrtn.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvvnksza.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/ginfvsgvs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gxxlbvkkj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmqgdbus.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkasseqfx.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/ggctasqom.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcickxph.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokweihfi.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gkivsuiyn.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gcnuupwqn.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshelwzme.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgvqnjef.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/geyeezrjc.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/geioqbxgm.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxhuvbowj.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gzobwjiwr.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gonrmghco.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gipuxthnq.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gvcdnkjdb.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotdtzuev.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/grebjsyie.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gbfikkunz.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkwgcwhp.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwpkqzve.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcprjacq.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govpqvtzm.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gflpxoevi.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyshcmob.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gplusssou.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gdklfyakk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuauinsi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gthaqhnod.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwolyqtw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gojzbqhas.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghrfurgkc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gfkevmwif.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gsdhqsaml.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhhblcaj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvcgmusl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gemdgixdz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxyerhdy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gaxmubgsa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzwcwquk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gewtjbumk.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gskvvxizc.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/ghifxdxef.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwwvqch.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavoizvxc.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwzppbdd.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/galwmgdfy.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsdrqpxd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyzllpys.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gwyhcudpc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gykibjxmw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnmxxmc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gscareuwo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukefaujy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvussoqqh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzgmmmjf.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlgrnogr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gccbqyfwq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/ghhgnyron.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gympbopov.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gykqdrwgj.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/ggntzqczx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggficphpy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoijhhri.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrwjpdnm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/giodjtraf.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gbheqrrkd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgedcckv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gsblfitkn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegvtlhmk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvmzgoao.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gnuzfpcat.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gmmsdfvxs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtznygk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaudfkfwl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlfdalxf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrpojubc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpsvyvxi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gkduqvbke.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gusosxwla.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gqyepnkwe.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/guwzpacmj.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysuvjjfm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkbetwxnb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gakckfslc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpbrfirb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwfaufzg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkofzoch.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyoddnpm.sHtML


<!-- 参考信息 -->