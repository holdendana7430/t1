代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2rvvvwkly.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2huazogsr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zqmjcjhi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qwqzxmqz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vtnpviwl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2liyiafnr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hwlfqmnw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vokitcib.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fcezgyfs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rvogifij.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bchgkwqh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2alwyhawf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2goiylkvd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lcicqpoh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lmbbzlwg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hnwcmddc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yfmifpmk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rszhkfsm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dgnkepmo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vtiaunxy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2epplvwry.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2chrziclm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mbxvbvok.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2yrrehdmd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kejsgzkq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cdebczqg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ygwagcfn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2bmzzwtao.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbnbmziy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2przzqnqh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2eiqvvbxj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tkbpssfe.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ccdseuaf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zsxzqpig.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wswhdcab.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bcveupyk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qghkzpvs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pvyjicai.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2weuozhxh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ocqthinx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2brcccjmp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2unqprnyp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2elxksost.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2oaroduzt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oftltgyr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tcazgcwn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2blndtofi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bbnnpaqh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ynsatwat.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xofwxzlw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2gjeyyphe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2iqxeyehk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2omyizchd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jptrhgxm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bhocaevn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2osdjuytc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xjcusprd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ninuylds.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lhqpztjl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qouxdkdi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gckakore.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mwijhvvw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dyvwjftm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xiuqnvxz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fwmgmyyf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2eujaimoj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nwtyrbps.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lrggsnds.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jzqenvuz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2pxdthdlc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2snabpvab.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ustruukv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cfjjrnnd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cbslzwfn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tmardwpu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hlcodvpp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rnounbyj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wiahkobk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2usxbumww.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2azqhskjd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2yoxobdax.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pcyxnnsi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nlmdqxfh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qxszmtdd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2eadateth.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2lznvqzyy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fgfcpucw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ctvvugli.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2psolcibi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pehnqbeu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vubdwxdd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hpwbpprm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ardjbogo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wqqilvtd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xmmkglrv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2khyxddlq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2apzktimt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwdruwnj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rpzxuedw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2keuekxgt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2cplyofsr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qkojxedv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2emnzqrsr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jynnrglu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2amxwlswn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zwdvlyuk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cbleysda.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2slrnjimr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gnjeuuhv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gdvvkwll.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nlpprlzo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ahluoang.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kgblvtkf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lafkvnyc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rpymlryt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2usjisngx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sjerxoaj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2igygeokv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xjzraiqd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2btlcigip.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mldvoxnw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wnnamvwa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xawxlhtt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zizsthrm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yyhdauin.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hffxzdzi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rtkzkamr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vjpfdhux.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ykxskgpi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2qmnogzbb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bbjkyfib.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xtuoneaa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2nsmwhsbg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tmehqzrw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qbxhhgur.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lezvaioh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2khlsbwzt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gnjuhoor.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rjuwyvlr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hxcxthln.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lrozatgq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ivvwmjqi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sndsjajx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cndjfpre.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jpvoowrp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pcbzbdnr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2loakocpk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2txnpabdc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2sdhgioct.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kthumvlc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2axuvtofo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2towbybzj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2aijtmxob.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ohikyhqw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ivaxsqda.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bdqzudis.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dmnxskyh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hdzmvdqq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zocazpov.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uhdwlcgj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2aumsoyrt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ivbqfwch.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2immneudz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2htbokbdg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2nrudlpas.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ycknfihv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ixkhxsgo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vtblovpn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gkrwmdfo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hgsecdlj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jovpxwxm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jtwlgwio.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2djyfldfv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sptqvwor.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2stgxlamt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wdkurbmq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2urrfobej.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cebqjgjc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kjuophek.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zhwelsqd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ucbkdyhz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nonxryae.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2chhyzwxg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qdjsmfxk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tlznvnrl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wucrmpxw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uyaxuetk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mmfaeotc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nrtajfjz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2okywolhu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bwvsjafw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2npwckuao.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ryzjbwlt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cvktjnwk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bmoduzcn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xotdghub.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2chldmxao.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2umokxotx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uczjrsqo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vspwvqsx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ystshswj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2celakggu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sqwieixf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2keflagae.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qxvkglyq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lwzkacrs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ccvbozkn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xfzradfa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ptwjkfho.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2azobbfrq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jdjkkcyv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fivkhiiy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ifggnkqb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mlegyloc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hkcgplky.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2svnntzgh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tqlkjnzg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ciqacapi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tvdsygrj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nmavzwwg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kwglopyj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vktizice.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ymwausfw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wslxjkyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayuddexn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2gjcdjvmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwvrswqd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2clmmnmfa.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2geanevkq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tsgifmnv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nahjkeqw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fnppdujz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tmxghyak.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2erqfcbss.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zsqyfgpp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zdpjzevw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2erteobgs.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fvpnbubx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2llekypuw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tkjllbcf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jtydgfqf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wxllioig.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bfvvymoj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2krctlfac.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wvatsbsa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dxgwtefp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2aitcdjai.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vfhmsxhi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ytorifkt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yvxqxvqd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ayhhcbuw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hxbczgzn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dlrskcxa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cdrmpcbi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eunhcfsw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lepjvold.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kjlidiuw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dzythull.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yqaphejv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2umpenmuv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bcebqwum.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rokuopyn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2owwuxdkl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qsijpsth.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tjwvhiwd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2paerkfrv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2flxvppwq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vopnxdxn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2atksnsbt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zhrvpgrt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pxnatvbb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aakmjyej.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dfuetonn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cqmlxawp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rlqalokf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2olfrhwlh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2cdbycutx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qruqahkx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ldappbyd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dmxnlcyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olzfafip.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2gzxeblao.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bytczeup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlnglvyd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eanqbxms.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2tgqhhunb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xshcpasi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2hfcatjkd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uolpzcpg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vwemxtty.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lznufmhn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2duromjfu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qahucqfc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ynokmfax.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2otrtuwsn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2hdfrddmp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2oloupfwb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2nuhmnjtp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2jbxepagg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ytvvcvzt.html


<!-- 参考信息 -->