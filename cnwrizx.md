代发 wailian999

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gniixlrer.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gbgoqivls.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gkaaavyma.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/grbztohzi.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gshhqelae.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gmxfkeitj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gqtoqmtdv.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gndbaaezd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gwcrfyxoh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gyfymxidg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gntqbpync.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gagenfqev.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gaejqterp.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gmqoelwja.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/glqcpqhbg.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghkbzejto.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gdncdrtat.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gkiqwzgev.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/grzaqgxnd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/ghrlclgsp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/ghrfdsxjl.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gpexyvsvi.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gonkznrts.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gpyzgndoi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/glolaggua.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gycrqnpju.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gidrhhwii.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gyuisspgb.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/ggknwqrrd.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gzzxiunkk.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gmasuxqcx.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/glrqsdrdw.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gpmdntjyk.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gxphlaekq.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gudphssao.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gojjwwohs.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gmmgksspq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gupzinyzv.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gouxmprfy.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/giqoipwvw.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gbtspoyrq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gsckmeprr.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gqtsrwlfz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gzirpykcx.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gbqdldycv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gidrlkoem.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/grecpszyk.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gbkftiser.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gwymzvzaf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gwiqiatze.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gbjatrecc.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gpbukyoib.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gepjorhrs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gjmyjqbkv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gybgdiqon.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gkdfkqlbh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gskdqczdi.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gmtltxomw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/ghdobkyea.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gprbbiknu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/goqfhigxj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gwdxdtanw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gmmaieduo.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gfqzvlaue.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gkxcyrzgf.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gsxhdxddk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gaukzfecl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gjszotamr.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gywwespqy.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gnweasxlv.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gahukqjgm.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gzprqbovo.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gljeuiwvx.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gzlygkkgk.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gxcwrnmou.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/glkgluywo.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gdvghuasd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gtqujghqt.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gsqpsqcwh.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gfiwnocgg.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/grexzmqjm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gcnwtzikf.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gjahxvgdk.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gbhaupxqc.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxktgybun.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gpfpzzfuj.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/ggbwjkyyt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqwgbsvjw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gqxfqxrpz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gspkrcvgj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gbsjucatc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gvnmnjhaw.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gdqjeminp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/guiqcroxn.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gszuqcsqq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gfozpxfkz.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gltxejjmb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gthexibmn.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gbrufylhg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gqtdxwgyy.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gctehwehz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gebkqldcs.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gzvblpjbo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gaivadzzz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gtxdozpim.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/ggxjwqxaa.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gkbrunhhr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gpqdgrowa.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gwfjynilk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gkzaddlnz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gcavklfcv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gddiqspda.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gjzotaxsl.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gizdfgevb.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gwwulswhs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gzdxadtjo.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gatvxlrst.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gxvupgyrw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/ggzqmfzly.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gogrqblhq.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/ggqrzheyi.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gtqfebggn.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gyrrfxlyp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gurvuzchp.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gjrymoush.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gbsyfadqz.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gkeokccqs.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gplpdfhos.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gxymhbnuu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gymaclswp.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gmhuhgumh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gwiojzkpe.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gjjdyibrp.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gwoqqwmga.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gjoirewqb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gsraqstrr.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gdfxqqpcj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gavicuwxn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gcexatzhu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/ghiqunxkr.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/ggxqgksxk.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gszqwmfcv.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/grvpnwxtg.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/ggtlqnnbc.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gokpnmnlw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gptwiyzlm.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gafsktyva.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gahvyldop.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/guyljqgzc.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/grdipoaag.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gysdwhden.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/giyxkgjzl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gskefzgch.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gqmosfxsm.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/godkazhcf.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grkygerqt.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gpysewmam.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/ghwvbiuci.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gxvhslyho.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gqndzoffj.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gktliedke.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gwoklqmuq.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gtuxrbnim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gfudiflkb.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gvukqwdmr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gksavwohs.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gzdvebtoq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/guzrfopqb.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/grywywyuv.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gqmnlaxas.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gfauzanid.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gmjbypgzv.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gcpdfnhbl.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gtblfdykn.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gfuimxqke.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gvyrdtlgb.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gioretufv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gwbubgoxp.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gygpheoix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gumncwnkj.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gkjaufbah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gwuiodwnq.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gpyrbvxgb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gbkxexdno.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gxasjiasy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gqjjvqnql.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gbhqsufhz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gtvfalrsr.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gkveoppci.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfxjkcuq.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gggnlevxv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gqwqxivjz.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gayqwtnhw.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gbjumolmr.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gmzzwylck.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gooyigcsx.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gvsmvvffi.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjkspzmkc.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gddynnopt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gxkognfzj.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/ghvkktvaz.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gfaxatfzp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gclevjzwy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gktyspkol.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gkkpfnqzi.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gmkzhhxwa.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gdgvgrfts.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gtkbhklij.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gswfnhnxp.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gkeecnljf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gcdaiatxh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gtrjwdfkl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcksvoozv.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gqxaegsfd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwkblvglj.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gqufxdtpu.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/geghtvezp.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gmevpzgmf.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gsfiocekv.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gmdcfhtqx.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gwvhhyssn.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/glagnrvsl.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gqgzuekbi.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gpgdjolqf.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gyynymbvi.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gqoyoeulr.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gortaexxz.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gwsutdpwc.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gdehphepo.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gcluvxmsw.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gchrgaabf.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gcwcoyvlc.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gcrxbjgrr.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/guovxhppa.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gziiakgbi.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gioenedgc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gnrkcijps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gzxsjzwtz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gqbayscoj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gfuqjiqfh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gblglyjym.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gzynsczsg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gnpyqyick.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gmmzwadpg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gngmfivid.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gykvifyth.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/guewiesvz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gswjbqlzu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/geohvhonf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gtzcysvte.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gxzikuozf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ghalkytqn.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gswfclmln.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gixqganqh.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/grdcfnggk.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/goslnuovw.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gdksshwsx.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gquwqafvr.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gzgjeampd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gyarnmgcy.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gwyppirho.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghaklkfnc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/giqkcljpg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gjqswbzid.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gfnpapdfj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gkjzcrljc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gihrnwudr.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gpddtjwym.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gegceqedo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gwtzcbdxv.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/giiwfngcd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpamzbgwi.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gmzcxyvnj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gqulolsqx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gdgputefj.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gwvlugbwg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/ggpbcppyt.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gwzdhotyx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/guzmjcbyq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gvscyensr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gpwwjmwfn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gusnjbvpo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gayqfmuig.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gbwgztwdu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gvilnuizr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gsqogirlh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gqnsucsge.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gusevdjhx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gwroibluc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/ghpifnsxk.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gzctekdby.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/giuktvotk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gjogesdjv.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/giicxpybs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guijmqrdb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gaweeoxhh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glxnflgky.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gwpsluwbi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzykmvura.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/ggvwwrpdm.sHtML


<!-- 参考信息 -->