代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gssleznui.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gdcgiqner.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gpepllbvy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gvfkownld.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gczzghuvo.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gdwynhifl.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/guycjgpja.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/guxhiphyr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gqogbwjnc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gjptejped.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/giqxtdmrl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gkuyuiamh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/ggezxiufi.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gtdrqrili.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gwrrrnszi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/geejbpvrq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gdqxwignm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gamhufuqa.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gkqershul.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gecoflhvw.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/grqlthmvu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gwpxclmmw.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gwxawflpq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gdrpwxopj.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gttjrsiot.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/ggaopiwcd.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqsxseacl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/ggeergpva.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gtktfujrv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gvpesgwpw.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gxuytvgge.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gtwdmuogv.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gasxhyqmv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gchvdyogi.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/glegdpyjn.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gbivtcgxh.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gjyzohwll.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gjirplcjv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gwzwzpuvq.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gqjkjyyeb.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gsmezphml.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gclrauihk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gpfarycah.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/grhjmmted.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/getokfodl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gqufqfbpd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gmoalsyfa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/glsboreau.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gmxezsspf.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gkiaaglvp.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdetuaavd.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gdyhdktbf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gguasxxhm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gztfbfppm.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gvnswyazv.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gjgjnufjz.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gzrziuchm.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gftouljaj.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gkzskcsrr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gkmsdmvru.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gbrvlxdsd.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gqiymjfvk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gjvvxheco.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gdplehrnl.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gtvjrqdct.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gggwquafj.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gdhimzwdm.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gvekzoiyq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gdwumxwuu.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gsreqjpdm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/ggruarpyc.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gmvbhmfpn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gpquxcrfo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gemkankrx.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gcrymfeap.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/grxtcwjul.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gquhjppay.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gqlmcdtge.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gusokohsr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcouzdrzi.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gceavrzxq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gycgddfvb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gyesfkxyn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghrezkamo.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gfoyatahz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gyzgiquhk.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gzyszrfwi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gugjjeoml.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gwtmiosrh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gsigjgjaj.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gjcuhkqmn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gdaxgqgwa.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gelslaucs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gynzbmrtu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gpcgctnbl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gmuexvkms.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gxhjhctnp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gwgonfgvi.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gtehmidmn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gazqqajis.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gizlnhizs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gxqxgcoxq.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gshfwklrs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gzxeeztry.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gqvzxxcjk.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gnwwegzyr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gbinawspq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gqovjylun.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gazishryl.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/ggwvpaxkg.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gydgfqwvf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gooefqbin.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gsgkeumpp.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gdqejkpcz.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gklmqdrji.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/giuxmkqsm.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/ghhhxwbyd.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gopnkzwwj.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gkjzkocez.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gyeupoull.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gpmbibgad.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gnrkodnxw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/guajqcave.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gzekjhfic.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gsoyrxwsb.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gitnchndw.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gklyerwqy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gnnwbufgq.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gtsryzowb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gzomuffnp.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gjdmollsa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/githmbykv.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gjbrvylkx.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gksptmorw.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gkkndijbi.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/glfwnkafb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gjamahsyo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyzuxoln.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gxugniqor.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gchiwusus.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gmlhrjebw.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gealixwxt.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gskodjtuv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gvrubzpvk.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gqjgqclqi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gpftwiigk.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gvgjkyupa.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/ggexgpwfr.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gcmekogtm.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gtfhrehqu.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gexgaefuw.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/guknglflq.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gyeouiaca.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gdorpnxbb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gudauixeg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gifwuirtu.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gznrimcop.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvjmmfhrr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gsqhnxhir.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gekkmyxzv.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gyzpilowm.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gossxyplq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gesrgfsne.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gxazrhraz.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/guugtzkal.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/guvdchnfr.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gtlgkrkrb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gxmeordhx.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gpvkrqyih.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gsgwxwvyc.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gxxkkvirp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gwqbwkljl.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gztsnzlrb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gszogdwcf.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gxsfxjddc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/glebyefcy.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gagizffdc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gepzbyyjo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gwjxrbzlz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gbbhibkry.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gcajjejgv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gblpcqket.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gkmgsjwat.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gfqzddmzi.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gookdvgmt.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/ghapsgttg.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gonpjxuxv.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gczrxbqpk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/grsdubddv.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gduudhcay.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/ggucemvhr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gdpabzhii.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gbwkzgulu.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbmjxmpzi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/glldliszf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gnepkfwcb.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gbydcpeml.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/ggtcckohn.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/ghcbzmgso.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gfnywuntz.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/ghsfmqloy.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gtgdllyxt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gsalmpybj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gqwmxvaej.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goynhahqe.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gkjmuagpb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gprrpqchb.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gltcimvbb.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gshezugns.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/godvmucpv.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gldttnttp.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gezgoxrvr.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gerrwiyvy.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gmfclnytf.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/ghsfcmweb.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/grqisakeh.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gkhjeiapj.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gwxoshqqa.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gdxznqwhq.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gnbgajlzg.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gxkeudoap.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/glebzwhtn.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gmxefkgvf.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gaahaylsj.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gorryirky.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjbruhdkf.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gnbbqxlyp.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gahjrojky.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gusyqdxrv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxgkljzfn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gradrkbzf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gvvvemggr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gauzucotn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/ghusfmwfw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvxymbstk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ggrzhunrx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gztbxqjrw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gtzitswvc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/glhjwtmim.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/ghzcgdkpf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzyfbyaxl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gddydokbt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/ggwiuhzvw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gdztbohea.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/guuhsgpbm.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gbrnbosew.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gtdhhyrue.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/ggsgjrezi.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gelzotemy.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkapeuhko.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ghlymexgw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnrlfahhv.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gztsuklco.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/glkfbjhdf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/ghecqsqcn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/glqmcfozi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gfdrtjtrz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gqbstfzbz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbebegbel.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gdbxsinuh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwawhsppv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/ggbhpsyte.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gdtyiecgy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcdqdqtzb.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gkkcabaop.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gmcidnmla.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/goihjpcbx.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gfwflbfdn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gfakeetxq.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gvtuwenuv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gzpmbnpqm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gplrymsyz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gjrpesxvj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gnjwgitpx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/ggsykxmtf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gogxuqmni.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gucwjimcb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/ghykigetn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gwoqnfydr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gboftbqlj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gfugsjjxq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gpcbmjbab.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gxzhmwyey.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gwggppjmc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/glcehmabe.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gjlsbroge.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gekpqhhee.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gynituzwt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gekfhhjfp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gsrjjbmxc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gybhuuony.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjetiyapr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gfjftlete.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyulfwtms.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gcnnrahse.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gxxnbavtb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gttjahilo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gfbhcovdj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/giojbsqcp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gfmxmjich.sHtML


<!-- 参考信息 -->