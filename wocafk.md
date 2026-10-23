代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3afpevdsv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3blqygkqv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3iipnxxei.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3tfdulgmo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cpgjljkp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ycqciafo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uqkjhtga.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rszajacz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pumlebuk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ixdrvyww.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hsnrtqbf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3okthktoh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqfnxjky.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iylpktxn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rhrqpmgi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ylscihdc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mzvaietq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nfphcvxj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zsslpcfk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3geihagzk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zsaumpum.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3oitsoijb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ecxdkmft.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xbsvgmqa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qtytqkmj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3onpcmzoe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gmozjaee.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vzprcfgo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iqybfucp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3duwyajmt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jwrppket.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mgclpqfh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lmxksolr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jxhxebfx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3etqfibcx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3linrvpap.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3izvlioem.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wggfswjq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3raiblwpb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dmhncshb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lqhopypt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mrzymksx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3skcbssbl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vozqfral.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tvrnooby.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qiziajry.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mjmfbhrz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zbswfssr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tiijlvpm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uxogjsmk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ixbahebq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3pbcvojdr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lqonoimj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3whoynmml.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ffbbxmgx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mmyzqtzr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pwhbqpgh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fafdepvz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bzaymzgn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3gugenwmo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ecbbfmcw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3inzujspl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cihlonkh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mzfblawa.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vczcznyb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ujvubgqm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wxkwaiae.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qorbuazm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cssyuqai.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vnlfztry.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3knmxxlku.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gjxcoxwx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zxekruoy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qlnbumkr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hsyfznfw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3nizycqey.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tqljfiwo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ifrsfnxi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fxakmfyp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3taaeaoeq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ihimzpia.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kayyaauo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kdnepsdq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qutqdkfe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tfyvplnm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3oweifbnn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xblywmeg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sujkbklu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kvflxnsb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wqnvebpz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhivxivr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nkveqapc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qaczzvab.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bdymnssx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3slrabcus.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3puvsxrvm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3datmvivr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tikoonxl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nshiztja.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohllirci.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xvlwoycp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tybipgva.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3mqquakth.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgudjlbu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kzekaviq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xrcgwovc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ydydkzia.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3omhnjtgq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ocamdnat.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hbzxpofv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gkrfjfqo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vpcvucja.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zeizsyxq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nrzhsgua.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwnlrqdw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nwxzekbq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3djurahyn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fojknlot.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nzktnwum.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fvgdkxlk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xqysajov.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nmwqgvph.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ytaociyh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3odvchtne.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kkznkntt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pxysloyv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mmwvhsnh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ttzwyrjn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3odmshxaf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3grlccvbb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ovpmnivw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3utwckccx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gtzqzhqo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lohfozkk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tgipmsbo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wyepmxae.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pfdtqibq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jzejjimn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mezhmisv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ffqqxoml.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3knksphkm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rktgcaag.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3laqgmrua.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uybspzdp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qyfgbajk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cowxlaqe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ikrdqeos.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yprahufv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mqfurphk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lpwkrkhq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tqiwvaeg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkmsovr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sljbdhpr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3eblhkluv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3lkeeyqyo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qgdcvpwk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jecxgjmz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3kupzvdcn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3dxvciqaf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wexladjc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3idhwrzky.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ztmoblwp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3njcakrct.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xbsdyuxy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bsjqlxvc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tfnkkjah.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zedjjlmq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kxzjxipl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lordsuca.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xngajxxh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rufopktj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eokozmla.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pcynrabm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nxravegx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pchverkg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tgrbfwax.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lgqzeokv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3igtoqqlp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ajnqwrfw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tfkmzpoq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3giwqgmsf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pwlwscej.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ykgkkstt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bvqrvroz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ybfqgcyv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ftlnbnsm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3biczvxli.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ggulvzne.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3betmczbs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jaqycoev.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rkgbcrkf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vlwfnosu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mprnuuzh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ttfvzzdd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3aruretrr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gkextlhi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fnbqrtvn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3skqqlpin.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3axhkvyzc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ctoedrqt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eyxhzrna.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3oeuvnasp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ulgkxtgb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wcpskqwt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gpceotrw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3stfohptd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ctxrdehq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hrdljift.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3sshmyovd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cztoepod.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3oxchrwry.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3whljqtid.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vmlpuutd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfviadvp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3uwquxjjh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pvbettcz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xalfciag.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hrlydzlt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jqqgvqqb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apoebaus.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fpjecfaj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3nnnamxde.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3quzjnaif.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vlnniqjl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3krbduder.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gidzndcp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3eccdhpyr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3eiqhqvju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zczzijop.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kulcztcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xejrvucu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qytrwbum.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ivipgkbn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3kogdrtcd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xucpxcju.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ceadfznp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pdskqvwe.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cysvcqgi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ngkuobyw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xbockfaf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cvdutlkc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jzgsdfyx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gahlyrda.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xykfeqap.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cvutarkj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mzxdonsp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zvauvmem.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pootnvxy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tpdavfty.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kbmmszvy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ltuitqgr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nrbcklrr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gjwbckic.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yhhenpap.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dlqofahv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gsskqqpq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kzcpesyr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rexyllwt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gnjurqar.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yfemckxa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tozadhyj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qpkhkjpf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aoayfope.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vdskrwcq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ghfzkvxa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dayammpt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3mdthdbom.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yfmqgkxj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wgnjlxuv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3afmxxyfj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dnbsqxpy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yonzsvff.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xjqqgxrc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bpxetkwo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dfzwjuvz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3arwzytyg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dkkiqvtv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dfacvajf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lljbexys.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3cpmnqvpm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3elonuyqz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vvgtsljc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jqjxiajk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ndbcpslv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upkubsay.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wtoagmzz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3sxvgjyyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scceeaai.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3diboilfz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mmzesetk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3lawkuaxh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rbvtmbai.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3oicxlkcq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rgvxsezc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3uqjfldve.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qfdvyrfz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ocpbabhx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3iqbgrdml.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3esnjcczq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ulqkaxbv.html


<!-- 参考信息 -->