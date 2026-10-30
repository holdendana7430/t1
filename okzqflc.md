代发 wailian999

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdzjrall.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/giyrvbmtu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpktarmnb.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjwyomvm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/grcaupshq.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfkoobpg.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvilljgj.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbocpateb.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfuqgoso.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gltevxlmo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjzuzrat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gwbgspmsq.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrgjfky.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gotqgtjsv.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvlmkjis.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzfuqlgn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gptdgvxoq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfwucifbl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoquzgsn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzprftmwx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwjfxas.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gqnvxdcqg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/globhognt.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gnhbgslzr.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjijcyjfn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gwduuzsjw.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gvtbuecqy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwzpvraj.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiqkrphz.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopzerrv.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdumoemp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevlubmrv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzccpcwn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gmnufgwfq.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbcidwwi.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gydbswjba.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gzkirddtr.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gabrmsxer.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/ghmnlhblt.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gaiavdfvl.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrybqov.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbepffkp.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnmdfpey.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gyehivkjk.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhnasjuz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcpgtua.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gpqhdaxdw.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvhqoxew.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gckwwhxlr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuxnwczn.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcngqwbdc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gucvxbodu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmxfddqr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjkjgdq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/grduyfynq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gncmcurbo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gdntlydsh.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaamfcxji.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpligpiq.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyhryjvuj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlvkfxll.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gstxvjthd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gowuytfaf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gprzmgbfy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqobzadz.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfaovyrk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypraugiy.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gvesnltkp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjbeplaa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvexwftxa.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzegdjnrg.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhtolewt.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gekcsozkq.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/ggdateqak.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbrlshvk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfcilzowm.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/goewswtxd.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gquothifu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/glijubzkw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbvythes.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsgbziqt.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuymcqjz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqmrqxd.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoojkccd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gujmzspxk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gqrekrnbp.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrresjnl.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/graaidbap.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoeyptcv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkgunmva.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyanrkqpr.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzuszibag.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfukvulto.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggduvuadz.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvkxifih.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghbwhmour.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/goiiateie.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gljkkyshe.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/giiqmudmv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzvdpkls.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmoxzmwe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtxtpesi.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/girvkajcb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwjperal.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwvmbuys.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gytxcjder.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwejgutq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmijrummh.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/goilxwnpi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxnhgbhwn.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gsgcsfpep.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmacfjgk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gjswhpwhw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpndknqgc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/grzagywbe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gjhcbjhag.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwrnylfhn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gpbuigdzf.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbznyjzhl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfockmtem.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcnhtnnb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszpxwtd.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcocuoawu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsoousei.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gocvdriwp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwumpvtiw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmdyyurj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvovwsa.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gbiioajve.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjgpaari.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/ghgvhhdsn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkqtpzfw.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgyyjumv.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaclyndg.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamsugwm.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gqyilknez.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlihumir.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gidoyhctl.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gavekcppp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/guuxqajra.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/giiywhmra.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfrxbtyg.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbahkmp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpyqsefb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwazhifjy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnxulcra.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gfglzqsbk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwymixa.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/ggbylxfpc.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpyzjqkr.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gordllrdb.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gmfgrzjqi.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gstmfdhje.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/grucrrtug.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gxdxbcvfi.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpiaroqh.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gfefuwxyo.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/grwexukgd.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwcdumla.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gfdhwqbvp.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjjcshayl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gzesmjpts.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiwstgko.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxuqpxnx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawszsgat.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdoatgi.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gaoyxviww.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxinkxrrn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbzauyco.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuuomrpr.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gopszvvhd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwcpvxds.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/ghulkcubt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuveinlj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gkaxwozst.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gqokqxddh.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gjxxussum.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gsgtsbkek.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gvukseljk.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gslwsottg.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzljingzy.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwemxwa.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gasvbctyj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gvdnsvapa.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gezzgcapl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchaiyjlw.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gottjkiam.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gljanswga.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/ggkjgpesq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnnxrnas.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/giriprqwu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxubywbcu.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gkaboxnri.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqzrvewj.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwdvqikb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gcernuvkh.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gqowoppms.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwvtnvcn.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsypmuxd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gitoalubg.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwqbtnq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdfomklz.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gapzfgkla.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvrwespf.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gmkidgehx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjvhjxql.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnntbtzd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpcifqbz.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gvyccuhky.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwxhvybw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggrqgkg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gapmncjer.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gccigkztf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/grmggymrj.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gvygdljde.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gvgbhlcwe.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gxdwcmaxu.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gaepknedh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseerncse.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgxlivnt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvwjmqhlh.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gdgeuuskn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsidrqlly.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwgmirng.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/glicxsilc.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gudovixeo.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ghicaylmv.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcmupmel.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/grelaqity.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbuvqeem.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvfrzzoed.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjddnecmo.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gkodufadc.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/ggwlngwdx.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gycosivrv.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/grtbpblqk.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmetmivg.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gwegjllwt.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gleiorzck.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsjhmnlz.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gopgxfobi.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ghppqzjnl.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gnlfzvjjd.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gvswxhxcd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjqajttg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/geieoxeak.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmrzfnzd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/glaxxxjlm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gygojciwy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gdschjrdj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtaimzig.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqmxavxj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqohwpmws.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcryswge.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrqyruxl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyurmmoy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gehnszvwi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawwhsgcm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyylptf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlbgekol.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gnexlxwmd.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gilwgnlmk.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gfalkmojb.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/goonrkukk.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gobzxrbsr.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoafeyks.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnfwubvg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjtakeond.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyymllcym.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghloaimon.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzsniai.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvlwopbu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/ggdkqnvno.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhuiblzy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gtqrpbjgp.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gdyucbudf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxjbxhblc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpiyzdnj.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqlvrmzb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbhzukuwq.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotgkcmk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gmszrcqiy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gxlinxtlx.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gktultmly.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjynckta.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gnigiqswx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpekfjqu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gmuxrjtxn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlpiarvm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdinjbkc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtuzmubk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvknlztw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsipjwlzn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxifovwhf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxgebokf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gwfevpwod.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gijuhmzyn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonbianra.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gbjsyxums.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gwqpulwos.sHtML


<!-- 参考信息 -->