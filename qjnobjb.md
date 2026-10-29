代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gzteopytl.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gxxgmevgb.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gwyuldxps.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gyfkttdmg.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gzwnqfguk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/grlgwidfh.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gygmnkmjw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gzpoyujkp.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/glophodaf.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/geaqiwfdb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/geoavzmud.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gvxnqxlfy.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gezlbkshg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gdkawiexr.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gtzhlhlct.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/glkfdooxl.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gehtothio.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gaamvbktj.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gplddzhfj.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/grvmsenux.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gbmhxtdai.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gwvkbhubx.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gictjwyfi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gzeduvyvz.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gklwaoafb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/grctxykpv.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gtyqqspbb.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gamusimra.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/grmikupgv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gazzjakat.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gesihtahb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gdwctctgz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgmvvww.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/glxocwkio.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gcxomdssc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gorrnmafm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gdtgqjcbq.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gjykjqsfa.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gazcbpkyi.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gumpqadzw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gggjoezxk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gntvcszec.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gqeihcgdh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gvpoepzsp.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gdlikmogm.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gsxwvrsqz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/govvghlhx.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/goqfyucsa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gnxtkmjln.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gzxdczxwo.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gmxijiuvi.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gospltzyq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gepiutwnp.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gzbvgjeza.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/ghywntgno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gmoujtvwc.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gfeoopnka.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gjnanrxvc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gcesfaxzl.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gkckckbba.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gxeecvnci.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gzqsicvzf.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gafugtzda.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/glyxtsalu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gnrumwyge.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gelyexvke.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gbujtnsmz.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gyvtpnniw.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gvvquicid.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/ggvnqbogi.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gynvzfpbh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtfjhjfrv.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gorwvzuwe.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/geavtjfwv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gdzizhlju.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmcpigtla.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggkatqrwn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gyopohpsi.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/grfewhniu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gkwnclzsr.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gslnjhltm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gprjjglvn.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gfkpclgop.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gxmimygkp.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/ggxoaclsz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gemcqnxxu.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gnnhvonvq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gdfeusvoq.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gbmzmijbd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grcsoethd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gbdbhqxuw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gsbbmpmcu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gqxlvcyza.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gaouhoadz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gxdlqdzbw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gaoqdnass.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtmrukszt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gzlotwasc.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/ggdjqxkwj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gqxznaumz.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gdrvswari.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gvhydnhhc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gtzlumvoa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gzfrppcmm.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gzcizxzbj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gtlclxbty.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/geypmxpoc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gffsnbmjc.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggjlqtbns.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gihenbhhr.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gftfpetgf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/ggvdxgqbi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/goxmxuvvl.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gzrrwzkxl.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gvfiuqyue.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gtdvvzkjw.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gzwwhryoy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gbkpxoiat.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gszvudeoq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gvkymsvva.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gurepqssd.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/ganokewzn.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gluzbryav.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gvphoteuf.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gsprgiktb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gftiykhem.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gfnxdvwtp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gxahefszb.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gketybrfy.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/glrnmkhwi.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gvyumkwsr.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gayevteul.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gjeiyebqt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gfiaqwcyv.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gyntcpqzl.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gjcscerub.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gzkrqqaiy.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gvxefmwlo.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gtxbwtohi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/guodyymlz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gussvxhzv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/ghoixksoq.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gfkbsndyk.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/grhvbkpjs.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gaqpfyusj.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gjzyylvtr.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/grohvgkrj.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gfrtfrtmz.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/ggubexuie.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gmdfsiyvp.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gjxrpvcgg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gskojtyqf.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/ggutgxsfl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gorunrgms.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gtlebfigl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gmjnayllz.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gglsmvakk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gvuwjmowo.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gfmycywup.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gvfjjqrfz.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gzaotiqxo.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ghnrtuorc.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gztkbpfvy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gbhbypvht.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gndjlffar.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gigyhsagm.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gyeipaqbc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gchrxdgqr.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gcwilcpxe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gpnucuhfx.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gbhkrjcwg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gqcuqmbmw.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gihxurlke.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gqkidnoat.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/glyepppvx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gkmwfatjd.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gyhzqlhxc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gmgzpppij.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gxkrerzfs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gbcdesnqj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/goamizapf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gdxlpihlf.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gmyixyqbs.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjbbywrdb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/geaqekhfw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvcvnbqku.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/ggawtdzja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gslcroptq.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ggcgtrcks.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gxsayteme.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gqadhaodi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/geznnjdjz.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gmumhjhmz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/grovsvhfz.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gobwmjxzd.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gwgreqqiy.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gdlhrjxor.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/ghsfmnbud.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gwlwgmhmq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gfnhlqcsf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkshqiorg.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gicmepexv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggzhoehzq.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gwzygvzzo.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gcbushrad.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gnztpnhkm.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gwvleohqk.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gdcvmjcdp.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gulaneikr.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gwwfqhuyr.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gqzpasqbh.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gdnjakkvb.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gsatfsqcr.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gnxcfwujq.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gitxlraaz.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gyvgcgith.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gfadpghtv.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gdeisnird.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gjogjcgya.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gwexruaqr.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gdkguycpy.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ggepwwfxy.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gqxtkqntz.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gvuuwaqig.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gkuipejan.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gcgkhmgcc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gflhpolqu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gkdnoesbb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/glzhnjmlj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/goebjbbde.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqsgsxpcd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/govnyaohy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gycbwfgwg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gftnblfxe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqstxxrkx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnooqocfv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gccksbzko.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gkgnchtfo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gydkiezvc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfdxqmlyg.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gauqzkvvd.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gqptcytsn.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gdbvffchg.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gezxnikwm.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/grvamlgin.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gisjkttlg.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gbkqofuxh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ghfxgxewm.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/ggujblhim.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkiubcvyr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gifzktvnm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gjnnowujd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gtposppzm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gnpjgkrqc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gtxmkaxas.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gtbrkxqin.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnyzgwzuj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gkwtrelie.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/geitmpunt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/getwpamcl.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gvdrfeqsn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/ggwigcxkc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/ghxumnbbj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/grwvbiliv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/geurqzmug.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gjbzvcnpj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gtkwobsku.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/ggqbtbval.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gpyxeshvx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gkrecnpud.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gsuvcbwpk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gctqfvehd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/ghlwwfzxg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/ghbvcqiqt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gvhckmyji.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gbqjhqeur.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gbxgxnmnb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gczrchjlh.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/glgmrsril.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/geczxkdvl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbxykztsf.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/ghsgvzzsn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gfjnbczpy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gknhrmhfy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gazmxbykv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gqgpnjkfk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gmfyietft.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gfqrbupvo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/girhqnogc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gnsynnqlf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/guexhbbwv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gkcrvexsi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gcenxkrzg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ghukhbysz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gsitlwkpk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnvevamkw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gvrgpmbyn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gozrrkjso.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gtszkpzen.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/ghkrepyuq.sHtML


<!-- 参考信息 -->