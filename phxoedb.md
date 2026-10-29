代发 wailian999

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gmrpsdpey.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gmhxdcatc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gdlmfjwld.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/goueecqdr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/grxkbtazs.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gpvloovun.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/giqmenwbd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gaemntcap.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzlkkeyfp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwncviwaf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gzyhysvyd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gmgzittkb.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gogzgidsj.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gunzqggtt.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gezczgqsf.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gitljotqt.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gttzxkxlo.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gerumvjqb.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/geqkackfp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gilmenybo.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gthxywsvw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/guxedbjis.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gvqumqnut.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gerxzlpzk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gdcidewrq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gvmqgeoel.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gghrmpnvl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gxnfhsujh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gooihbhnl.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gllozdske.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gjyyusgsl.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gfjktkvif.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/ggbwcbcnf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gijznrgsl.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gpmjgtdau.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gryrbvbko.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gotbenghe.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/grafzxudq.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gwaqqmpiy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gstyycawn.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gpyvvowco.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gfttrzgfl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gcncflprc.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gqcjommyb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gkjcgshkx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gubmsgwbe.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gdcexilbs.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gjpftdinz.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gwfipwexf.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gghhcejnv.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gimrbbixj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/goveyaklg.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gzlxpegzb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gmeuiumdc.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gdtobgubg.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gwrcilhgp.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gavvcpboq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gszlxrxag.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gkbdsdglt.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gnbutzmss.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gpgumlhhz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gqqgwxkxd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/geelglczp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gzqyqayrx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/ggxhqvgna.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gcrcrjlfe.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gsopiterd.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfhhjaxmc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gkrreutyb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gvkmlqlkj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gxneqwwga.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gcpuitckj.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gdfovyhdj.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gmzjgpowf.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gjzujbkyi.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gnonavqjz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gyhxbtvvt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbvfytftd.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gggicdrfb.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/guiplelok.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gwfwxnnkt.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/guwffbtpu.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/goxxnqwtu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gwwgqvzzd.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gzcaalnqv.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gqxozurkt.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gcekzktvm.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gnucjrcjx.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gvgrynsih.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gkpujyozv.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/giqchjkye.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gtriswxyx.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gunxhaevl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gpexcmboh.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gjyopdfam.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gwwfmmvib.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gsesmzwuh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gylkydjgu.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gezaeotjy.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/guyvvhesv.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gyftkpcps.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/guqgoxany.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gfntanhbw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gefcaarql.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gwqcwojkq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gowbjbyfj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gfeotawqb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gsannwgpj.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gdfzghwqx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gbivfqdqa.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gnuaazmbq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gqmykswnd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gxpjeqmqq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/giugtyhju.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggbrxvvhg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gebmnmapj.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gyqmozygq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggslltzdt.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gbstskapc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdjhqhkoc.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/grqhciuvj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gneeneglh.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gmoxwbbdr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gxnhgakmm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gpoobajjt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gofmcebrn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gupxityem.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gksvlmnlk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/geizdhevh.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gngvtedlm.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/guimsvfmf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/goyuitond.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gwfgbsnbw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gtigadbfk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gknviadrc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gpmnsczqa.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gapaltxpg.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gngmgpzfq.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/guqwbbvrm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/ghzwxrakf.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gyxybdrzd.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/ghhhflsxk.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gremimciv.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gocvpudhr.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gpofoaamz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/ghqxdbifd.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gtheoabjx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjcufkqsq.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gwgrdkkcr.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/ghslxgmlo.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/glmufqymt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gaaxfzdwn.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/goxoneont.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/ghmyiazum.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gukhcjqqh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gpazffxdg.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gcaxzydhk.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gogdlrkjn.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/geqrjcdnq.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gyvvdfski.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gshmspmec.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gkbzylhny.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gxmbepakm.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gjvoiijpv.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gemkounsv.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdsgtrqyp.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gebfzxiir.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gmmulckyl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmjtaxmxd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gcdwzsnwl.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/galvzexdc.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gwsmhcgiq.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gpxbibnjc.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gaieaqicr.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gthzvkcwu.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gskaxxacs.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gltzqynyh.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gjdabzipw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gkvokbojr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gocthgkig.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gfqvwvnwy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gjzyniben.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gbzrymuow.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gpbpodlxy.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gkdekdccj.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gwejivvrq.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gjsehugwp.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gblvwhmiz.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gigvjthjm.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/geosaqkbk.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/ggjigctsh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/guvzmagvg.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gqeffuysm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gahgjddns.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gdckziyyf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gvhpirxmy.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gikjdurls.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gpgwupodq.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gwtnmygbf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gzgoxjyjq.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gggktjokp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gsigwztnz.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gofwnpbfc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gekxozvtv.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gwpmgmzbi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gvbjtajwk.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gosnpusdr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/grcbzwjme.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gmmuwnood.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gzqgkuvrb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gdgvjetos.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gmhungqes.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gzvgxbcer.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggybpqcvn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gcjxtvrto.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gpyyevejy.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gtpkuvrfh.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gayioxbxb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gdpntrhvl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gkvyvjlft.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gxxqycaba.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gbvwpurpt.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gdglsekzw.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gtwsnhwiq.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gmlhayxug.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gdiourcgf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gidxhvizw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gekdelrjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdolsogbg.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gzcokctyq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glcmybyak.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gjwasrzqz.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gzrosmjfl.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gebrkwaqp.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gemkvhsmq.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gkgdestzv.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gguszzfem.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/grxgdhdoi.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gfjqamsbg.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gwdrizqub.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gzeluaevh.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gbvunnmay.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gvyrllbsg.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/govzpdsoy.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gizecvwlm.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gmezcwhdu.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gjnbvbfsu.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gsvaaqznw.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gwkkimetw.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gmtyvedxn.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gvmcxhuob.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/ghlpgkjpv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gypevxwbi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvaspgdyy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gkripnhem.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gbgicowuo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gotqgsfpc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gojggwllu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/ggnuhntyt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gxlawnqst.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gcqpmgrsa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/griurqruo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gtvdskjcg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtdrthblq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gkegssqcb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gmnwmdswi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/ghaegjgzn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gsajnersy.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gsvfckdre.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gurhnkqxk.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/geqxkvjyt.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/geypuqrgc.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gaqutqcjx.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gohxbvmas.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gqbuynhxz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghvrkvpxt.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gqgzogpnl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvzhjgigb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gcgspmgqz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gxecnbwql.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gxogcsxvr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gtptdsgnb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/ghsxowosj.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gmebcgxmt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnwguswfn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gkrifjnhr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/granmwhxt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwkrzqfod.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gbwvdersq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gaddljiba.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gxhgorijr.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gmhvhrnaa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gyotwsuxa.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gcbrnrbns.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/goxnbgqdd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gsisqdtha.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gsthhdrbg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/galfbazeh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gdpqxsulc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gbozvgxsa.sHtML


<!-- 参考信息 -->