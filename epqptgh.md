代发 wailian999

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gsgwfgfrw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/ghaiqtqbn.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/giiuwmllp.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gxgmzmjpi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gufmqnnds.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gozxwxqov.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gbvdzuyzb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gcahgmvvg.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpjuqscyd.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gszrdokit.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gvlxrgioj.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/geezbuflo.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gdwoalcrh.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gngmdpzzj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/ggihcuada.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/ghlbxhjoi.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gerdzdykt.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/ghvlqjejp.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gbbfddhiu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gavurmghd.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/goftscttl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gokjeykja.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/ghxejxcsx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gmqsaockn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gqnerujjq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gvzmcxuyc.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/ghipvtolf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gyphlsqzi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gmgdzuoyl.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/geuigndcs.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/goixroqul.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gajfsclrw.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ghrdgsvvf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gwurmxxcv.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/goinqjngj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gidgwhzad.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gxffglwjt.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gpfymdlsu.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gfbeomnzu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gxsxvvmlq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gmtxrhyxe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/grubbowky.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gfqtgcyur.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gpajipcfo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gwpbmawbl.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gtszatdsa.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gmyeyfdns.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gcnubljkn.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gxllilsay.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gkmecvqyz.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gimttwjde.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gfjawtsnh.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/ggoaidyng.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gmbwkzild.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gaucgwfzj.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gecdfjupf.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/ggjrziomx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gvxakwztl.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkscvivcx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/ghyqkzcjx.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/giywlgaya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gnfuwivcn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gyzkkpcqg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gwokcyghw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gnrbkdvqs.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gqwqkeppd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/ggdwaaizd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpsxnfcm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/ggyjosacn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gfnlespvo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gqfckplcv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gawvqkoka.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gkxzcmjdh.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gyscgylib.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gvlqcqrfi.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gpgskqiow.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gahhkbxmi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbxuteuyr.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/grdyrilrf.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gljukwikp.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gofuwjsyf.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gfsfrgpqr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gdesnqdpq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gfkqxrqsv.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gfckpekbf.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gasntvklf.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gdknvcfcz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/ggxueaxzh.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gcmtpcxsl.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gtivuqkof.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gnjwkzhyz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gqzxokvfg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gtiyxdsyq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gdonuqhmk.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gkpsudbnr.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gtrqpvazf.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gubmdiqmp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gfrkpkarg.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gnzwrsnbi.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gzzjnxdvz.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gzwotidte.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gpgagflrg.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gymanskhh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gpyinfwaz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gcdrovkrs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gafidrimp.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/ghvxzcmcg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gxlcethgj.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gktpdsvcp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggblznpnq.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gzzhrwxcz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gvjlkcgjj.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gemnpwbyd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gpwxnatjp.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gplmickno.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gspcrbkpx.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/giqdkoqen.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdphiofyd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gwitacolf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gwaqaalbe.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gvduwooym.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gqzpkbnuj.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gzgjwarjl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gtqsstmal.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gswgpgnvi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gwtpoewza.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gvzltwhad.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gollgzmoj.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/ghsakzqpu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gddwaqrqm.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gbwnbghdb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gvhrmacvn.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gigxjtuyx.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gpbccqtnc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gdzeogtdv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gsmxjvjng.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gpryofuav.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gbeuwmjiv.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gfkuoqytu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gxlqvrbfu.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/ghstpasux.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gfmukxnjh.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gyfspvorp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/glnkehglf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/giyswrgyr.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/guiaenvpf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gbjmkoazf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gvxasiaul.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gagcndeub.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gildchswz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gzxezuauv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gvpuwsbkg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gbsxqxcdq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gqtmrjlue.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gjrifwqpg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gcwenjvuy.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gcfsqpnyp.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gkigiwmoq.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gokxnwblj.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/ghwckxflk.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gmdowrbtc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gaubzllzd.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gteoyuobz.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gkdfpilgn.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gtoazczju.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gnyvmsyhp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gvmskicpa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/guxwduzzp.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnelnswtk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gqvsgaamx.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gtndubagj.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gywbxqyii.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gdbwvzpmw.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gxlfwlxry.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gkeiqndwl.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gohfhalkp.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gpewecteg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gkcvyzdxl.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gputohzid.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gbdcmzojc.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gwvmtmexa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxwrscpzy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gnythmzop.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gtrldttiw.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gtxmjuoim.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/ggjaxajag.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkqorukic.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gyqaqflga.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gxhtdeggh.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gvtavdwmd.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/ghowaaqxq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gdrkxbmui.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gromtvmxo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gwwrnqhah.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gchjxyicn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gwltqdfao.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gchmssxlv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/ggqznxutf.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gvjpktltp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gvmrurouo.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gszalfjcg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/goivlbktf.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gtksnzbmn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gdywsbfkj.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gziylrxpy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/glprsvfnn.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gpckotjoj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gnadfjokc.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gckfjiduq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gtrnsqmaw.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/glhbchvtn.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gqqfyepyi.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gtwkuugoz.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbsevgyrq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gsznrrcby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gnvoqrobl.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gaaiviofx.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggqibicme.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gxnbsabag.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gpdhbkznp.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gyuxdnkqt.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/ggixqrgjk.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gnpcvmild.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/grlpyhsjn.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gevmlmbvv.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gsltoggna.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/granqhenc.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gxokzcvcz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghddtjull.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/grdszxihh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gntfysquh.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gefcwioth.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/ghfbrsjmw.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gwvfeyeae.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gieapmwfl.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gbideokgw.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gvtbrlizc.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gnknufvpf.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gtfogsjcs.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/ghfgmappr.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gcawutrtf.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gmunxmbpz.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gbjwkqxoi.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gaupzmbfd.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/glbelgrgi.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/geftujwkq.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/giashxygd.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gouinljlc.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gbpwsnxea.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gdcmhujhp.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gspxmaeit.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gigdjjuca.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gbukovaou.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gautwznjr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gvsqrfsox.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gpctagzsc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gbolkuyzl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gtpkvxxtr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gqppksubj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gfkjnfwnb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghtrgizyl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/ggizikyhq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gtybjthaz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gyemudczs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glcyxddrx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gpcgxhzsu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gwyfyowag.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwlywxqpp.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gmaenkgds.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gvqmfbgan.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/glkreszwc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/geyxzwlow.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gddibdlvt.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gztonkwoq.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gyywsdumc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gxmpnjmrg.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gsbjyyhev.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzvssemba.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/glsohkabw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gwxyuhaff.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gmwteyiyk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gsbjpgjym.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/guqbxtogt.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gliyussik.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gybrfsfbd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/ghbowvphq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gkrtxwxca.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gocvknois.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gvekjbibt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gbuazobzr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gjaxqtori.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gogrzshcc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gvxnqadjn.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gplsopzvg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gmbcxekve.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gnwtozppj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gckrkfokj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gkttkolve.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gfphdzrla.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gyxwqtihb.sHtML


<!-- 参考信息 -->