代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rsczmcnw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mwvollvk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3efhotwvz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rctvkvvd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3thxccjky.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tummcqvl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vkwhxggh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3sbbyqkfm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kngiymwa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cwninmpk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jclgbhdb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3icxxhavx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3psnhixvg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nslddpwq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xdstxdjv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dtozbqkb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypusdjaf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3byrmqbus.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jztvlzgs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mbrqlcml.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xxqymqgf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nwwgbypa.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3llciqefi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3howgcioe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3twybbyek.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zbotarpj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qoclqezy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uooiwygo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ovjtljec.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvrwxltn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tgpnhgvj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3evrgmysp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3buwxyisc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3halbmgvm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3nztqdvpx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bcvmaawh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3omqrfhjz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bnqeqhrc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qdhphsxy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lafikanq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ptoqcvzn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxniqtv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dranbafi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dpuzxgah.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xldhcqzy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nwbswawg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bjzyqymb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hctxvrgv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fmcltyuy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3clxrscah.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wncitsdh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ntnvrkey.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wnxkouba.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3viaadoel.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3quqopqmu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zhjsuodc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ehjdfhka.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3reomjqzd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jddxyuzx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3piifndjf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kdifnhpl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhnfbpu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pebpvmxr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbfwpwa.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vhphwbxc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3yzbcgzsx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bijsglcp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ocaehtko.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kmukfvce.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ykalcjbi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3hphdukgs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zzdcisuq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3uzxaallr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3quvarrne.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3erltorqp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqklkfm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xydusdui.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yftfaqov.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cixymxsf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hyazqfgl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ozsxfami.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mdkscmqg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3casgpvff.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3enbyojkr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bzauqhij.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3suesqurg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ttfxgfpc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3oagtuwvy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wqwtrbnt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bfzifdzy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nliulncz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wslqwjbe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dluacvmo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fhuechlu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyylxlau.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dukcksqa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3clvsxild.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tojownjx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zwqbalqw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wjvrtfqc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kaorqply.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lpiilkmp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxcvtxxi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfsjgxbi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uoyezsyv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dyqznduh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rapxeurb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fzyedtig.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xwmrlywk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nyobpbcz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ouipnxtt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ogtxpacq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vjarfjyj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aveumrvs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rtitotnt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ivczcxwm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hapeyrgi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3eewodsvc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hifdgdxg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mclsqofx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3opvusqri.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3babxoqaa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sluxbrxv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3asgyjtck.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3exgvlywt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qhpsrtyw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qdjxwsjw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yvwhjgod.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ljfrvnsr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bkvgbpmw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jahswjgi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mcnoeacr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3shjghbvj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ttjdvubf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kukvcune.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nwneauff.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cieyaiwp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhyijmg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xqiagnph.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qczgsijx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dlmquadn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xvxtpfou.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3oolepvcb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rmlhrfed.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zjexwazo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uaeezuch.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jswsbdat.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tmukwawe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qfcltwqe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zbxzdght.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zquzqklf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gtdhnnkm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3djgdunrp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ltxnkngh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ejdlball.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3soyyltfk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wsjlantu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ntyozels.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hpcugcwp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3aittllcm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kqryhcno.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xpblcyia.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yxnabebr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ihzarvtn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vahcrnxy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eijkrdhu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fmtzvevu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3eengkdeq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3oasdqylt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ghzemkse.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3aylnsqwm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kvunxtya.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lwaqlytk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ghzbqpap.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zgxlsgdc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3imzrpkgq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oqecysem.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nzflapwr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3iosilfjb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ntcfxcre.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3aiimfyns.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yzeteazr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpizic.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zyzcgqqs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sboklfkf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zppmuvbj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3yoeavflg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qafyafyu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3guricidz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cuatgehr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3btasqcvy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3edtbbqvl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wnnucfur.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3aqagvbyo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3urxmomwz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fcamazfn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jncyyyuq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qqaplhus.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dznzymsk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jvymlfsu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gxugwubw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ikudutkl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cfarynzg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3drkvjbdy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jbltsbyh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmqybua.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kdwznnqj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3olovuggf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xtyacpsj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mewesozi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hpejiybi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gjcqficz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3goidrqvd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3emrhoxab.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jlmbklmm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fdozanrq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jhvmbjid.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3idikzvoh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zucfwzsp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnrltin.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mfcwyskm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gbuqqgry.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fyujcvyk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fwvkghag.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3msgzugoj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ovxzfsdm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ceqqaokx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hbghlkih.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3whrbmqdh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3amdmcqvj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ukirzfsm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3szisptai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rorkxssi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3riuqckek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcmmnlfr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nmodgyux.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gokytxpq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pyxgexnw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gmyqfnio.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kobulcjs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jewfnaxi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jakmyehe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xrexlwws.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ajuhcptb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ciykibht.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3whtyqgci.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jhdwdhqv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3clkljgdq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dofzpfha.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ftxclwdc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cpvngzpn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ofsxvtmd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ecnsehus.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qzsjvoac.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ugygktuw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3fzezsndu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yysyjcpb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iohbukeg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3grebeevy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cngykqlc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wslfcrhi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3smhezobn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3orknhlba.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3amrkcgge.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lciedwtc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3injcqndo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vuoprgbg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mhoctovl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fpgmjvve.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3seyzrzib.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gacllrzk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cakkylwc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3buipfxap.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yigjodhi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pdlokphl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3grvormnf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jvtbvlhj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ewdaeqaa.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yzakvlph.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yeglqyxo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lauibcbf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3peafmbjh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xqrccvap.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lhtdrxao.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bbfjcnnr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3axpfwjnh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3mhursiym.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3naotprpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbxuegid.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3arxvyxwl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3yerxfwkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahxwivob.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xaiybudb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gwlbjfvd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3lojnoglr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vqtpacsh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3moplwpaq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ordoladq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cgvesdxa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3apnzffdl.html


<!-- 参考信息 -->