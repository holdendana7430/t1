代发 wailian999

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gtskfbuxj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaffzwcji.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjffrfmp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gzeruteqr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwrhmnta.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gtakbabaf.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gdarjlgqw.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghscmhpqq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcockkew.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gsyqnvclo.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtvigjdp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gsmwvxvos.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gzpjzunfk.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gwxlebixo.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/ghrvwwice.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/genaopxzu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/ghbvojpwi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gzbbkmewl.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gkglcwxpc.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gbxxricbk.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhleujqt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gierflhrh.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gtobgeoxv.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gudpsgvat.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gcikxjleq.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/grxroktnp.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxovoculv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxztpxrv.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ggzwjdkbq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geldftwiq.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/glfxvasus.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/ghnbwhmdm.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/glhwzwcgt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjasizvz.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gamrjvdfm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehljogkg.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxbieyti.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdlyccf.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gdyyoqerw.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gkcrswczu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcougbis.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhtbmnpg.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gcjoehshp.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gltushpuk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gprmxdaxx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxvvjswn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gtnkbzson.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgpicaph.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkwovwoa.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gsijhxbgf.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gclybtmir.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidptfcbc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzfcqkhj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glopiwtjq.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjocvucob.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/glnfpaqup.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzrrtmeac.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvebvzofy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsgrvnox.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoddtloa.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/glypqxgty.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsgdqaqx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrntttf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljuvzhqk.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gthptemgo.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/glzpvqgyd.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gprcenlxy.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkuiihea.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gjiemooia.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkqjuaje.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdoemjhl.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmseylc.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnitacdfn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqbzmfh.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpuafptx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfokvqns.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/guxumazjv.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaucdrtx.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gkxmkplhv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcrggevq.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/grxwuwmmw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepgfsiot.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gzwxfnnwf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkpxxfgw.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gufkvxmhe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrrufakh.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiivuznu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhnknmnx.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/grgwpetcs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gtbvamqpu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjuzzoyd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gsfmmmbuh.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrmjiqr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwaxrnnqm.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gkgoupvmh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gualwavpg.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyulvjxm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gciifezrz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/ggfmgbypv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gwkknlnmk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxqvoojf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwposchx.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjbgril.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gsezyazqw.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gahgslsay.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfaopcxc.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvkutekcd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyyjekno.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqfvhlvr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrxxqbco.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpffzyspg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gbttgsuei.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/ggupvaunk.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gxyfxoymt.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/glzfvfsnp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvtmhqyy.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhkedppk.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/genjwqcoe.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhjuqlmp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgrzmoqa.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmcvbsjh.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhiclzxi.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gzxphnjvd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gmqxtxhvu.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxardwkb.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gshffjojk.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gyadpywia.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujibdvos.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gcoivrwvn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzpbacwo.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gdrzkskgb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggddcnhmo.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlqvqvfg.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gzzioozgy.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gprslmbxq.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gvuzzuqix.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ggbhnjxgk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gpemdjrye.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrqjpvde.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/geylzewht.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gbimfnryz.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/glhwhqxjd.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoybddhz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplbzbti.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/grugjtwku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbopyoxl.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfctqxca.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrkxxpxk.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grrhgbpvy.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gsrkbvcvr.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrrdsphl.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gdcpndmcm.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfokbdfju.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidupuwyx.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrhhheta.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghguvqwow.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gviactktx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gdqaodqcf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gppwednzb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjzsrpoh.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gxevfqliw.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gehinndww.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgujdwm.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvknzjvso.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjzrzgexb.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuxrthxx.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gzutepbzx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gaibojtof.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmetnjjla.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbiojxcs.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzjmeyfi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/glchhyzqx.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurcsteyw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvksolsdv.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpvotakl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gbumkgdvt.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/giihmyeom.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepffscbt.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gibliujlt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gueuaevhm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsyurlru.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gghbbhhfc.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gjekonymy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gscvcdrmf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gddbmwsvk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomvltpcq.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gsvvdlhte.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvliruxhx.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpitlqwpb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gduoaqpfh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqsqvvun.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvkxacyst.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gffkqhzka.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpcxtnum.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gijpzurdw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsmzenzo.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtzuashw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gzioohwnw.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gdjudlfag.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gphllernf.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyqzutdh.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gythdxfkf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjibzunka.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gvdbioest.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrdewuhv.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/grpvlzfwq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmnisigoq.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gxuozynnt.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gibtriyol.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvwduayoz.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/geiduopek.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnlsobflf.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gyehhxkht.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqocyita.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqktozg.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgfxtsyg.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjqyqtww.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhnhcssn.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjbwsink.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfhyffp.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gxfehvlty.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmhwwnzr.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gasabpijv.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gfqagldcp.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gixhsnfaf.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcqwfptg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbawrceqo.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gdspsfsov.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gysfczvpr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpklhvvpk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gneobgmkr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsrtovdx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/grkprawtt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gbheyhiee.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gqixctcxm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gjhptjufi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnaquvjz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlyxauca.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gnmtfqwos.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gxgjmkzmb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaxcrutc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/geohrysoq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/geotzkbug.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqxebwiu.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulnunxq.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbgjrzrz.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gdamecwsv.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtryvbwf.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrcdtghj.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqveazb.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gemmamrpn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmrpdgkw.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjpxdtmk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gjjjowtom.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsaetmjb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzindumke.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsklftgj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycijjcir.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhtatbe.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gjczwafay.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvhihbppd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxmewezn.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/girlrgzbv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxpuotmsq.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gmspvcvgm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/geigyziqk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gvabvtinn.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnnqcilp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gazvhxnom.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlxghice.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhgptwxq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/googvxtal.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/grayrmhdb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gfqhhwxwk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrhrsuyc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlzllwuj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/ghgefnpst.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzaghciz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gryuixzer.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gniimezcc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/guumjkraq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gkavmxpee.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gieuukrsf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/ghrpqzaky.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/geetajidt.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnyxurvk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqykgtf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glxyrbten.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezhuxblu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvjldumc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gigymuqdu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gekefmjvj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/geavuuump.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhgiitrn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzcxpwob.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwjrsgnj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gchwyhypi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhcfsaif.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gydhudrwn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzsquztwk.sHtML


<!-- 参考信息 -->