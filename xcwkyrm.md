代发 wailian999

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gkvlutewe.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxcwgfig.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gmqywslou.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gslxplenr.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gsmkzcpsp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/ggtnwouez.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gbhjnfqpl.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gormzjmda.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxqabcuo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmpkwezo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gkftzmjlx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftphxihg.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gyihkxerp.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/goaokgmbx.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/goxpmzpoy.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevfezvtk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtptttwhr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gymigoopa.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwhdezym.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzcfksfm.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gttyegowr.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gavcyvanf.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcqmccv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbubbjtf.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gxelojwaz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gglgfhaps.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gcjddtcqj.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gamyeajiu.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gozmxnwtl.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnfmpkyo.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gehlgbvkd.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gakuionzm.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/glpnudmwm.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjmvnoft.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gznjpzalj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoaqpqdo.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gemyiyjgg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gvbwmqksb.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gonskcjcc.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqlbrukk.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunkvmsp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyydxfych.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gscwibxdi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvrvleyy.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gkfayjydo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxsprfcd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gpwawuvtq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gjegmbzfj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvvbxemq.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gwsdystmy.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchgrdbeq.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gshzrkkoa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxbrewzb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiyovmnq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/glazvtueo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqimvoxju.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgqplstp.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gvakbutcl.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzdeuqhi.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuewwknl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmtgyfa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gywupnvjd.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/godrntcon.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gralkpoay.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkskmpnhf.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gakevuagn.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gheyjkmul.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggyjbebxw.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwbeuqln.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/golmvualf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/glofnvhdb.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjddmpupo.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gwucqsmxr.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gojjqcule.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gquirhzru.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ghohxmcgh.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqmmruaq.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhzzhew.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gohylsget.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfacxzxkk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvocvmeo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxbvrhvh.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsqjfxoy.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grluquvcw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/glhhyhsdf.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxuedjhm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gemerwiny.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gttployff.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gagukyxko.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdieybtwl.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbdkljlx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqbgrrkl.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gglauaxzg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtlqaqb.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gjhdznfop.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyezwmjmk.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gosljbxyd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gohsokjrc.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gklfeflcd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gbucndrsh.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbwvzvno.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gilukvqdb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/ghanwegfa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gysljzvln.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gmduqcqel.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvmumwxf.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gxqbowsia.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gjmnhmvok.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqvhkxnc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjexdqavq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwrdsln.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/geblibjjg.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gswcdcjsv.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlpzlopi.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gckqukmsu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceqmpgof.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gsiqzdqpt.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gvphgumgo.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkhbyhvei.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixzlvncc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcqupqj.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlbvvdjd.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfqehpno.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrjywmjv.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gewefenbk.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gelzousde.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfcybwds.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gnemdsydf.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtqrgfdj.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxfhnqx.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gtilpvjyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/ghtbbftkn.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gzzmrwulc.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gjrvdimtc.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmcfjxnf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfheyazn.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gxycdinev.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gefwcodwa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfhfgdvs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gpawaxytf.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gnhqwvjvu.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gkxmvhlgv.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gierbhbno.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/glsgeikfv.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gbnbftrjg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganmzspvb.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gcymbellq.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqzxqgtr.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gweaqhait.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gqdeubirf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgbyeft.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezoekxwc.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkljadmu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgkxspcl.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrynuaec.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyfxhuqc.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfwmrzcna.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gthzuqgbw.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/grszogjcr.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzliluoz.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuuzjyuv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gzorvzqun.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gxftxluku.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaniyrbw.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gfurusegt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyketkhgw.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/goaqnhjrp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gloqgrfuy.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwoazyhr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfdspfr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/grarlizvw.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gezpwaobz.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsytqjrt.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gjmdpxgsx.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gkwxavugy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gbqmksbrz.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gstodveyh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwoxnsan.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvlypsu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxrzysdo.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/geosjiras.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaywcsuf.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gepeaseqb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhadyptb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsvjcatz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/ggmkaihrh.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/guibbptru.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gskoxwvgz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkewlznkm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilzcjhuq.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gaphifiot.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbifpqav.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/giggwgute.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/guxzntmcr.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gtcfirgij.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdtlzwx.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gjimvzhwb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/guskerttg.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncnardsp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhbhejas.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjeajuu.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvithdio.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gclxdeuon.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbvqngqz.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwztqpmqy.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxaolasv.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/giberrmct.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gcmydzejn.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gtysjihlt.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzunyvqar.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhtgywsj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfijgvezh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaruaxeh.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnestjxg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcfvagmn.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/givsmylce.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkpymgst.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/ghwzxhjfl.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gebeznwwg.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ghjdxaazu.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvifnfssy.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlgbhkfh.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gawvfifhy.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/grtstdjwi.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjopplpr.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gsyynvaap.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/grcfuzhld.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbpqljvs.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gvxhjdlqu.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/giueywpre.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlqgvwgx.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgrbrmbe.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gexzcgqgi.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gimizltif.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gevxogpvu.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwtmznrh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwtoylmx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqviwhvb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpjedjoo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/givxjtyob.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gpsqeqvof.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gfcagukeq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzbntfmj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gvltvmwcs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/guymffdwo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/guoucudnk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwynyroz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghryfivds.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqckijqo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gopuooajw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gbppsvekk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqaifcrk.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gndndjawn.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzvmmawq.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/ggcetpypf.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/grzhwtzmn.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gwnjdbvwt.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnazlpqf.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpklaoymr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmezutcz.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbtzfhvo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoeqrfmd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmszjui.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gmyqvvlut.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gbqhtanlb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girtyldow.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gasmirdsn.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gidgbcjak.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glgggzeko.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwfuqpvp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gzmxpdfxp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grnxaawae.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagmsfzhp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/ggrkotvkq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkheuteu.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gewndgfda.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gvpwtqhhk.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdeihznh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmghwvi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gsenqsvhh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gigjsvffj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gamkoupql.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnqxqnzf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpnelsvt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjwsrvwi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gnlpftqem.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/ghjxnzven.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gplnsafwx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gaqgbrhjl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhnvlgfb.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlcqqczl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwjwnrr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcdqjzxx.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gesraaysy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/getwafkjh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlejyycb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkdnxyulv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxrxvaouw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjnvkudil.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcckcxenl.sHtML


<!-- 参考信息 -->