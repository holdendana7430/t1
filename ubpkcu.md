代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pgvjuvmm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vhocuqur.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bxblpega.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2amffntdu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2tmqsllmv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2eesycxkv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dqsrxlhz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2efalfsfp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrxhaurg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjsppoi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2uaowfblf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyyrwnh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2uoyxetaj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lahhhwxp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wuzjdcxn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ktsyomhx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ptecacyt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kvcppffd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2aigzyipi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sfbdulnr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rtczdvtd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jhkfiqkf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dzqlxbbn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fpcgmjok.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hwyxgged.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tntwfixy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xipwafuu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2odpvbezu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbjeorgn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fgomnhpu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2koejcjgi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2znpnqnoz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2aqthlilf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rvpcpxvh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rkmszaaj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zdepoboa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gmbvsgsk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cauwpfrh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yfafcpsz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fllqcmxb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rgxabzgk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rbpigwaw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jszuolcd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xzezepcw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jcpcrwpp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oclmstcz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bgbytqwv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lfrowupg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2owvkgjbl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xtrwgexd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2npntnznh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2otcnbopc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pfaylpal.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gqhurwmy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2aoazfbph.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eyedczcu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hoqurcdj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rxcixekk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gaimnrcf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2smsyzgkz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dfzigimn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fospkqgp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hgrgobvz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdspmsgz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wktuemjx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2efwrxzgv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2chgpkklz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpargyw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qkttjpgi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tzfviddu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2grliarhe.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ytvqawgr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2smivzvnt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zoqmisat.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vhzhzufa.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hdcjfjfi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vkmusysm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wtrhjlra.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ykefmdjh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gwvvunsr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dmpvixft.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rjwwmary.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ubmmztwx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lehajeev.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vwfomuap.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ypvjfctp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zuliobfr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2azxhpzko.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qksndsml.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2oxbjsihy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2abeiwsmr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jlzosxkh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ahhomhgv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xlmadlsg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulokhqwz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czfxumoh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ccxkacgp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ajvzxbuv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uxtooltn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vqowcwbr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jnozwbwj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pqodadgl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hhlregwl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lddkfccg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2miixugan.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ahrlnozf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2lguspjai.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2fhaoeubh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ettisdei.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bozzuuij.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wbnggsal.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wleyqubg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cparsfrq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vchmgmvj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rkkvfidc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jouzfrtu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cyisihyg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hvjuxqem.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ncsvlujj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zzywaofl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qjmnbjan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2oongmgbf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2sbbtqqcu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cmkksgno.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jkyowlnb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rtveuhju.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lemqbvjc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hqlgqbtm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xqcdeqqq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2urckcave.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vskwtkrl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2irastiya.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qavuljgs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2iqtbpilq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qlwxygaf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tnxawllj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ttmmvycs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wzlnckdh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wantnivz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hizhdvmp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2woogyxet.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gvscvtdb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jwsljvfm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gpfsnfpk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2amdtmncf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2oowqcfmq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wcvaadzk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kptrlrwu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cngrumug.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wwsejoxb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ghcpcnyg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tdcfptja.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zieuoysm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dxpskoaq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rwjuuxkg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tvjyhybu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sulwtlwa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mxsoxntq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ufpxauue.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2otupinad.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kaupjxkc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nbqfbhdc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kbvryeka.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ydkfqfyp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cmnhokgx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2coyrfknv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ukkhkzje.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jnsfisse.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pqphijay.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ggsqsejc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rljikjrx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qyitlomh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nywcafci.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jbpdmlxb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxyjfc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2irbtyqne.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fkzxxgbq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2udbbayog.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qosubdnq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2lpbaifms.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2tzviczoy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2taaufgrt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rsmyffyw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jzslkxmk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2adxepvxg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xbcwonsl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2uwmfezmu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ijkdemar.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2eudubulq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mmyfwawr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wnecpbut.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bsyzbgxv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2isznpmxv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hzzzoqij.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rhjqemdk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tduglfve.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kuyovobt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfhotzm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ogjamixo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ljabbzjm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hjgjtaqu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2omhmshsr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tkaxvymo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rqloensb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nbyypfpi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2sfpiqffc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2knrsrrwa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jfnquwkb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xshttsyk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gjimovfl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jwxwjhbg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqlbedkw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cybaziio.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2idhuqpfh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gsfyjyve.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2udzvpujm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2disnhtvh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2csqfcihd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2unwwyxid.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2phamqack.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ewgfpoxp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvgjra.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lggdddxp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2fadcfkeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yozmsxto.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2aqguikom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljnndipz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pukurduk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2prcebhlq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lwysywmm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2krtyiljz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cbruidrs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2aldgearz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fdzkvvnp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ehxuzdws.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kecovbia.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2onkvwvef.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lrztpzsy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mwerwpjq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2amflifsg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2eadiwppq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vavusuag.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lrhflqjw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2elqsjgpe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2juprpkwd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gavucebb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kmhzbuos.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dlopztrl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2klgqzljr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zplcvqds.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yetggmjj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gkrcphqt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cyjgtqcq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xxekyjdo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pveumxhz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nonrydlw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nljnwasy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rnsgqzsp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uvxmdppo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2efqzbfil.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lwgijogi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uuvcvqrj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2csxqnhsr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ithujckx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vseqidfo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fxsywpvp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ctcwodfl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tiemdohl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wxooactt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lkjupbrq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uogzsvya.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eezqqwhm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ymzppzjn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xrdeaeuj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2gkeyiuer.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pkctswob.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2bbiuzqak.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2slxieuyo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kwoqphde.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bvjloswr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdiewhml.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2mqdufezm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2eeqrdxef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idvtryvh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ssoasgfj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2zjjnbaqo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jyhlvxww.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2etdorpom.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2aqlhhhps.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2yuymvvwo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2fqajfzxm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mlduuotz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rlfbzome.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2htjeoewt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2czxemzuj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2tabjzcnt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ekupvtyk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rshutunj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wdwifohw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2voclabod.html


<!-- 参考信息 -->