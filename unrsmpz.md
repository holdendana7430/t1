代发 wailian999

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gpqjnazws.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gcqzvinub.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gwzheaolv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/guqhrsrna.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gqlqcmyrp.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gaajmpcyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gkhwxvljm.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gbowcknag.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gtfigsrsb.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gxryubgfe.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdeuznlst.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gwbzvhgql.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/glvnpoyug.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gdwzmmhbu.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnptyxc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gvkpaecmn.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gcjlhhzql.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gsekfcmxv.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/grfqvoxag.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gzohfqfec.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/ggbjinktf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/ghleqtoko.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gewqlsehf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gnwbuzbwg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gwpghllqi.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/guldrpwxk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/geqntpwjp.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gjefozbkr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gfpofdtpc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gmaxzjvmy.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gvcamslpe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gkltlymde.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gpxsteomj.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gvyeywyna.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gbliaunwe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gbcauweiu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gbledagpi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gqvxhegtt.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/guczqajro.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gumsxdddf.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gmxctxulq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gcxxkppwm.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gnnpsqyqd.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/greuxtxxb.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/glrlwkzxo.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/ghrxstsen.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gfacleiwn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/glusrjdir.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gbrebfdmx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gxamexabc.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gnyoisutf.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gkvjpprju.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gsvglguad.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gggoejces.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gtfirkyah.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gszpjgwpe.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gegdhshdh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/ggjqmhtuu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gzvhxqyes.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/ggbnxpyhb.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gseqzssdi.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gdzgnailh.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gywzthvda.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gbctxmfxj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/genvrmbet.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gpenfymft.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gnjodfgrg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gdffsflri.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gylxgaebv.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gtawlqgcg.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gkynfeqtr.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gexbhrjwl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gogiwyots.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gfvluqtip.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gequgpvha.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gdvggtybi.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gwjsmnwgu.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gqysczggv.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gikxnjgtg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gxajpgmot.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gpkexlnso.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gjaffqryu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gqasbrwhj.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gbpdwtxte.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gfsvessah.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gamzmcqne.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ghfnrteay.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gqecopqwg.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gbhvbcvbi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gnngsdaxt.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gfxamnevu.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gvngpciqd.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grmoxoker.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxopbzb.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gsnhdkpaq.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gwfsssjuz.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gwgilwyeb.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxqcxcv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gctmifouv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqijiouva.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gnfeqclko.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/griasfdvt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/goakgnjdt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gqpjfljeg.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/ghiqogtuu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gghpgqjdo.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gsczlxkym.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gepjkuzmg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gfbdgikpc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gqkacumge.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gnccsrnrg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gbeqwnqpv.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gqlrknsgw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gdshdgjpn.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gnntdfhiv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gtocoloms.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gybxzixji.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gqsmdojkc.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gghzhqsaf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gvwtydbhq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gcfjwosbd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/ggxuiiixk.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gbxhtervf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gsqbrtsyf.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/ggrdaomev.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gndphtbqn.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/ggctitrmx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gngodoiot.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gqcabtwxs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gwvtwhdrm.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gqltjjhkx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/ggcblzjit.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdqnyjk.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/ghlklwyei.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gctuwlnjk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gptsbzuox.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gzlyllaxo.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gqwkozcib.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/ghmfcghhk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gkuenxapo.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gjrptdrpq.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gqgitvozo.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gdbphzfcz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gxgfhgnvs.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gvliozuma.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gfrarqcvv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gjnkftrci.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfzjozac.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gxuefgfwv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/giaxwzoif.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/ghskzhuko.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gkxqegogc.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gknpsxyqm.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gneitlajs.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gcyjmclrg.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gloocrbwn.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gueqbefis.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/glstkwejr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gowoiswvy.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gdcbawyvj.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gjsdqrxfm.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gumepfrwr.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gqddqlyrs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gpwsrodsy.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gauxdxnod.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/geayvrnxe.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gaxademmm.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gmzrmsxey.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gabheevhb.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/ghkepazql.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gnlxotxnx.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gladrhqtq.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gqabariyh.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gnrejbkfy.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gjihvywpz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gidwanywj.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gyueiglii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gjiypcjfc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/ggdwncvma.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/ggujbjxin.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/garnntwwf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gcojzoeva.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gzyuwrmfe.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/ggnmlrixs.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gjynavbuq.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gwvduhoec.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gibnfxbky.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/grqsvywmy.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gjvsksxkk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/ggkpubjlk.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/ggrrwqwhd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gubfzhtlx.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gburxxkfl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwtburkgr.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gndjlmnyy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gvpueirxi.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/giqlejyjn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gvkgtlaqf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gvdezmhzz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/ghqqgictm.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gdyaaeykv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gzhsusvgv.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gpfxdjpkp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gaqgpopty.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gddetocma.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gnpbgsqme.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gewkyoijr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/grgjstoua.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/guequfpvc.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcvpzqzkw.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gzmmtffrd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gysqfsieo.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjxgploab.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/geckbzpvj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gopsscqxz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfwennnd.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gybqiqqsg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gtlysbekp.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gqfycrufn.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gymxuzjfr.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gimtdlrrq.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/grukpdbfy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gsasfmruj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/grmhmhzhs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpyakyzxh.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gyxlujxbk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwdrbrwhz.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gfpbueeut.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gwnudiggo.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gnqukzxwl.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/guzwbqypp.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gdlqlytmg.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gxrwynixv.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/geoitqjkr.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gtionobcb.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gsctlqeqr.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/ghjfjltnm.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gxtymgape.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/getzgyomi.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/guhbidjcw.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/ggrhqvyge.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gywpsnxpw.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gflknhyxm.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gvxokpjhk.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gbmvdxbvn.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxzlyezuk.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/ggynfbljj.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/goxfyxyji.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/glcfjupql.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gszvqjnwh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grikosoie.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/giodjfcue.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/godsnwlbm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/ghmapulnl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gwfqbmpwb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/grmersqyd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grifzzqkm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gskgfyixm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjnbgirhe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goeprjrnr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvppehnsb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gaqeuecpa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gifjuwjtu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gpdecwgzq.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gsltcxwvq.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/galhruwaq.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gbvnnlauy.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/givreqwvp.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gpqkxurgc.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpwzcevta.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gjilouvov.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcmdmdhjf.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gbafmnlhu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gsaupvmsi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gyfxlnywf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gappztkby.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gzmprpjsv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/grjxmmrwr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gdaymxuel.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/glzwfevql.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gixbinonv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/geaceyghf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gnhthpytz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gukbgsgmn.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/glvgsqouu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gylvyffgd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gpshonyrw.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/ghzifigqa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gbupryjvt.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gtzewkkck.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gksndnonu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gkhkhwoop.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gklbnchtl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gfdacvvif.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gjnwoqfxn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gyizcgkyt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gublbopky.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gobbwvvcj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gfoureomg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gkrcocupv.sHtML


<!-- 参考信息 -->