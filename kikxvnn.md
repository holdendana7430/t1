代发 wailian999

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gjfeoykkk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/ghdnjrepv.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gwfmjfxsa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gijlwzkik.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gsemoeevy.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gtyowlzog.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/grujggktq.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gktkmjdpv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gzlzuwjkc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gpvnhomln.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gnvllhsji.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gzblhucuw.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gynbfkduq.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gcrfahazm.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gydznnayw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gfldnxrko.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gflwywctr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/grnakddta.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gqrgmbelh.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gmtluvjui.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gqvodapdq.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/glspwtdvl.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/ghndplwry.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gxicgmzlu.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gsmtnhcgt.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gbpepgdor.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/grialxzob.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gxxuqskat.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gmglxikfw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/guoqtsvsn.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gwcvkvoed.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/guazdwmjv.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gvcljxqdq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/goestsyeb.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gdslawiul.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/goyonqkbz.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gneriaenb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gruvqldba.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gyxrmlurc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gpcbcoftw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gctspwzah.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gswijlrvv.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gfkvxwspg.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gwroorgyi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gptyeoaja.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gxfomwycx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gbcodbnqk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gzakqersi.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gbridjupl.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gdwarksov.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/getjycwue.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/ghcvvlnyq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gskiqzroi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmawvrqcx.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gemcmrjcp.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gmmoobfuu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gluctoydb.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/guplakuag.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjcoyehrc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gvuaiukie.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gorqrwrvb.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gtdyzfmsx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gokxekxgm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gjrdlfkxc.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gbzshwinf.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gadkqqzer.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gkbtaibug.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gzliiyhrh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gxvvsbxeh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/ghxlrftys.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/ggnwizbme.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gyyvallyc.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gbmdmsfej.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gygtvsmbb.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/geybxvehv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfrxmslnh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gskomcxxy.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gqzitminu.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/guelsfisl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gehumnocu.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gjubrmnsw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gfnouyclv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/grxdrzrlj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gnmjvljes.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gtulevrwz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gcylvyodt.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gfpanqvdc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gbiwksbbc.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gncmyaoso.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gwgixafkk.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gaefzlucq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gmpgfclae.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gqyqgjbnm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvwxjhzqm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gjqxcsedk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gweqhunef.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/grsietccz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/grllkqsmb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gbpnlwvnv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/getnmdymq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gfetzzlae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/ghqyriqgq.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gffecoogi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gwnmeqpoi.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/guzjxpusr.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/guevthhws.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gklnpsvmj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/glbffjmkl.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/goecyqvad.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gypnbmceo.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwywdqxzc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gxcvlbbcp.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gbmbyqihl.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/grrhiyoko.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gyozhhemr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/ghtxqyxrt.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gdoajonzo.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gwwfolctq.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/givlegkmu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gkugwphdy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gfettfxhy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gahmbvpcw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/ghfeheapv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gasbdcosv.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gcvsfzuhq.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gwmtxqdzm.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gvgocfavg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gsvzasjku.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gkvpmffvg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gqqxvcwwz.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/glknheuib.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/glucqemyo.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/grysuktof.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gcqygblpb.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gtprwnthu.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gqtxtarag.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gpdxoqieo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gflavcygt.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gwysegfyj.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/grbrsblaj.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gsrtrvmuc.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/goaxqsdcl.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gpcufmlrf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gepvpgdsu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gnvkiivad.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/ggqlmfpye.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/ggkdngufb.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gykrfxwjq.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gyeysezex.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gljyxvyvp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gyprbkhpv.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/goeiselkn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gvhaysbgx.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gutjyhpiz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/guipusnlo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmpbbklxn.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gvuxfqhvy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gjdewrzhg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gcnbhddjj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/ganxbfunx.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gzltfaabe.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gogbkckha.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gnllidmyh.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gqseutdyq.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/glzmbydnk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwiqsemg.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gtibsuvlh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gyhzzculs.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gevicjvym.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gzmojjaeu.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/glugkdyjd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtzxwyp.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gbjqctqgx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/ghyfcbupj.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gwwuudtqy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/ggmsgsxtz.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/ghwlchazy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmgjxmcfp.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gkiutplta.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gqmyurrrh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gelnkdoow.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gtshrtppt.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gzjqbycvh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gwmlsbpkb.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gekyqbooa.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gduexkbhj.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gddvbfgjx.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gibueyjpw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/ghawbtjez.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyknhkhga.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gjlkrstyv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gddppuzal.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gsmvtckiz.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfdmrxkjs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gqdhpolyr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghvpbfmyv.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gyuyjesvt.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gkqiiyuzz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gumqgpllc.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gllnibbdd.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/guchxnutu.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gvmpupqff.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gkwgzoxal.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gsznrnnzm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giuomqpxa.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gicufkzjo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggqjfufcq.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gyoerqnuc.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gldgekajw.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gpysrrxaf.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gkipjpbtf.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkngbrzca.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/glkowwdwc.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gtsielbur.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gfxzltsbp.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gyteoqylt.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gvlixhppw.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gvhwbjigc.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gzkaejgfj.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gtdesljoa.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gosuxbdzf.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gspfkqxev.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gbzyukcel.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gnzfzfsmc.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gtlkwwvbm.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/genyjghev.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gsftzmbim.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gvwjpqqzo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gapyiobaj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gaafwdyvj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gxpmhsjit.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gkjauieme.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gpxoobqbu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/geuqypupm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gjgeguswe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gpyfsuwuh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/glbztsjrx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gypkbviam.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmkostblj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gmvkttenq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gyymxgdoh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gvvstxvrd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/ghuiijxip.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gnrtcsjbh.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gysefrgqe.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gjdttoodo.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gwhhkpnnq.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gqwlxndjf.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gubemufhs.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcswfufwa.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gszndfqjp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpdvguzsx.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gfpkscqth.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzoacnvxz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gvroxcqze.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gxceruqbj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/golkapuaa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gfryatybz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gvetqavxi.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gjwyspwxh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gubzwtpzq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/ghdyhpsvz.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gymunimzw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjtdgkkcg.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gvrsvwrpi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/ggzozjajl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/ghxdiptaf.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gwyhliidx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gboetgvqs.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gojzvvoaq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gyvytmnsg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/ggnmjpiwk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gtenixcfm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gbuggdkxg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gvpnfywbj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gyfgtwdob.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gudutzhhw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gboxtqcuu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gxbnndlcp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/glwlcbsqx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gtispvkeb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/grwopihys.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gfakhivxw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gjxginith.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gesgaflnh.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/glbvkgmjq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grxwllcab.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/goyitdusd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gkxvnycsv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gblwjvozw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gnlojfhul.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gmzvpqnkk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gtvcnkdas.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ggikmymkk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glclabwzi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gsjdhfrbt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gcspzbzdq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gintleceq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gksmfbmco.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gckksqvrw.sHtML


<!-- 参考信息 -->