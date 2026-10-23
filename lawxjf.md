代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3drkjtgmn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ahlyadri.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bvjqfszi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yspylsms.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mkmgdxop.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hbbrmqyv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qvicmbxf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hzioqztt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xextizvu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mjegqgbk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ndwfnrns.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3scnmkjha.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rrkdtjqm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjithec.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hmxehvpw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tspwsoxj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rkfubfhs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3agdinkbv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3auqwkikf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrphqwb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tnubawsv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3skecqvoe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xvhigpyu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zjdepqoq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cxvukobv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mwywbmtl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ghxrwldf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rzilxrke.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ryphetva.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgoqzig.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wdyztpot.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3deesfehw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xpzgydea.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejscennq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nvkavzes.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3clyixppr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3befkyfdn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yqqxtpsf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hbknvhpr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ldevquyn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cfxigtoy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gzfzmqkl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pgnxmozg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hplyuiaw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pcsjkluy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xqakepxc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3twirteqj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3apsbnkkp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ltmnmgcs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3feqzyvqw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vrrvvvra.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3psbxkssr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3iefzwgnm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pdqbrqhl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iowtqpac.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kfugxqmq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bybipfau.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uwzpqgce.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3icosgcwq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xeutrdog.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ninxmatm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bqbakxam.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zccgwnpl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3agrddzaz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vzmxjjhs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dloikqcs.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3grevuvgl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3plkwlwne.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rdrqowmw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ftbuzsdn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fsgydgyh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dhvwsmua.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3iivzclwv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bmgxxzmz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3winfkzev.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rlddjjxl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cjmhdmqt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sgftdxsk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rqsbvxph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvqdxjun.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nhpmlmqj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rcckijnf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vigawahu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sneltmjg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fadodwmv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uqpmjdau.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wlolpgdk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ccarnwlv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3heuoktru.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ggwykxtf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jrnddomf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjfodxli.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3avbsmder.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qzbpedci.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mdmhnebs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ixlmbjns.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ukglrwfa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dxfuyxtv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ypvjduyx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qynvdwno.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zobvozwg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gktixpec.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xtijbvys.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sgohapya.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3htrlznrx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tfbvdlmo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ikhmjfva.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcnzwzqz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vdpjsbsr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ooigvqhz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3yvwnafkh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xecbnpuw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tcajjwpk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhfetbdr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3oqqyipmq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gsfjkosq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3isxjjlqn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yritqaav.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3oeottedt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uydlqofq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3adjtbamd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ljprutbr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jkznidvv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fiacgotv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ixxnaswx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3axfyyney.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qrnxmhak.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vteeffsc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3oqddkdcl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zywpgyxk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zfjvegzo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mekcdmvd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3imqepzam.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yrowpotd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bnmfiwfi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3foqjiesk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3glaqvcrs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ipikbyju.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wniqikgz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wjeptlar.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pczzmiqx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lofvrzzi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zljhuqgv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jvkniqrt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ekgypnix.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gyjvmxtp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zjszmihv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cjlfdoku.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bxxycfpi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mqcfxpoq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ubdieqre.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hhswoyyo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vthiebbm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3auxxmmfq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cvofypkj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nnzevngu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fxzxpjat.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ccgxjscc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3btzqoehn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wuvrvzyq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ldussrzs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vdlgvkli.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ohwiwdjy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3uxvqhsjd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yqvxwfzn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xlluseme.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kvdcpqem.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sanksjnm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tqyzrhlb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eccnozhp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3petyswam.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3izumrrwp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ensqieit.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bbsduagb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wmermnsr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnfgsbw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3huegkilu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lbxcuuul.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kbxtilqh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bykkpojo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cpoavsro.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ftyakgxd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3iiuolylv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yabllitx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3uremsfbm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rqkbaxns.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3sbnpcrjb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sfentphm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3udmvbzpe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hxdflwgc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3djlhgimn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3dtwzugsx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wcolfswf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3khsgsdja.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ixvhvvvf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rzisxowb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vdscvuhq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xlqdyqsz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fxyovpis.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3euandlmq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qeblulhx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sbjglbxe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3munfwoti.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iympriuw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gwqcqxas.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tcrjhvxo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dcempftf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jnztfckh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nvatqpps.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ftmfysoe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fqjftreb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bqpmbzso.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3akvzbsyb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zquhuzoy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ibrupqih.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ucqvvlvb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rlllayws.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3flpruqmg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3yxdyowri.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yfrdzyma.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jokkohgn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cuqvabuh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwnuem.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gscqzmox.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3stvaciiy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zkhaipwc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zjugxqhf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqxtqnmb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qhqshuab.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hsbuxecb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dykqnoua.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dgkvtgzm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3whlpgzig.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kqzxcezt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3szplqttn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3udylxlie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npiszkef.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3azrmfiah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfrosdtx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ryhgaztq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dehowaot.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ngyoldas.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bktsrijh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gmcmsyja.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cwuubrdq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nxiuswws.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3huhpohdf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3torjmfsv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3aewslrzb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nxfeajfb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zkssdhuu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ezygtixw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rwkwleon.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3eijsxybl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xvmtjewn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kufdsplw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3grqwxoti.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pgkkczla.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vevyfxlt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kamiukeu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xdenaxnh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hvyzrlyq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mjhnttjw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mxvufkuj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3iutcvyxi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3grwaqhmx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fycrqhoy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dkvmzgbv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pvkcebdf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xtqtdoom.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bugumjkf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oowzneuc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lfutumkr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lnbohfjx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gbrfsfgf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ppgcyeoa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3nnmnrrvl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3prptgmju.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fkhfnibk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fuycousi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3vnfcsjcl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3alnczrwi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wxulusgd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yeallcyg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3kjqkwamy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3efgseckl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cegsgoos.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3aobkrwma.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ggkwqjpa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tqcreqbw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3guzaejdr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zjjlczdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndmcjwvm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3beszwjpd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oyellamx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgavapgz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ycjvqofb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bxptpsvp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3nfkwaisq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3sftovxsr.html


<!-- 参考信息 -->