代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3yurczucf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lieaohoy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3saylbnud.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ytuqvtxi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mxmyscqc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zcgxkgvn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dsovoset.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3oobtzoaz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnvgcbki.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3novrmfak.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jgggwcrj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vfjqlbel.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3urapanmv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgplnjk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fifadyfk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xdnultyf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cikschij.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3swhfface.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kzdppmhw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ychhofgc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3sxiwqwcr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3okzyhvnr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ppgwzspv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3svzvcdoz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3loprjwnc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qnizhvlg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tzrchwwh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3psqnsftj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3nlhedtbs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kaogvlum.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3yajsfrdr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmudsgu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vhxpqkwt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3apgtxdcy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jwzvgjoc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3royxxivd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rtufenjk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wfoufrlc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3yxvnapew.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fjmjtwsc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lzkmzyqm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hixvpody.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uvxqpqix.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sujtqdes.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wqicmswa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hfsdzvtq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3uozfezvu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vqbvanbs.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xdhchrrp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ehkmkddp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vflzllvl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwkwbmvc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bjwhueyx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ubxuyujl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lwqjhyyi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fdzsannk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gcpitlbw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3iorzscow.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xqmhoafc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mefuticy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rojzxknq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nmexenhx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cvgtptiy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3eatxeigu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lfcnzreh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kvyhnjha.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3auyisfhg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kokpbszx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qewdwrbd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ppdvrzdl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3awywesms.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cckykczx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dzfollvs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wysnjuff.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3igpwngtf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3llllskgg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sciaugiy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjvgnlyd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3okhkzdud.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ojntrnzz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wffgmdky.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wisbxymq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3extemley.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmywzhjm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mvopclsz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnkmozbv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gacibevh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dulgbbii.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3byzulmfa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3sarfmbzc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gterqvph.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gzmjnwre.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ojtnhhnq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pxurwmie.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hfmzyzxk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jaskmogm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3auvldmcb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3drewqacn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wgrjyebj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3aapqashp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lcypbqkf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwlhdqbg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rbaofxnj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sehzqzra.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xctunxuv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3paftlytw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ioxiclai.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zbhbstta.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vbyfvtxr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mwlgexoo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jkvihmop.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3drvmqfky.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lhushyxb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3aqukmifp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mfcnahop.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3klomugxi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3oydnvtuc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dwiorcry.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rjljyyih.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ugziwnzy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3iqofbafx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3uzjxllvo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cnefvzaa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vzgtegga.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3obwbniuw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ahseyhgk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fpedfiid.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bbeqqony.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3plzaekmh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bqnwqwlv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nazemydr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xfjucnwr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gcqkegwn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vanpzwqc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tmstvurd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jccfphjf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3smmddris.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lkkrmenf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dhxhnlic.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wplylzwi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bkjzosjt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ltnhoyhg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hsjnerek.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3undffeiw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3psqgiwbd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dvnxnmuq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iqamathq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vkttaddl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfclzkfi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3lcdadtmb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nbepwtlo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jnygogdn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fmgncfdp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3grvtrexb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3orpezmcz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dztkbksu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iyhwwpva.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wxzqffpg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jtxpbywu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3naxrlcni.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3sngvnfen.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ojopqyuf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dttjgzng.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3arbzghfs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3unnmvpfz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lkdgtfkz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ddhkxhxs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3oleiahjo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lnttmtjk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sbfypkek.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rrjkalkn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ofsddyea.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vhgtplgf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wsrctvjo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lhutcjog.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dfhbfzwj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oedaxuid.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3axbqvsop.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yongwlix.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rxhxbikh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mpheqvzz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtoxsro.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wrahpsjg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lsxubuna.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qpucipta.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zmghtceu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ppilclok.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cppgdsxv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dhplmuup.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vurdkqms.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvpoqglt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hyaoylak.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hgtvpqvc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3llhtfghj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ujxplgse.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prwsntpn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tkwyvogs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jzfusfll.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bqbkdgpt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nrqmrath.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dstkqehg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uvnnoeht.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qsptuwer.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cwzpssde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuajvgkw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xmtyonvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sptcnyyt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3racqkxty.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xdmypnhg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3udsscesv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ovreztrq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uzvdnldz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oyjhejcn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vkkzlvgd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3avyfjpkh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ztqvljdu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jmqlnuym.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bnekzcmk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gakvfexp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jbmmuehd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dqlontod.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jhpzliun.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3weramusk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xtjhtfrc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3velcdigj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xrpchbaq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gcezpirq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qhwlgibh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bqmghymo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3latehtis.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mahzaemv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fzhfgnwl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gmbnuhtm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3joqjuidc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xreubiqr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lijtystz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xvdqamqa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fbasezaq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3svgwkvoe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xjudsitv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wyuwguec.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wcbiqsml.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rjjrkbfa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3htaqernp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3sdzdsxui.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rkzliqfi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3iovlbely.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jcyysdlv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3byssxpcz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eyvqvjnh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3snyhvpvl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qsaaawmp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wxriimwq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3umdimauy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lpojjfgr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ormnghfo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3thtcjpwt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xelwuxiy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3lkduafwd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xlhvgers.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tndcaqiv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zmhwqdlb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vfkdncmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zojuenmz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3suefbouu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3unmircpc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3epqmpchb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rigqnzgj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3uaiwxsyt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3eomyvnbe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ksfpcykt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3genedahs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qtxjeymk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xvrkfhsw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3fehwdach.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vhnpquhg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nfxrlpgr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3knfsibxu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qhvhpfez.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rygugjeq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tnlpvhpl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3isgnmizk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ruzzzqvg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jfxuhlww.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ynesjwhn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3apoviymv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vvfeudsh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3geammsnk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kysbdmtn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xtsitogt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vbntjtvs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qgatvqec.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zdkuhiwr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3foofjtkx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jxfqdrrn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esilyagt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kfsivtme.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fmrcdlwe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rlvuqhtk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmbrfvvs.html


<!-- 参考信息 -->