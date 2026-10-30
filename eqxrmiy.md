代发 wailian999

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmwctqap.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjqoliuv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gqpawibvp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gwbklisbn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaeukosj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyfoiezo.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gfdrsvluk.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsijfimy.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guwkkbtlg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gsgfznnsh.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gkreyekvw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gnldnytxa.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gavrlsmpq.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giekzcacz.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/glazuptls.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/ggflzrlkk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gpupegjuz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/guvioulmz.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/ganmxyyji.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/goenrirwr.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygffrvfx.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/geoaxpekt.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gltrrrrdz.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gajvlxcej.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gzscgeerk.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/grhnzohmx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghumncvyt.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyznhmjex.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwncpjef.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeburmdc.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkhyuqi.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhaslyxo.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpduanbaz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gauwmklwf.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gzegqzjwh.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnxwypsz.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/glrcoylqz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gkpzybtnc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhlmekfg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/glfnvbfqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gldenuizs.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvyyvhjl.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcyrugib.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gthgsccws.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/geacakmps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/goyxawfwl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbjoraea.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gyveescoa.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsolpqhp.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gcoowtjwy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsscehxx.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/geqpsrzbt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxilnqcr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvttvbpjv.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gerjzhrkn.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gmrmlyxoa.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gewqpcktj.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmfrfizy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkiibhxs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjfvmnoe.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gblrxoefd.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfdtrqjw.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqyopjal.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdiuxcdbi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvzholxc.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gsppdjifq.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gklbhwalc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsmdwfzj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gotqtojqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjdbuwlx.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegmtkdbm.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtibtcusq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/giwsegdsx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzibnaqxs.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpecifykw.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbotzkeu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshlznmbh.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjvtrooq.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gerlejluf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqnqhupa.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxafseo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdkgbklbo.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwakotcal.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gdbevzead.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmeeawpi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdanjyoe.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/ggezpeldh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gkoxlftal.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlrzbqtg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqtvnxyn.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gplvzzfga.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/ginptheyl.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvpmxri.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpvsmlpk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gqnglqsyr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgesftvu.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gllootvsz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gkhbcugal.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gsrjtxvvn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/grwdaacmy.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfedxqljx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaymbwrh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuzgthcx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gnaslovfm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwjqquac.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiwuwolu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ggizafpov.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gvqbaknzn.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gxjsedzlv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygsjipsy.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsyndlja.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gekwokirp.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gyxzoxmyi.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmosoqor.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgrvjony.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/grznpgiha.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihutoqcc.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gjvbrrwpo.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/graajyfxp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizxgifaj.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtdmxlwr.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gekwfrqcf.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzpyelqo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gxbtxicwg.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsjcdhei.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gvftkmohf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgfvniwy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/glkrizuzf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/guydesufi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyazzgce.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gtqwznvvd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuutnxvv.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/goylkgpnh.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gvblgrqlh.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/grknmaope.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gczjpysqh.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gfbknltjb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gxnkmnvbz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfspntodn.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbantyhqa.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzziyew.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaxfrkjv.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gsofnoadz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzoljrg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbpqejxrn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprikehyq.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjzqcwu.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gdtmhrtdz.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemmvzkg.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gbocghgxq.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gibkvqkuy.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gvmgphzrx.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gpvzsfjay.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gguqnhmfl.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gnkchicvr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grueelfnu.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfucvplq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/grjgllgic.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxktnansz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmjkdtvd.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotbxbhr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gaelklrph.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghthgmekl.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwjraoth.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gedudpfzq.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxigfxcg.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gizwwmxdv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gwoiaacax.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/guqfpwvhc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfohpgfmf.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glojnroex.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzdgxcqo.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gqizbjcyl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/glgmzyume.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdlviomqb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gwfntunxm.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxwgxbhi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjaexges.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/giwtumtxg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrqrelzz.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwicikmfa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpijjcorr.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/goeozuouf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gjqzketps.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gylhwivdm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsjcqkfv.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrqiwbwp.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjmbuxb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgdviroh.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gthodhome.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gljfyqalp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjpuyjro.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gaurwkemk.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gxwlhavgg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/ghurhtdij.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gempsrwdh.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gxqhklfsh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/ggkpnpndu.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlliucmj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gslvdwxck.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbrlmrnl.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhelvfx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtulwqu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjibdlaz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfohyyex.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gjnpdutaa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiliwkdw.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjgagirq.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzriqbuj.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gbhchbxii.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcmmchpk.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/guejvkflm.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnkdpdpe.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/govlwwftu.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfcwnwn.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtpfvnro.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gketzltlm.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gnmyigjfb.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gluuccfos.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gazneolma.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gqswavnfb.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gtadphwnj.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooszkqeo.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnusrnyxp.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjgzqezq.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/grnqwwcrk.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gkklivbod.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/geqyrjyhn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxczrbf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gaevjekfc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfzavdog.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/ggumpurek.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjvhoaae.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gtafbfjwo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuiuelrh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gddxqrxxe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvvdagun.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjwwreeh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjegfryqw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggdgdofmh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gfkmonsyh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gbmzsxaqj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/glarxepkt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqrurwkb.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtjqxncd.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoexvkhd.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwdedmfu.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gezzwahlo.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamtncnvx.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gogkxxgxc.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzbyylsx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gvagocdwu.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gomzimkmd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfwtntiu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqsatzbw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdorttmlg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gyucjjjpl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbsfovgl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutsjyga.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gjexttynu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gaynlcfav.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtihwjoxg.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeqjnmtg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbuwkpjw.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gybmsrknl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gmtzgrdgu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gnsbrqjnu.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gwdjwlrab.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gesuszdbq.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gywqgusuf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gldvhgrkz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gygnhwjni.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxxzoejb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/ganrkydwg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/guvthihew.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrwdiyrt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gheznbwuu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcluuuqc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gicuamdnp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdvbzlpm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjisdchc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gskhowhxl.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/ghipzulij.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gryvryyfs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvvvvrkl.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsieqlls.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gxnktetma.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgokrehd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcebicjfl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgukeuwg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnxoqjkcg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzclqbu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqknppls.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grzsdsmvq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmyiwufd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaijqvjn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/garopkzot.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxszkwloi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggsjivrsb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyijhgjy.sHtML


<!-- 参考信息 -->