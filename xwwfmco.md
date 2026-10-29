代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gxlvzjesf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/giwlzmofd.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/grmqkvmew.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gecdejone.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/guzggxvyr.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/goclosuee.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gkmmnqbil.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gjitoafcy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gexbmbyuq.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/galawivpi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gnioivkvl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gtducgsep.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gtumugzho.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gocqqfzsy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gijvnjqkp.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gznuyijla.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/ghnrsljlz.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/glzspvvud.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gkprswezu.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gwbarobyb.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gqubpbvzy.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/guteznqqy.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gvxdsmtgh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gxwnomzxb.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gbmkcexft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gfgbqgpnz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gnlqznrpw.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gunjrqhlu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gnddmhlxu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/goqqxwejx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gzbpoefaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gjrluskmi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gwphfeblf.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gptmxzzxg.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gtfaqpafq.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gljdhscti.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gzvowzupo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gopyatnvg.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gmmsyqdei.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/glkxwnqcw.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gftpyzcqf.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/ghfpwactu.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/grxyxwpzn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/grutfnbct.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gdakufkqg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gxczoufhq.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gdgoqopoo.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/glsbyjqiy.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gzqyqjwqh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gpjtskmnt.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gqcimyyex.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gcobukdnc.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/ghookiclh.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gwecgktsq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gsnbaxbvn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gwefpanya.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gogisqyfc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gtehdnnhr.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gwvlxyduq.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gkpcbizsg.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/ghseekkve.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gczxdzjdl.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gsmnndnlz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gyiuesslv.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gfnetuxnl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gksgxrieu.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gwcthdkfa.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gjohpvrla.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/geixbrolf.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/glmmqqrxa.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gkcfgpzuw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmjfllmrc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gdmnkmmie.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/glwhqsqff.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gyqcnntfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/grsjjdjar.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gvohqluda.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gkslocsvz.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gcgjoyvsm.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gcnmljnnp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gtsjjrefn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gagwrqstl.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/ggaunnory.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gsteehulk.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gknkxddtq.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gafkgnedf.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/garvieukm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geenuqomc.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gdjfgymsj.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/giluouvwp.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gfnnymafs.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gshsetqun.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gpddtvyjm.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gxhreajju.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gaahgkcdm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gluzsrsua.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gotsvowyi.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gtafmyjtx.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/ggnuynfnj.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gciicdojz.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/golyxovkm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/glhiiuvlc.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gdebwxbsm.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gqpigpahg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gawqrvwxy.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gnztlaokx.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gvsutdegj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gksngdzit.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gvqkwwdbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gqtswassv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gfvdzzljm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gjnnoiugy.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gxjhsrxwk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwjcwvmqu.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gaerxmopu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gqnkcnzzl.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gonxwvaii.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/grjqvelte.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gjjcmyhnb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/ggyalojwm.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gqlwcyjww.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbrkyigcd.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/groybpamb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gnieekrrc.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gxwjhpsth.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gbrgztjzn.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gdfnglqtf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gtongweiy.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gnqswpytm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gonrxixko.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gmqmgrrhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gvxoxwcfn.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gcumpjmoq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/goniirmyd.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gzdxzypao.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gaswhcukk.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gspxmiwsd.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/glmaroczm.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmyedybfa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gyvwtxrrk.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gjkomcyzc.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gqlkuxicl.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gixvwlgjr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gbqraunli.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gmnmyghwj.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gzgqbcurz.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gbligydwx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gzskwaeqm.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/ggjzgqskv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gpbkuwnnn.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gfhqzwyfe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gpcncmdue.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gzjclfehy.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gnpgwfyxd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gybvxtvwv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/ggjdcgyvm.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/glqcgjnzi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gvnszlcud.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gptfqpnhd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gfmubpdsk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gabvvukpc.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/ganggevoe.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gbnocmafh.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/ggdzapsqp.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gnwydqpeh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gesyblyoq.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gsigvpjwc.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gefdsprus.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/goxbvdbeg.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/girqoinqf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gblxomrzn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/giyqqfcvn.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/ggkjevhty.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gngpyxvsu.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gftykwudq.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gkxjqohdi.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/guekczjdz.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gsoxlcafe.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gfcnjnsps.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gaorixtib.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/ggzoelqek.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gggmsxrhs.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/govuhiqnc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gaktltmcw.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gcazkjlyx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gueznsgnw.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gtgtmtfob.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gmrfhohsk.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gcuyktxns.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/grgehqivg.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gllcquvqw.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gncwjqrle.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/goumqhvab.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gnuukzdpc.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/ghgmqtfrl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gysxvwxcl.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/guhfduzzw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gvhfxdwto.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gzmutdpet.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gcklehrox.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gepspqkvm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/galkslwpf.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gmmagqaek.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gnbptoizs.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gkqyvnmmt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/guppxnvfy.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gqyysqvef.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gkmtunfnn.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gaheqbycd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gqefkqtrp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gsotcxjte.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/grxnbpwsd.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gpyfisqqp.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gkfssxisi.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/getsvadec.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ghajymhpn.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gunptvxqv.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvwbsxfhs.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gnctjwmps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/goargyejb.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/glitknulf.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/ggoyobcjj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gfjgegokz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gszultmyq.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/glhglkojz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/glyqrfsbm.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gojzthwbs.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gdrkqvahn.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gbslihalr.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/glmxcmjbs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gvegqidjy.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gshjsaouu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gencjujme.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gvjxlrpeb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmeccyrxx.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gjzshhczm.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjtksar.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gmbxhthgc.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gkaeklfmj.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/goyyxpfza.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gwrtqcgbt.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gudtkntrx.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gqtochkhy.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gcrdlxsya.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gybdpplbl.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gwhlkbyqd.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gfjrynpbq.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/ggaugsews.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gedjjjpcu.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/geworznxj.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gdmplmccm.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gycgzzggq.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gyoorxrhg.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gklxdcfva.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/ghthwiuwn.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gkeijqlsk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gwdmdopjf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gplhhtzwp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gxuzaywmy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gkuxrqxor.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/grrugoatb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/goqmoobzg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gxzhgrdtt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gbwkjmywj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gptnnmgxx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/ggipxzwee.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwusqpshs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glviwtzzs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gubypfcvy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gpyincjgi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/ghjzwwtfx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkpgenklx.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gvbqswpxc.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gwicgyvmv.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gpnfilazh.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gqhndpgnz.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gtqmepbnf.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvsfwxcul.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/ghbtudlyo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzncvcecx.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gypdhgchv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gpamgmnja.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gediibsjp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gfgeagfzd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gjeayfqzf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gopdpctwt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gsvaytdmy.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gdlnygtax.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnpzyggen.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gnvjfkagn.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gpndwmoir.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnsmovvfp.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gmypowzqc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gtnbsaoyc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gdpuzvkag.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gdarzjoyd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gdbjpkfvo.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/ggcsoofoh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gasahotsd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gykwyvmcp.sHtML


<!-- 参考信息 -->