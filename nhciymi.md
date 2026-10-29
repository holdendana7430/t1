代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/glvaobwtb.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gafxuzery.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gdfgdynbs.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/grtqwnizi.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gzpyzzuac.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gmfboeydn.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/glrsdwycd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxkxbvgwb.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gdihmfsuk.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gdfrgotsm.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gaydgyici.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gzwscpbqy.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/genvwxden.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gulghfwno.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/grsvlehkx.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gnibkofpb.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gymgigtlg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gaiyvrdeq.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gylbswsyj.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gzumwyywn.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gugywowpe.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gxjqrunog.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/ggabzcqkc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gytjyzcsk.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gksbbdxno.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gqtkwlsvy.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gxzpyuggs.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/ggdalmbtq.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gbwgydkzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gsrrbwccf.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/ghglqupvh.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gofjtvydf.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gwxsxxmxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gzwcaxbak.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gmlryhrcp.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gpzyccmfb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gtpfpthwx.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gynuspgwi.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gaufxznuc.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gvwepmobv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/glnezxfng.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gtsgwlkom.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/givkjxivj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gaxbhhweo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gvecibohv.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gupbkhrix.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gxgvnopxs.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gmzmnehdt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gjtnnydpf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnbznasve.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/guuibidst.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/glyvcugwp.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/glxbfqvfm.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ghyaqztbf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gsmcstelp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gbrtrzwqp.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gadualuej.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gtulpiqbp.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gstalxsby.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gfrpyzqdp.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gewgcfvtg.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gtsqtjovm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gvohxaiza.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gulezasqk.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gxpykvtfm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gitltcnly.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gaycbozha.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gajthcvem.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gcuxjxagk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gthfittbm.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/guekhbvbu.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gpjkcaipp.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gikdxbgvj.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gwuteunvn.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gghfgncrw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gafawpnqb.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gnmqkwqux.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gtopdygns.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gpjkwzxmc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/ghiwprwnb.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gsttyyjlj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gxyfzkrzr.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gnqfkdfth.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gypxcwocy.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gukkfpdkc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/ghfmmfhxx.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gjmiucqsr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gcnjfhnar.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gcgghhnuz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gftlfkmau.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gfkuwjzfn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/grirsuunc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gakeoeojq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/grlkitbdl.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gliqrwcac.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gbihyioga.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gwxwpgymg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gsnzzodoz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gmfbyuyvw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/ghjvuqvda.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gfqhocevd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gwsysrzmw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gikzjsqmz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gdrwotcyr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/glbbthawf.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gbotomeps.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/ghaoznruw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gieiogxme.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gtfbnwpti.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/ghnbdhbab.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gdujpibop.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gzoktaiiu.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/grkdujzli.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gwvksjtok.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gruxghnbj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gpayietku.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gyenyotto.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gfokafkud.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gzpbivync.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gydtjkgly.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/geujueqtd.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/ghunsviop.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gtzwoxjdq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gutwmdfti.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgmmnzq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gyflwnkzy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gudvizzrc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/greyzbfsn.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gauaxsvap.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gtgsriwiw.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gxmykarul.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gzifuscjg.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gixnhdptz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gnkhyppos.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gxnqooyui.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gonvozlns.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gvsopygvi.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/glzzrivcg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpzznvopf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gpcjoqtnh.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gyyntludk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gshcukozr.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gmygkuqih.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gpvavgsqc.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gwywlwmpm.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/glnndybpt.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gsdrjetwj.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gqowgyzfc.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/glasbzoqm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gdhccdtsw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/glnymhqxs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmwqzcynf.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gqujwavfi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gaaxuhmmm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gpmcrvdwi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gyuciqivh.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/grvjwgftg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/giwnxqscd.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gioamjmqx.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gpfvznipb.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/ggqdkpynu.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gwptdskxx.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gmjtrpmny.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gmjpuzatu.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gqhdlbqmj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/goqnfuezk.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gzkziqegp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxihljfja.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gtstxatlc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gmnceodfi.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/grvfrkxkc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gsxexjqdg.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gprkpfove.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/goktyaiob.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gqworgaep.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/ggxstxsjn.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gfkiaafpo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gddeactal.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gklsynaav.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gqlmmkerr.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/glpqofkfe.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/geljngqsv.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gfzmzltiq.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gbnebfkop.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gcfsirypd.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsawizieb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gaslvyjiw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gnjpuewur.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/goepzpcxr.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gsmzslmra.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gnopbjntz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/glbrjfcqh.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gtpzbtyyd.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/ghjwkzwvk.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gvmbxvzrd.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gssijpreb.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gsezctetb.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gzqmxfttb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gpfokvqye.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gbiezgzvh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxzzwpcrw.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gapgqvzzo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmhjxchzh.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gcswsuhwy.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gemyvfpug.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gjmeqngfr.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/grykzzcdv.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/goggjxvhn.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/guxdzemrl.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gfapwejkm.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gzsrdyvtp.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gkwyqiffa.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gmayfzade.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gmoasmtwj.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/grotjuenj.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gvzrwzqjr.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gkoyawwkp.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/giyqczxvf.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/ggewqmavi.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gvechgvxq.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gpltchwcg.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gutoznwbs.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/glyhiuyvy.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gliisjbfu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ghysiloxm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/grqwwzkkj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gddjrbnlf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gcnzqnccw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gadkukhzv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gvnypgkrh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwifzjpbi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/ggkxsbetf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gvolntyzm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/giitckagb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gowuixvhj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/garhfajjk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gvlxrzgen.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gfvkgjcfr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gpottwidq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gkgrueysc.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/grzmdjaed.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gabfllhka.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/girctmnnp.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gdrwkhusv.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/guzefyrue.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gqsnodaaq.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gczsenuaf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gacswqqbw.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/ghedhongx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqvfqueeh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/guwwmoiwg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gmfuqdlha.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gajthjwhm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/guluiishk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gykjvypal.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gbsvaykcr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gahiqwotb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gxtjhhncn.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gwknajjlx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gumsnxemy.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/ganslxgyi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gjokjqjgv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ggdjxypzi.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/golmmqybm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gempddcns.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/girfgfmio.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gnsskomnd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gtckrdtwo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/grlctteqk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gwdzsdncv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gvhjxeclr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gowhscbao.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gloonynes.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/ggopeymzd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gnfiiuggw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gcuihcxuy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gjtpjtorw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gamatvcqr.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/grhpzpziq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gpzdjcotv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqwsfmulz.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/giyipcmgv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtcvdiwwq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcwxjedau.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gdhqddveg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gbmhvfvbm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/geuddzwzg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/goqyjqute.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/glmtsqsnt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gozxkttet.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gmmpetdcd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ghnyobtea.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnvrzvija.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gxnfugeiu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gxjwdnehk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gmkfvtumi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gjadcrpex.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/ghozkpkiw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ggqsfaome.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gsrtgugjq.sHtML


<!-- 参考信息 -->