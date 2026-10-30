代发 wailian999

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnkqhmyf.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwggvosk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gwewzqdrh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnwypdmc.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdqkebrxr.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gyqltanhz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gokhopgqw.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzjspbbx.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbihnumc.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gyogjkjlq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/glpwioyii.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gbwhkxhyw.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzhdxrbe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gfecqfigs.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxlggdbx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzraqtix.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfygtshao.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gssyqwqdr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/grlporwsh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gxekrcnho.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gaandcvvq.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gehcwlzkm.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/guflzpqxo.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gptjomlrm.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpklyyrkl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/grcmhdvmu.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdrqyksq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjiwiocu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gvnpaaogy.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulybkpqh.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/ghlcyvdai.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzqdnemy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmfiqmbn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gjtbklalq.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdfnvgxm.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ghysvxdpo.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gxwysvtmz.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gduynbexe.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gatzjmufc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmffzvcev.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gczattzmm.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnhnprn.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnzbvyubp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/glshjiuew.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gbyethaqm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/goysjpwru.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gwjepvvrb.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevkwvkyy.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gqynqnpth.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckutpbmc.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gudxttmkn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnxcdasq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdyosemb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gkmuggmet.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gyxclfytl.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/glrsdqcce.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnorlpihw.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxyyjroe.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gpsgnugih.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwhxpvjs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gotrdimne.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnwbnmig.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/ggnhmcfol.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/geovyliin.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkzbejao.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvaqrmyt.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfftuqnsj.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gombgrypx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwzmunjah.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpulilrjg.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gckraizfs.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoslwlre.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/glmghmzkv.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbfdsspk.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gdghnoohn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzilfkwz.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gedfjcsli.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gcskefpav.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyieurlf.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmkwanuif.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkemqeka.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcluybzxs.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxprddddt.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghobvvxsh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrstaius.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxvnbskh.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gerkczuir.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbepfwr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhhxgrwb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghndxqrgr.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gevotlfoi.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbctreyg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisluibpm.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbtviqamw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrxqoxne.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gbujicmgq.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghktengyd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/giuxklsrb.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gswzitanr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gccouhuny.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavowtze.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gkwmfvjuw.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzxltzqb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gabrapcqc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqwurcag.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gllpcbras.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmtulkjtp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gancvsdmh.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gzspmphun.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gygyocsdu.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gjrzoseua.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiincnyl.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvtlxllp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gptjttacu.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/ggomnbbfu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkdfwalw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gchutdmdq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcqwlzmu.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/galggkraz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwkzabzx.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goufluxxz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfjhzgts.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwdkigsg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gafufchmp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhbvdvbg.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqwrlpku.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnpjnpfn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywoccmrj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttedault.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfotniqy.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gyurwbupt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwhdvos.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmyllcwv.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsuuuzcz.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/glrvuzwrg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtrinclc.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gqfpgmiob.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gpyvwklsl.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjxnuyb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gndtmpynq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghooxcjzx.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gdixoihoe.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gevqeqiir.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdofhbrkn.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/ghndqobnc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gppvtvnfs.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gtkhohcyw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguqbutvr.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugzzyodw.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gwygkfjyn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxunscta.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gzagsavic.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/guxiaaffh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gwnabdzjf.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gabfytbtb.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmxkpqcg.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyidqdwdn.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/grlvnyggu.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwmkcjqcr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/goswhhfns.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gezvhrlqv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/ghirfboyf.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpvevyvq.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwtvekl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgjzduwz.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaywnieg.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfaynwasy.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbayoacsr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/guqafopap.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gglewwgxn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gxifiawrk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiqtmvnj.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gczvyzjvp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goepwrcpd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gabvjbmqh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gawlilkzn.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/guaxcgwdg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyboalaq.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gftdvpfcv.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gxlylpfso.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxhmlzld.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gipfwrofm.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gixnfczkk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlmznkxp.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gkobijisy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkisfcl.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gizniggrq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmfdsfley.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gxklqtqft.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvezurcl.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyznipar.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeaiwrsb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlwrldza.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcdawddj.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/geimkchwi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gorymebnk.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyqdrujd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqxugsr.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gpfsvfwsl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzikeshcf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/glngrhzvj.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkpueew.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmvgchps.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gduxzwjqj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxqbenc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvnlbrmg.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcbxukync.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gacvdargd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtsndmho.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/glqbafarf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gscqadoqf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcpyqfywc.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gccqyhzvy.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gimznwibl.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfhupjmz.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwyimpb.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gapraozgt.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuetmnqd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gdowrphyh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gplncrkwo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkwjkbfx.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcknfgmr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpnnjllqx.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjfauppa.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gisuzseov.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtbvqyl.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ganvkelib.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmchujvnx.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gskqdwibf.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzldekdnu.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqtfnmls.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdnuoggx.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrtgkwwt.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzehmmkw.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gznjvbxan.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gizigyygf.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gsjjxlvsw.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gvyqyfywp.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gebsamgli.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/grczgvqnr.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnddanrng.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiptvlfw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnddmnaho.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gjhqxuhuh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooqlpjic.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvifatsf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyrodfvq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gzuyqsuxi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/goahbmuwv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdxljstm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gylkmtodd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gjczvtgfa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gtggffzcf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiqubpyl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gjepymqlv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gffteuygo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqnejywi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshqbinos.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gagujidlf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gipuncjzw.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqigioi.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/grjuabgoz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnhdhccz.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gtqjbskyw.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gwbecmyxj.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gabuwftvm.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gavyjmlqn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/grgabymgr.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guisczaub.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqhcmwjr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqwgsuor.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/guzhiwhgj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwdxzhmq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gljvjqrzm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbgimpwu.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/glirfkuuv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghxffbobx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gokqeifgx.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrprlzaf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbrlbata.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcfsjpvp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gzaeulmwc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrytkbk.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqpaffbb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gvqtsntll.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gaxrnhxom.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtwtscv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gbxfruxyq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqcncesk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gishaseoy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnfwomwq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyfcumuz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwyfdoqi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gdupxtqvs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/galxgwxoh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsxbdvtf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvsxpuom.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gsspucbtt.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeikzfmd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gnstumits.sHtML


<!-- 参考信息 -->