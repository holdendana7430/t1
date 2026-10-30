代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrtxlekz.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhzuwkwg.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gndmqcvua.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhjdlrxx.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrryugc.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdoxqprf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwghbkdcm.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gbostiwon.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gfvrtuivo.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfzhzata.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozzgmsh.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gaqhskrsw.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmipldsy.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghisynewi.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gqeflfamt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslpqihs.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnqryfbv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvotukyrk.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxejzyia.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ghxvoxhon.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnfimbsw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/guiwdxucr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/glaxpaucy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkepljxo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gbzvgnozo.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gargeocuv.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gunawvajr.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/glzvlhgtk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwfqqdk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhraiyvl.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmetfotv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gzmnyyrxo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gtnryceiu.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gsnndbffw.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gdumgeyav.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdujzpgy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gvraewsuz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjidnrvfh.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxzkppdr.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllcdchnk.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/guwoatxix.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzbbhezm.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gryqpihrl.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdsfpgwi.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqqvhwsn.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gzijhcgro.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuwftqll.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gnqwogaig.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gistasizm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gfnxpbcqd.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeizclfa.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gufmxzqcf.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gxrhdfdka.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmfphnl.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gushmmoqp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsrwfhgs.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gktypflxt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbkiofuv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gilhgeirh.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/glugyxvrc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/grskimoxj.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyjvogep.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gmhjsbqxu.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gawbjvqgi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gssgcpgxr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gixkvuulq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnurfqsbx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzgjhsslv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbckkxiqb.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gqhzhfmao.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gccrfzjgp.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/ghrjexraj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlsnykxn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnpetcvpl.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gaabvtuim.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyqegglz.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/glmcyuujt.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gugrjocxr.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkmdakjy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grpmvisbi.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gcizbiwon.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gtufpmclb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxycptd.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyzcyzob.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gqxwlabyi.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gubyiteht.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmloagrkw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhomgmnc.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrwxzmos.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gkoelpguw.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcrkcjxr.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gdqegflth.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geccuwxug.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsddggbee.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvpuvlzfs.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmzpirdp.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnnwqme.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbsrxxbe.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gtutayqtq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufiegkqw.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdnxuchl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqymwwsol.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/ghvvqdbze.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqzmhpok.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ghauxkmhw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gtegmnlvq.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gdteossdw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfqpozwk.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/grqqeqosf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoqucivk.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtujtalmi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gkepabwbq.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gjpfgevji.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giovinzod.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gwazxjgzm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvharecgz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gxuzgaglg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqiwcnsp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gnfflxjdv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydjhadl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gresffpwj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtdbssym.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqobnqrsb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfreukqym.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gyhvxrgyi.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gjdgqqjmy.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqarjxwo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwpfgcpr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gpeucebcv.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzahuzuy.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcdfhibal.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkrmcntv.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfzwgsbg.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpruygjzf.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/glvooueiw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwnlqntp.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gofaqdqhk.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/groresnfh.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gotarceup.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gleplllav.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gopjjdnbk.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gyatikotq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/ghptcxkhj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfemeezqr.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gswmdxcqr.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gmptfvkoi.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gykxnyolm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmolpadf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqsmoijm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgbjravm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gaujsovmw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/ggdtrywkp.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqpkwxbw.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/ghedvndbo.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/godfmscfk.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxiyyukt.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gyuifujsi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gidyljtvb.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqplvmhsh.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjfhxnug.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gwnqzkkzz.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcgqkeip.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gluohdztf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmcmxjrz.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvwbtccv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gijilpikn.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gytelgfml.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaojlwyb.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejehculo.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gtlqqdopk.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtlgrlfpw.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaopsffbw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gagvrcyfs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyilzqbf.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gggigmunv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydpbmgiy.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/glnbduouv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ghrjkgtco.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gxjrlvtzh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftderale.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhnoirra.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/ghxtgaryi.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gryifqcxk.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gwbwaacoe.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsplftuof.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gyasypeay.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/girhlvuvy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/geglltrej.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpiedjtk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gycweivdf.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gqkgfsvlm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhdtsfw.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjltbkte.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcfhjxtwm.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gvrvskiuf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdekryhr.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtjkhrnr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyziiggmb.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/grpeszarv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gosprpwrh.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdaomghj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmbjomnf.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/glpdifgao.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyxchejh.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gdggoohtd.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glytkzhju.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gjukcurrk.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkkqsxoj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gospcvyct.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gldnjsexl.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gyziosfqk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gcdlugutt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtjqsmor.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gondqhpne.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhxmzzxa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwcjnugby.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtchkla.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/glfwqccxp.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/glmkmrquw.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfjhuor.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmgwkgg.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gqcnvqcam.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gkqztdlep.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvwshbih.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbkgyvtm.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvlkkjj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjatmkgvo.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gvqfpnnti.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gddbclwxg.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdvulojp.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqavewlzm.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznndgwmv.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gxxytdhhv.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbdgmpdrx.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplxfzef.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubcqjnqm.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvsffuyeb.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzaogaet.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gsulunkub.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoywtiop.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhmbbuje.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gjvlwyniw.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gadbfkhuq.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givengwrb.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gajdzbejb.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gopcbjffr.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gdxbmbvlj.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gababjhfs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkerngkgx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvteprfa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoonhtgk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/goifhoqjm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/ghxfcdrjr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswkouyjt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahehpgaw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gkneemgrw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gcuxodman.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjsqivbs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gobjdsiaz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaaulqxt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gewcvfebi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gatsozxas.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/grakhqgoi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gydjoerop.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gavdibgeu.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gjjuhoyis.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhdexzzr.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gueevlvtv.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gbejyabre.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gqhnjrdou.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnofeyni.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/glfapdick.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcbmiwfo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkxmqqil.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gdxxwjyub.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkheezlbj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxyreqm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhcqthrr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfedygn.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gthkerazz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gddqimqbu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqhidhsz.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmfdonng.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydksjghe.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjseujan.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gtmzsaxys.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gumcqewvl.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/godcxbjdg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gyafhyhhc.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gxcowopxx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gcrtenacv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gpuavioqk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gjymsbtnz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gsejyjdvf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/grbqpnhpx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/granlcdpq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/govyjwxqd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gfzsgeaoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqdsbqy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gcvvkwfaw.sHtML


<!-- 参考信息 -->