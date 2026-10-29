代发 wailian999

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gxfxemfci.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyybhwtnp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gqxrgkqrj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gbbzxjuyp.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gyfbeeuez.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gadjqkqrw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gkihaqtdu.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gmoortscd.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gwnegtdvn.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/ggfpajman.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gpmdzdqnh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/ghmepthhi.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gwntkuhtm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gvgvbdmuf.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gfnvowzms.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gubtqndzr.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gtmhldaht.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gwuyqeznl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gyijktawn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gdxfrnpwu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gsfyxpvoj.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gszglnssr.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gfxfsjwgc.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gfhodhdfz.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ggmudqydn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gewcjoumz.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gxicjewmw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gmmkxvuzw.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gfclymynq.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gvzgappbn.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gudxluqdi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gpfqiolzu.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gsvqlfjwv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gddjsqbks.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gtqfqqsig.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/guftqloma.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/ghigwgfce.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gdvghjkwc.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gnfhkbvhe.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gigzmcgqg.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gshzervqt.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/ghpylnpsl.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gvjzdkctb.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gubmuocaz.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gbexgnsvm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gbgxbvcws.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/guhwfsibu.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gvokmgdpr.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gmjnvbvzl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/grhsmdjzw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtgfzbh.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gmkoiefpi.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gzjiyjlfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/guwadhfrw.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gxcspajee.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gykhnfumt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gjfvxvuac.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gkoarsijo.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gxnlzrddt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gjchjijtn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gyaketvja.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/glpsiffkl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gjqjzqzgz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gqtvufthm.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gabsfqzjo.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gncrslahn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gtlhdddxw.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gkgleleoo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gvytkrvov.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmnidgjj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gpkvnqzrh.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gawfxhpzh.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gtdxuajoj.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/guvquildm.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/girnlnadd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/grttrevev.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/grpwllrus.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gwgwivtbx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/galakqbxo.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gmtrigjfe.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gojaqzhly.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gzixohmwe.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gvetwexrx.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ghpnmdaif.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gaezyksjj.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gscxlrhmz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gntqahffx.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gvgogbzsb.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gerrlczbs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gybekgikn.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gtnmjpgbq.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkubrphow.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gqlqdojqa.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gcgizvosy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/ghgmojcee.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gnxrbluan.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gigxnwmku.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxfyjfhlu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gmvcoxtys.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gmxduqunl.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gtdsyygva.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gbrboagbp.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gupntskdi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gpltrhmxg.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gqlqzfdoz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gbzspnssq.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gfosuhvgx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gpytdxezy.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gfrevqtsa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gytjwdyew.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gtawbxyiy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gzkcgidbb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gqffrkvay.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gbzpedyei.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/ggwfiskmp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gcoarifib.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gasgzeprf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gqrxfwqrm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gsnbnoiyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/grwocsvhb.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/ghbbfmoay.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/guimkzzat.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gmtquopeh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gygnonyiz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gvnuglzbb.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gjqmajkza.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gunwpnauj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gxvgpmvrp.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/guzaabglk.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gqovvpagl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxnozikqp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gwxwccnev.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gceyndsss.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gseiaigts.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gohbtvcai.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gqkbvqnap.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gjcolynom.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gvlueqrmo.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gajqpjaok.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gjotxuwtj.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gkkkzyweg.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/guqnnkkig.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/grrlfhzuj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gotbpvqrt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gxzkaqriz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gxactmria.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/geqwewvbu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gkblmfypx.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gvmsvubxs.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gbpsmucon.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gvsukhgzx.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gbztygxqi.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gejegberl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gtlzpeaef.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/ginycicdv.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gjmahpeal.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gdiyyhlar.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjtwcwumo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gxsybhhlv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghxjvfasy.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gxfktklna.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gxxvcmeqt.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gzevxzjcl.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gsayekhpm.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/goquucccx.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gsbbdustl.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gszuiasom.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/giwsusykl.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gasizvdxo.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gscouqbit.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gdpmsbueq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grmgegyng.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gsauycpzf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gsqelswgh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/grsrtskcq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gvkurqmbn.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/guckxkvsj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gyybwgoww.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/ghgqtavjh.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwzsksjwz.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gpcfppycw.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gmcmitpfn.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gcrmmfvov.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/ghvuqedzj.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gbzbdprjr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gvzopaacd.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gwvogrrct.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gqhioohgc.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gwhezkhji.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gnveafllo.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gveoicymz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gwovjzvfe.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gkiljehjb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/ghtwtegvy.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gkwrfbpcn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/givvylpbj.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gkviqrbgq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gxcmlekcv.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gueuegucp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/glclnwfbu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdfatesab.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gusogawuh.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/ggwgcsymj.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqyiqygpa.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gxhurgcki.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gnoiyoygl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gxerfqant.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gveouzrca.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/ghrlbirmd.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpbedhelf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/geklhwqff.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxefgjedt.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gaqdtfvap.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gbmmeylxg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/guitahmgg.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gwtocornk.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gllbivhwi.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gjbiyojgw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gpdppgbgw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/guutilibj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnpcjstoh.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gqbxmxwnq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gptikcxrt.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gyyravphv.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gmeyzsnjz.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gjlyednrk.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gkrrmtpuv.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gwfpcgyuf.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/ghiqhccog.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gafmkxgvq.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/girowryxq.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gnpfvtvlw.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gnvyyjxmw.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/ggwudrbbz.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gcezwcyki.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/guphmohis.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/glabwkyix.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gycoqhbwh.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gqmdsmmsi.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gqhxoufua.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwawaoqix.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcgzrbpwu.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gqhxevyov.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gthndziuw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gizgxcebq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grugdghqm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gzjuflzuv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gegjwwlfj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gjgglduhr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gmgzuhstm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gwnludryb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gxhcssidi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gumuqlefm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gvtoubkow.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/guevwuygo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gblwfpoxz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gaffvoivt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gnjyyyinc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gwxngvqgz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gfwrkkdzm.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gkjsbchiq.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gziawpepv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gjqwdmdgf.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gdpoxgtwc.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gesjxsude.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gimdoadgu.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gpwnocoim.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gdxhucpxi.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gnniddtxm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmrqzegdg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/glxobrwki.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gdjzuijaa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/ggqohyzck.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gclrmsfau.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gnxolrvca.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/ggrscqiea.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaofnjhkn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gpuqiyhwe.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gvrjrlcgj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghvpqveep.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gcglwipai.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gfipoyyes.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/guonikizh.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gbowiyefk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/ginlrjpzi.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gyoijkooj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/glxrkhser.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gnhyvighm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/grirtwwpn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gwjpxkati.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/glybmwtwq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gvlfbcapm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gnqmdhfcj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gxwrkdbkj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gogjzzsfe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gfzmozwov.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gagwduntf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gydfszkxy.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gittaxlri.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/giwzelfzo.sHtML


<!-- 参考信息 -->