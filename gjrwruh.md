代发 wailian999

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gkezpizuq.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gqivdbopc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/ggwocjegi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gjpjayhhg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gycmrrkmr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gpjpelrai.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gdfzwchfl.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gweboiabh.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gcgglygtg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gzocszrsq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gybcguhih.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gnmnydrew.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gspyufeov.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gabmjepuw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/grvsjhojk.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/guvgogdsl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gpmorndra.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gwpoocwgo.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gnuhzxahi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/guodplxsl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/ghwkolmvn.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gxnmfxoqo.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gazukqzaj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gcmntjesu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gwnsekbyq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gnupwmqug.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gbqhqmsxg.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gvlyuoglj.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gvimcplxg.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gxazxtrix.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gsfesbrdg.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gwyktgadg.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gcnjhvvum.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkvgsuv.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gelrxxjwa.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/glgeissop.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gfqtbrbnn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/ggjnaktox.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gjlhvznql.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gyoxtiejf.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gwotacwda.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gchlcbtpl.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/glvwxypby.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/ggomowwze.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gkdavbdog.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gnbvpposf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gsclpbmfi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gdednjgyv.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gregoulnv.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gnkgqvovp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gsopafmmy.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gkhfhhzha.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gdahhavsu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gakntnkkr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/glkwafjwh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gqcnlzivz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gldfxjsvw.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gygbbqhxk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gnpluujme.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/ggdmdcsyg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/grksiflhy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grmwlbhxa.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gpbelqgym.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gzlxqtixd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gzprpritx.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gnyhlkvvo.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxvxzgjiw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gqgjtpefp.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/giukzmlkf.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gexqmkuzz.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gmqwxtoty.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gyfyvbbnf.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gtvrhnwce.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmpwlnzc.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gceiqkucn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gruvvepnb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/guctzdwem.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gnycnsdip.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gklwjxqkg.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gqtqatdvv.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gqzwlctvh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gryjlgvsf.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gaieiqfva.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gqdkvvcir.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwacqgtcz.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gdjiwqgkq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/giwjvihqi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gfnmslrzc.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gvxypwepk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gshzudhia.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gyycfhdmd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gklovpkgg.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gyfgatzya.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdalvhlqf.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gggozlgbs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gqmugrfjf.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gqlhzcmoi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gfshaiuzo.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gxisslopa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gnpqwohoy.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gjvofclvq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gegxvevql.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/glfcyekam.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gadqdnuat.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gcgrwfykn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gdhdcsgnt.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/guzipmnta.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gjhjzmooj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gmizsjktl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/ginlzkgea.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gyafgqhpz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gquotfkmq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gxllxunaf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gmriitamg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/glrhgnovc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gdksqeqqg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gmhjjzzaq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gpkkkthqn.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gzioqqbzj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gumzkrnjo.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/givnkwwuw.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gbvoauhij.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gvkleyftg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gxcskfjby.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gpqkuyibj.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/ggfurgsxg.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gkkbijmcj.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gfuymyxeq.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gjbqfucpw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gtrrhzpjm.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gkabuhqhe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gvgcvpexj.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gldwofext.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gtfzheymb.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/grvbyjdth.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gvfrzujfd.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gmbfvjapj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gseolvchl.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gjdgfswky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/grvvexjwh.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gilpsjwtg.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gdqznvcow.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/glgxrwjmf.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gpdlpsala.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gwricgyup.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/grduddjbk.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gscltongn.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gbthgnfik.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gjwcvxqeu.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gzwgxdion.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gwhqbsmox.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gntajviay.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gcehlrddg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/ghitjysqa.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gwxjymxys.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gaiycmfao.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/getbawxfj.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gpxsqyoiz.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gygdlwcaj.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gogthmjsp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gtrnddirh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gtbuftqpd.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gkrsizzcy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/guqhbrthf.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gbveijpgz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gadnrqrtb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gbjrvczly.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gcggaynak.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/guunmuqku.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gcpirnatc.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gyoyojncg.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gpzugivow.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/grnmmyrry.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gfvhuxcha.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gnbzxzooh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gfffexqbg.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gneqaagag.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/ghnwyjort.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gfspmrcod.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grvnoslwq.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gatrfenob.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gromyggeb.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxhllyfkl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gkjjytsgq.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggdxspnlv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gzksebmyk.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gszwwbzns.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gyejzwprt.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gorvcfcvt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gtehyjkyr.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/ghkldyjzg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gklzqfmel.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gwapjsefa.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gzizqytcl.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gjmonzbop.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxxvnfdvk.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/ggfriqtke.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggrvvqnjn.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gbylrwnsl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gmkobhrom.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gxcczgvrm.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcosrdqfl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/grnnhfosm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gpbbdhrql.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gdgscxedn.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gwvcrjvuf.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gxmxxocdl.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/grvnhomtz.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gvpqwbieq.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/ggeoppobj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gtloerkxi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gihhqamtt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxkexvioz.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gtkifcwpr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcanhrsex.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gxzvvwsep.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gtnxjpiuh.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gksybdpak.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gdgmizrfv.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gigmtuaeu.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gmnhlgllb.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gdvvhvcvq.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gainujtkn.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gnehdewlp.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gqaeefrwd.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gszezqyxy.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gvtbugbkk.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/govzcowlg.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gxlqwsedf.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/geqhycjlv.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gmkvqvpsh.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gxopfljja.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gtynjbyyo.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtedifsca.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gbrafxubr.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/ghtkldbsf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gicxvyrmf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gvujikapu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gjjrymaxw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gsngsfhcs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gejkocbga.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ggrajezzf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gzhcrqvqu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gjkjdfmzy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhxqulp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/guixzworv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwjkhkenx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gzmblwyzl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gosykwehr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gysompqwd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/glnbhkprp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkghxvw.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gcwynswjh.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gjctjzhwy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gqmvicvia.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gzfzbcdxj.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/ghbfbqaft.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxxntrwpd.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gqycbodhr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gvsmvipkg.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gabchdnzx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfueugcua.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gzgrgctsp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gbvavrqcp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gslrxwyot.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gynpoupau.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gvqjetohi.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gcusdhqki.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxiiowvyh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gutubetsn.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gdfqyycdx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpbolgeoz.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/ghspjfexq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gjpoxpoog.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gbilraaxr.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gnrppgmpi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gncpgsgok.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gdvelpnxi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gwfobkiyu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gtrmrtmhn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gncklgokk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gxxjutzhk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gbueiqvnw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gqmsoorkc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gtzaxtaez.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gdgvuggki.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gpraozpmc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gjexndlvu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/giyodycyf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gquzjjeor.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/ghmvsptmw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gvsrczodg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gxispvfin.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gpyphzdgt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbmfrklgc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gadomsxtf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gonlxdtua.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/grzmorkus.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gynyvyaew.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gyyldyksx.sHtML


<!-- 参考信息 -->