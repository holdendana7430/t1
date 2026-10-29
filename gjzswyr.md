代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gpowyyagk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gsagyemxm.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gyhygrbcw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gijdpqyxz.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gnapdhvmk.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gvvolfncf.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gynxrjcis.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gmnnihqwv.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gebcjyswv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gxvtwlajw.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gopfhldru.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gqdceqhbr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/galxviwre.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gnecqatxx.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gmeaixygi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gbwinahqx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gbflzwrgq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gkikydigj.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gjbcdbiij.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gwmvmgmfh.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gqutestkf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gyadaavze.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gwotoewbu.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gvsfotunz.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gzshwvwwu.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gqwqbnsoo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpszmuwnl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gxxqyyavj.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gsfypdaph.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/glwtdgmeb.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/geqzsxnym.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gaadqrgtp.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gssiuolqb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gryvwexni.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gvmaignqi.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gymxnvaey.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gniwujgeu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/geeoytomr.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/giiszjaov.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gcdjcvprn.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gpdyemfdr.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gamktltyc.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gcmnlqqua.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gvxgbnzdp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gxhyxhbql.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/glwqsxgbu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gmyqxuvlu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/genrkzvir.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gqmpyndxl.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gmzmjjujb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gcqwfftfx.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gtwuwfefb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gxdvnxfpv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gskybbjot.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gmhllcbfj.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gxavztrbj.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gohxcohsk.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gfvcgvhht.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gctesrdno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjjmimes.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gnbwypliy.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gkgxduscr.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gvtyrnnmh.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gstkoieby.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gxqlynzmn.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gddyuwgdz.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnwyiufox.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gywlmaomv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gvywdblct.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gmetxupgh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/ganezoayf.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gsvpoyzbb.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gqdeuavtw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gttyxlxbu.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gnvdxgpoj.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gghporxsa.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glddngtof.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/ggnxkieec.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gebttrlvj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gitndszmq.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gxtmajwvx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gzybppsoz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/ggqjnruzm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gwozeazbn.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gczxslsjz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gimutsfbh.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gnhahfujg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gopkyegcv.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/glpaaryar.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gkmkagdxt.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/glfjiyclq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gkvbuecpf.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/ghphztbtq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gmyfuhcjq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/ggrrpyjrd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gogntzojd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gcugrxanf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gtknmqzgn.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gapkckgur.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/glnxdnavh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gkmtayegn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gxohqxrbo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gjeenxgat.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgrtxeq.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gentipogr.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/guggwfcyo.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gqehstlue.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gfrlhewug.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gtumlzgud.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/grqcjjwia.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/garsvaxcz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gkrwxrjkv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gbxxxjnob.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gihkrjbln.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/grntlushu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gkbnrfqio.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/glbqkvlpn.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gxyjxvmmx.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gvyqdeglq.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gmubdpari.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gptnqzdqd.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gwkrwkbzd.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gprztddth.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/glkwnnbkp.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gjttsuhze.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gnftbgldt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gzolpuhte.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gmmkzcwqy.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/glaeyqzfr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gpyvjhuvs.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gvpzufnnv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gmytzdjqg.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gzgaxsfkx.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gybpshewi.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/glfmcujca.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gbsutcldc.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gwvhylgmb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gdqowhnml.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/ghbdltwhf.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gpkjvlwma.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gdvatclfj.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/glowcxdvs.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gyaqgiekg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkwvfcvcl.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxehlijbx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/geqygiqeg.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gdprhzhhq.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmgdnxtko.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gsutbmnil.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gfsmrfuie.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gbhlohtlv.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gileqymna.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gqbkgmstq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gieumwfna.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/guuavjavu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gjacfvhmg.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gaslhvdzw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/giporuglm.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gsjqmcvwq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gpglitjug.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/giziitsuw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gqdhsrdhm.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gmauukcrd.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gzauzfkoo.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gqoebhygw.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gwcgusabk.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gtkbgthmc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gkksebwpm.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gamjjpgmx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/grjeitosa.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gwgpmcamu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gecgkbcjp.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gpoiwjyrt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gxcwfyaox.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/grnccfdbg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gxizkonfd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gggdmllcn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gruowhyuy.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gxttjuhul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gpqlgsmmf.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gmobjlzqy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gigheomzw.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gpppcefbr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gchsonwef.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gwxcorgwm.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gossqiitd.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gpkhizioe.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gmlbozsvz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gdscjovaq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkzzpftty.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gekjldbfp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gcbxkexuc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gsrqtrpla.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gswrytbuk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/goestwskz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gjfwhsxgg.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gociutkmd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gjnjfysxv.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gblijubjq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gamtfurav.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gdxewabat.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gzriwdnkf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gsbyndpts.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/graspcbxp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaagohnxi.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gpjosqogr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gamhsruka.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/giaszuqle.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gatgeelmy.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gcbxpvnbt.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gzkddesxd.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gdqwbbzle.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gdjtglitr.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gjunotxnh.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/guqmqzwnh.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gsuycfgot.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gnvibowxd.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gioqofdbk.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gdsfikuhl.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gqmsuynsb.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gogocdyzz.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gkfoencnt.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gebzsnswn.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gjyipewns.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/ghyfvakrs.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqczqnahh.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gqmkejqet.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gmtkscobq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gjaxmyknp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/glfdykyac.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmbiulbsc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gvrclqief.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/ghffscdbi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/golyybscd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/goryfrebn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gwvtscphh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghhaxangd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gyqvdepze.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gcpjjstiq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gvsnaxqll.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gumggpmku.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqlwega.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gicopnjtt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkkdmesrx.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gznervxoe.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gfbefqppa.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gogkcdryi.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gbtfmkjij.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gbssehzxc.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghtebtrdb.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gsgwibaet.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gcycjreoe.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gjsjjyyfy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzssduwks.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gwjporggj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/giittjtkv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/ghyvnhzbf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/golayqict.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/ghldxafpo.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/ghwbcwxfl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpczejbll.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gmsxyweib.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gbnrefqpa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guqeqgfcr.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gcpxksisb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/galjrthqx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gynwjoblv.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gakqowynr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gjvqswply.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gznnsccry.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gudfnwkze.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gzzvqszph.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gmpwfrmyn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gzmnlosco.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gnkcpfexw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gqrqjwjse.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gotfymbte.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gzyfsghhv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gveokdcdd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gpyjxhqne.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gpzuyusxt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/guqbdcceu.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gxppcnjnu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gaojgjgds.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gepokygel.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gkacpomgf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gislnycos.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gapcviynx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/goenbzkqu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gnkgtwpsr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gkpybdwln.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gosjqnnoy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gvsaqkchs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gvzjyysip.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gjtgceenk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gtvideqgs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwfdxgcea.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmghsoztn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grkqjujwm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/goqwluquh.sHtML


<!-- 参考信息 -->