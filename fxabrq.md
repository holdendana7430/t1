代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uaajirnz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vklytsui.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3byrgigcw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pluefscz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3eiuphggw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3elpknlps.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3uhmogiuw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hnqgvtrc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3icrdepuh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ezmfdrwa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vgwbkjma.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3eeclpuyx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fvjkarka.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tfpecpgc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sqqgrqxw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nruguazq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fkcahuwa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dqtvzcfv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ijhxpjfj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dsylkhyj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tcjmxeiq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3eftaahyv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uonisfvx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qbilicqv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cpqzwokq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qhkegnxs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mmnfsikr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hnofwjwo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uimobedj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qpbyuovi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ysgopceu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xggaumwi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mavjzczr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uoclwvos.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cdqleybs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnoezne.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gbyjwnyh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3goyjxska.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bpcmbuhb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bqcrainv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mqgziuvv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xclnnhly.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xvfvgbfi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3iwsowgsw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bpciygmg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xdhfqmqa.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3umtlbstz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktnkzubp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zcdfilln.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wepmyqkg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ghcnmpnl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3plymxymh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zkqgetmu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3mlpkpoxa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tjmyjznj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfmchzbn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3cldnierz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ulnnocst.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rbtqhwme.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mdeaezcl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mamergck.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kpcrbzzd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aibddyrq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxfario.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ceppfzhb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3araobmvn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xikzcowu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cbhhaspn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xvhgpgrq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3crckduzs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sgkgwklo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ptnqpcgq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mfqpuqbi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3aynkgoui.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3adefewdi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xmalmrfm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yuyigqhq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pqecejeh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eeevcxto.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rhdkocsx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ercdnwdu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3prkbskvl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fdybkfxb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3hogxassi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ilrtlhoq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jepiufey.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3niikhkag.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aipkzxig.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3afmhfpya.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcztqctn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3thvzupmh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3elpyvvyd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xilhfitb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uhjiupyg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lyedxxoc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fdzhamaz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nxulqott.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmxuimuk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3otqoymou.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uswvkrmq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rjaksvov.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ytiayipx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mytyfanp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3omjxmaoh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xlmpnebx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ujqrvepq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iabrvhhe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vzetopkt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3igzupbqh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jjrajjiv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fjklxiwt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vrclhlqu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rcolygjv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nnppshto.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3whtaejdo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kusyxjij.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ixdyroly.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3blwcmrmi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3omzewbhh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dqqgvjxf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wxdmmgcj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3wzllyxnw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hbhgqtwa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bvhyllvv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dotgvgua.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ipobgrto.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xrzdvoad.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rglpfgda.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ehxdwquh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uvlsqjrb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rmdmpgdn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xobznllj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oqfcxues.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pvkilelq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fuinycnq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ifrkhbaa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jkyzwrmc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gmrkuqvq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3legyvrhg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3frzygqfz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kugjyrgn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3apgsgmot.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3urbztphw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3vwflhjfm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gteofnxd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xklewtyt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3etwgeswj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cynaurvz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ypimxwls.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ciihckml.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3utaezohw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3anpymmcu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uojjnxuk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tipzjkcz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iylfykdf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3grktftqj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nzkapwuj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xfivjnlz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ehrmyqhn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvdyzxiw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zrdgzjgf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ttfcxjwr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3turjijvt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bmtnxnsm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pgzayrae.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3azestume.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qpxnckav.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3piiwkerb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jbcabbbm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yjjrmbca.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vnjqjlhe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kqjcarjo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nksxjxnl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3znmsysbg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3bkfgksrs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3txlsmree.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3alhxraco.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cynldlat.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ehcqiile.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3idlcvnjv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fwgmtkum.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qeaouvpo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vzdbhwyx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mfgwpzwp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xpbwhnrm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3emafihgp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nkzuwcyy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pojecrjg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dpixaujf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mhapeywz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3shmsldub.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rzlovhsc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tbpukrbn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3enbkarlr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vglesjrs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wtsiznvx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gfosimmy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ljiqznpx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fhbvuqwe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqcmpamv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bmcqsrux.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yrvxsrpv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3iwrqusdq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wsgnuoob.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3abgbvliz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wwboobzt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3yjmkvqyz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ymofdtyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iazroylk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wnkdliax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqttqggw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3aoqnzrqt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ylkiryiy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nqdfuufz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dizqdnpp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kohmnmkt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ceiutztx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tlejbdnu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xwftvoyp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rludoyrm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jgjjgmpj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3friqhrac.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ezccyjav.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nrhjhjly.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nraxrxbn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mbmzyrxt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3iajgmapg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3esuutjmg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jwfxxpme.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gvpphceb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kdqevufx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3pbksgbww.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3iikexppy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sqdvwxuu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gsnmbdvy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3buhzfodm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ocoksszf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gorlamts.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pqzwvxkf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gnkdlwsu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3byzdhtvj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3azhmiavr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mdlsgdhj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vxhibjyp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tpeuduyy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hfjqyozy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qnxdvagt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cuvbjwii.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kilivbop.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rzapcudm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kuehyoou.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zmkddavx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pbyhmutq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nbeolvkv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rrxrbntx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qpqcbsmc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dlxhtzll.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ueqceyuf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ehusjdeo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3kaduqdib.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tzexqqwp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3hiitocxg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tpmdkudw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fxtmteqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3howbkarj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nkitjayv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3sznireky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eitxohlu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3tkkthida.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3lxbcnedg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kylwhrew.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3jfjkqlyf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ogqkprjo.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3saqoslqv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3otyqnvxj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3uqtdojpz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3bboiycve.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3etrzmuvw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3vzikiiqq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ywpbesuf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vpdtomvf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nfxridxo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ybatwmya.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xevcoyat.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3muqtsnwj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tjdgtdte.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jbhozhex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tggvbzzc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dgcadyen.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ihqdaljn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lcwgmsuu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ccckbaxu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uysdiimj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tujcdbra.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kjxbzwrr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3updtnbgl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkjkmqvy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wjilaopv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aguoqffh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qbnhcpcu.html


<!-- 参考信息 -->