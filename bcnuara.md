代发 wailian999

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gswpnmapx.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gsghiqmvk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gsszldqey.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gctidqicc.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gugvkhvzp.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gtjjkkaxz.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gpzjticei.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/ggckdpltn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gpwcucpbj.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gsyguuduu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/glcixwyap.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gdwdgjyuc.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gmqcwocew.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gyyjdekii.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gqcmicqgn.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gbkmypzeu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gadbdqaes.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/ghcwvvnyu.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gotyxmwnw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gctchaizi.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/grvecovuq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gdbzwdyak.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdphpwq.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gnahqtrrg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gzpfzbeuk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gqyjyzvng.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/ggcjslsro.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gvupboypq.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gqkflhlhq.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/glnljvjpa.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gallvbesy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/geppugpqg.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gadsxgwcg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gsgcsiggi.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/grxthmdgs.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gmzccfaha.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gdgwgqxlx.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gfkbfimwo.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/golaojyxl.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gwolljzvp.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gqqouvbhw.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gnfyibdph.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gdnkmvlte.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gbfkkrori.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gpmrffudz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gaejtuicr.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/godsqjljf.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gsdxxeeqe.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gnlirsepd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gqvpxikjp.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gelgjqgng.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/ghjyoluhb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/govnmtpwv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gkmnbrdeq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gozorqulm.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gwjritdni.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gyxddfbbq.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gykrnwbgo.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gedofsahj.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gadsepzup.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gimxekbdv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gotppmapq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gwmtcwlao.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gqcrqgvyb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/guwzxphnk.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gmfabrgff.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/glozkptqb.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gpbyqoonk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/ggplcrofi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gorjevkqo.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/glijiqgiz.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gytfklmnl.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gunyitebx.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gycqzlypr.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghtveaycy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/govyovztx.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/geuveyyfj.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gmcqqicdb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/glpukwilk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/goeutpovi.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gfexbmxne.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gbcnneztk.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gsesxnmto.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/grptkpgno.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gjjhabaps.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gcgfbxsbu.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/giuoijxsb.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/ggkbyofla.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/giaezlwfl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gndrejbyy.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/goshrllgd.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/glsbttrhx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gkrpugbxy.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gfhtkrirm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gbjyjuryz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxhwcdbcw.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gndtbkgpm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gwladotwt.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gdvbkgtwo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/ghrvlinbm.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gpfgwzzfb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gkwwskjki.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gteqrwssw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gxlusuwir.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gmjtzogkq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gfiiommdg.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gjukxuvhx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gdsytpcvt.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gtavciuwy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gypnkksyg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gbrcumblk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gtmnvvtxe.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/giwtwiyvf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gasswtbue.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gglishppc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gfzjreczi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/goyybknwr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gmwhziiik.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gwttlrraz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/ggqkmcayl.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gguoywssz.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/ghprksarj.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gpjszdixp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/glfilybgr.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/goiaolfyj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gcorfgkzj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmjlsrkdi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/glsbnfjaz.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gswtonycy.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/givrfgqkm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcevmof.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gpycstewn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/grchkrhgk.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gjhtfxeaj.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gjhtpnmrs.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gczrxdexn.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gjdttjtxw.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gizabqdge.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/glloerwdz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gmbwwavbe.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/grfvprnqm.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gtruigibv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gpwddjqkp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gtwxsqxwz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gebjhkikm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gvycvbfkc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gwiwzavms.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/grlcgdwuc.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gxqbzsflm.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gxnhskksz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gsixmvtrd.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gxsndhkcc.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gtwfwizxw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gexvgvzdw.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gzoyqhvgz.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gxxcuyldh.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gwoqxejst.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkaodqrcu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gnqcmxczl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gectoqqrs.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpjjgcwcy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gkpbzmkdz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gxwaniqin.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdmkdqhjo.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gcwegsgle.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gdbuaowkg.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gamdfdyoa.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gilprfbvf.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gluceoisy.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gjewiqhpk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/guenksgae.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gisojutfr.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/geyglohuk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/glgcgukho.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gzbhbhvle.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/glhuprkzk.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gissouwif.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/ggxqfnaza.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gayqieljp.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gvbegresh.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gzsoyowuo.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gkawhrfjn.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gceqyzjwh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gcqgdjpmo.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gkguinoqj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/guvrbcxtd.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gttmvvdyo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvjkgksoc.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/grnrzismj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gggzaiecv.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/giygjlxhm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gsuubxvvf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gmcblinds.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gwdsfwcnw.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gdgquaskl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/guhofmguo.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gdnqbivnj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gioeqrafu.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gkrtnzsyk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gysaysmru.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gbbxnwoqg.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/glutlfuek.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gnwtsubnm.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/giqhozwan.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gjulbuixq.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/grrmtjakr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gtogqxaqv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gxtfnzgwz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gnwqpelbh.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/geufthvas.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gymnmjgsx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guwbpdlod.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gsvajzwlh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gdooprrqw.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gdpgffyva.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gfqeizwmg.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gqtcdeiji.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/goxfnntku.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gdvyhojak.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gvccuwhfv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdgqmcxeq.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gasvibyqi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gifikospw.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gqqvikbwe.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/givjxemyr.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gbxqyryav.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gphzqnypz.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gdbhrqfav.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gfomsxkhn.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gqxcmvqfr.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gkhjmxdrf.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gogchopfp.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gjwkeackh.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/geflrtcwv.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gveeovkft.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/guodndtaz.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gpzryvnww.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gyxtmftco.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gucykfbfy.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gcxlgjhxn.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/ggzmnwofl.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxfzoqlos.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gynfmlryt.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gqhgjumct.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gfnggkyqy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gnoqypvyz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/ghdgshfoa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gysvjtgtm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gugqzlmqz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmctryasi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gceeldnoe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gmcztnxvw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gpsqobqvp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/goxdyyxhh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gpmepbypd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gvbhhqozx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjbclznok.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gxnwuskjz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gmzlkiawh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gpbkusnsx.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/ggalxmpsr.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gvnbpdqiu.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gesegfcio.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/grvkencji.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gtadsitfb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gouelufsc.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gikerjxzt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gigbtrqzt.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/guhmbxtkx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gbcbanfsw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/ghitxnhpg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gxyimpkno.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gqiarbekf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/ganflgjrx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gfwyxxqfj.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gcogdkvyq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gslsyswrx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gmxyzmahe.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/guneeditk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmlcwcuez.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/giugqnwot.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gepprarom.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gvzczondi.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gyezglnpu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/guxmevvvb.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gslojumcx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/grepcebnv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gsfyetbnd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/giofewuaw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/ggtlcyfal.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gaszvpsej.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gffkxeumk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/ghtdpgnbd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gpamkfqsp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gjncuaxpg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gzkzjwvik.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gsavynwva.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gaiuzlosx.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/grqofhven.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gqktkgygy.sHtML


<!-- 参考信息 -->