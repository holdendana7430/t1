代发 wailian999

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/grvxwlomi.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gmqiglscb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gtsrxyrxr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gvevnkaci.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/giesobnlx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gdcsukaze.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gxmpntlws.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/ggefpelik.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gjsagdemk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gnhqfjkwr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/goiztbwms.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gdnyqfjkh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gojblktxb.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gkwsmgmni.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gasfcijou.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/ggpnjljai.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/giziblmvy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gxububmgg.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gphrlglyq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ginfggoxe.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gvjmhmfjj.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gifmjpkti.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gwsgygmfh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gsanewxxt.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/ghgvpgcgv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gpkccqcho.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gvgupqete.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gmxznbney.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gsmmcoenc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gmjpeydqd.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gryynqslp.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gbzmquitn.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/ghgcobopb.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gngegypxi.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gvdysbwsh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/ggsjinazv.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gmcyiipfw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/glcbjpqwd.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gzdakwekd.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gtnkgnyrh.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gldechdnr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/girxzvcmr.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/ghwrsxhkb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/glzepiiwy.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gcfvibrif.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gvwvtxjaj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gmueqgjfy.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gvsewwslf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gfyepspqh.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gwbkgavua.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/glpisnzqn.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gnvalkdoy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gsdphewbz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gmjjdooim.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gdbjvprww.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gcjwqxpud.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gbfpamsvr.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gpfyxdhsj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/givuvdski.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gvgjagdxr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gvculghpd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gqlfkmqop.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gnonuizgt.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gvkzgfswx.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/glojmdkda.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gansbuotw.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gbosumgnx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gdurbfhof.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/ggehaxdhn.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gnxpuaxoa.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gdlkqzqqs.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gvcbxyqil.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gvwqckxwe.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gizjiqjxw.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gdtdzyhtb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gdsyuyedp.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gxtfjwkhb.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gzoubpieq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/grrcjofki.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gcglihacc.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gievlacni.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gjxphofhi.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gdyyrmjqx.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gcqpauzki.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gifeqcweo.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gxfjrmhrq.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gdgbxolpp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkmdqbhbo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpoimsy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gjzxxbylx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ghlvxgsyf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gxqlitpuf.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gqglrlfjv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gjpmsaelt.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gjpzfmrfh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gljfqjghr.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gexifbgix.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gbavyvmzj.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gzjbnkckl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gvahcfmbq.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gwoktjwug.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gccsozpzx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/glbnrijnz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gxmcygvfc.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gjmwenats.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gujscjxma.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/ggwuplzxl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gszczpjit.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gxxadaaaq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gdlbezztn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gfidjzigf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/garpcrikl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gmdovqruw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/ggxkxpipe.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gwpbycwlc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/ggqjcosuy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gnghrykow.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gatszveeu.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gwmdwzyvn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/guhnyglct.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gxsvrfjhc.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gcyvxrsso.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/girasdgnf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gnbmoejjz.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gqzitazyr.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gswbbrijy.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/ghmygmdyl.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gmivlwehs.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gavnxaphl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gawyvhlko.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gtuqmumbh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gceachzlr.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gobyuetzp.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gophydhkk.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gbymrabvu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/glxzgsgnz.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gihywyofh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ghfsuffko.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/ggxdpfnmg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gcuuwfqnp.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwxuagz.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gxosbsvcm.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gpfcsoqgx.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gicylturc.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gaxaeelds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/grnswnrij.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/griacvydh.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gxpipnlro.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gwkuakprt.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gifoswgqg.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gysfhuejq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ggbezwyaj.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gbfilzeif.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbwapwy.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gcaimhpzw.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/giytvwajg.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/goevmfaxo.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gobztfokm.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gtbaqhwdm.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/grcmnqscu.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gcrbldzrd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gpcqlfbun.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/ganmvsldf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gmqclguzj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gtqbepjep.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gbypjnjht.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gmebdzwes.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gbnzboikz.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gwjisxcyz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gxarjyaba.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gigktvlxl.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gpjqqarzc.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gibrbuync.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/guhcvyjyf.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gclpaegsi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gfjgsuyii.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gfezqxywe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gmriwqqld.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/guhuyqznp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggwaridjr.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gvnsapfyh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gcdrpwukd.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gmdizxcph.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gjnrutunn.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/grbpgxgig.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gwfahmnpv.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gbonsaqfp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/glbxowkjd.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gjytxmaxk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjaspqxgt.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/glkncpdco.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gvnyvspgl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gmfjxgtae.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gthszvmzz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gsilyryjq.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gqlltzyam.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/ghavrwkfv.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmmhcubla.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gklkfavoo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gkwrnuqoe.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gdjyrcdnv.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gddyfbhze.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/glkokxuih.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gqkpbckno.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gmrpchwgk.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gvmrfdshl.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gmspswtvy.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gfedegccn.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/ghjcxtxow.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/glubszlca.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gpmrxegdh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gefsyozvq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggiyucxbe.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/ghaknbgtb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdwkpdgev.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gwgcdxoep.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gyajgrpqb.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gmqjbuxew.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/ggcfosaqo.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gcwdhkike.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gwtnhgxln.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/ghwhnvzpk.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gafggwwqq.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gdwzroanp.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gbfoqolmc.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gsglhbxzl.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gcdzstvzq.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrbnnpb.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gxcqulljr.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gfthrimwy.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gngreycav.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gykkhotec.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gylzjehiw.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gryirciwl.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/ginrfndfo.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gcxqrvdib.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gknbzptrb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdikydyyr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gxiagoilu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gsqfynsdu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/ggfbbvfgk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gisbovjwn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqdosfaqe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gzgypebnz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghrhfpffx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gfcynxoda.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gfuyuubfl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gihlxsgsg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghhkpkosp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gbrwlkrkq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/glnyquyih.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmfuaxlyh.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gvtezokyo.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gfzhbjavc.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/glywkgcsp.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gzbtaiwgg.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gibalzqhj.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnctmwgfg.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gpdkfbayu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnoegnoie.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gfijdfbmw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gcmrbrsbh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/geeglfueq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/guuamplti.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/ghqynkaer.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gwsosgxnh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gviptbonn.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/geamcsopd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqnmwgyhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/grnrjydky.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gysizwbwu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkqmjetsj.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gtmuihgre.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gcmkbodjq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gfacnrhqo.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gtgdsitsw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gavzbrddl.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/ghbnpqsyj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gwmprvloc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/glwuogyxh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gsxypihwv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gcwsrjvop.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gtzxaaslm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gmzpxjjoz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gbkvsfqas.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gbgmctsjj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gbvxiiklc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gtuzvmtnp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gtxilbbjx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gwssaralu.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gochjmmsi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gqntqyteb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gyrzuvbrg.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gdrhmzout.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gstxqcdai.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gufejpdji.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gnhzmzkym.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfcomkcxq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gooevdizy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gnmoggdun.sHtML


<!-- 参考信息 -->