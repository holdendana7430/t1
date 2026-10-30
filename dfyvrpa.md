代发 wailian999

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gqfchfkcr.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwxgmlnu.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmaauvvjp.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gupcitnxc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadwevakh.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gczppmans.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvmmohgi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqchvcahe.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/grmmfvmro.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigisnujx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmcsbcgn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/glsnxubxd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gllsnhjfc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gygfuaupl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyyslqgn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvqytsxs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gqesmdqmj.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcoruumm.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlxvbokl.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysldtvim.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gftwvfnxw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gdalxrzsk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghppvzpcx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmujdosn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlrqmxgk.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gunteuuhh.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gvnbqjgxq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtosorzsa.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuhctuqm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gajyirotn.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gcylhhejx.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnewcxor.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gpmvylxqc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gebhkrimd.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggesnzfjs.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gopswrfvz.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxpaqgxh.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gijeqmdcy.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gcospjcyg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahsmyhey.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtlmbhu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/ginofobns.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsgsvlnp.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gqgpasmue.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlopfgak.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glofmienc.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeocizkp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkzefkmf.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gvvnoyvbe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprasqptp.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gahsjungw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwvzlgy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkoppmyb.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/giiqqwfdr.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtaejmcf.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gibbdyqsp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/geoshmanb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gsohrspyg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjgxipcq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gotmeiupm.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwjevbrz.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/goepfrllf.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/guuaglqlb.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/grirzdbzc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpmrmjwlh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaeuditso.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giemzcuzh.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gmtmmtjbc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grltaagzb.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gyprauvjo.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gvcvhxhwt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaobgvufx.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gnsflyvzd.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejitstkz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsoyxjia.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gouldgluk.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gaxlsywvb.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjvennsd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrfnbfbn.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gogbuaphu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhxpabd.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gkkfzigfv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpllrxgdf.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gktyrmgeu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gypenkpjy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlfjpuao.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcidxxqjg.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxuavjcs.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gebuwpdem.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebvtxlsy.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gbemihecq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpsesmhu.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjxqrcbni.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghiapoltj.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/ggnvrvuqc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gjqtchabl.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gtcdfmitx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfwcymh.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/glrkintoi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsvgqvuo.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzdslqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxkdyzpi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzocovl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjazkgmo.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/geodfmtap.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjfokgpy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/glboozhps.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxucbsm.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzeymxzm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/grdpxklnu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gvrueiiec.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/grvewltxe.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gkkssvirz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gnefmteyx.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gziduzsiu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyihiize.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeuwtjfp.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gxxfffkba.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/ggwbbdlne.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gruapgggj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gljmufwyt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpmxybuk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuiknwmx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gacwzgasy.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/guazkotpd.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgxoxunr.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gymwvwtqq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gtqadbxen.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gxeehukoi.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goplxjepe.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gkkdcezuh.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/guwaazzdd.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbdbhhjv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdmtyhga.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgcrjgdv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpyyuezo.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/giexfqivl.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gupkssopc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkneqfxku.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqsngqdot.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/grebwsrsf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtmydmxd.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gjdwrndpd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/glhqdqqem.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhlgexul.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gtrvshqex.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gfirtiuuq.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gsclhswva.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/giayrvdcu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gxqbtcpdr.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gesxcvhuk.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gndscxwkx.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdiedfk.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gomulvfna.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geevzmbvr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/glewzvgun.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gammgtjsy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdzstjbc.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gjaullrmu.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmzbhqzu.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnmsnvzd.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/ginsqpfma.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzfpgosvp.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhngoti.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/giszdweqa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtxxmxkw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqunssmf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjipblsid.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/godhazaqc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gkcxvujin.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/geoupwyfv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/giiocvqot.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmmugxem.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnuwzzrd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpmwqwpx.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehvyqny.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gbknaxquj.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gttbxtawx.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/giheseetl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gwhdiddky.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzlyvuxn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikceqbow.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gydaucxmx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/giyxbjqfp.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gllqdmuuv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/giuvykfwb.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gguhsijfw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gntbfpjzw.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gesvtqbal.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gjbsnocgm.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gxorlcich.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/guczawmlm.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gpaokkfqn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/ggyorfnpe.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwogxarxk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gcgfpghzn.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/ggjqmttpv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnlfszah.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoojwkbz.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gpewzqdlj.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gxwvwklju.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgtvpgjr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzcrbeejb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfxjssyc.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gailxihwo.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gffxuicxr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gtidmgact.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfssxsnwb.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gxdqpugqe.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofqyonxu.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimnqksg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqxnmanv.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxbpxggo.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuwghaeg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhkgjiix.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbrasufd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfioatrav.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gienqfcwe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbofwfka.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgtpuzkq.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gueoqhthr.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/guukfrrio.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxogockg.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gptoglwvw.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gaxsebttl.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcpabrer.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmrlimzwd.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gasiddlnw.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/glaywklft.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeboramq.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/ghwitezfd.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gthoeiuca.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/guwuiebdu.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/glhxnbhyy.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gwllemsbh.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhludznu.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfjphtea.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnenavhd.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/genrdnpsp.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gerbsaahj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/giemwtuso.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegrgtxcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggwudtlgv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/guhgudquj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gcreuboin.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/grtkvaaio.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/glggnkovi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gvitnowov.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gztxcmjhd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gbufjdzww.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/glrlztbcm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gacmvnizc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspaziznz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gpkqgwhvb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaulwyyp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfjosrko.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/glchxvial.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutxoczgm.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gdthgbxxa.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gasvgwvig.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gwifexvuv.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gqktgoqti.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwcryxv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxpmfbdn.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gkglgrynb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpvmwqzh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gplpqroxe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhixvyyp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gqmcgdcrl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjfodplv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gzbinjcer.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gziadklob.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmergeqmw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjesjirss.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/goszphkkf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhohshvo.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gkqeuoxso.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gfkjcnxpt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdhhiuri.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/ganhocazc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gywcdbepa.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/ghnfhsbxi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/grbozroug.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gilzchvhq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocgefpc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/guyfotafx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/guracfnwv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gcollakwe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrdsxrca.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/gvntreukd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gigsbgjcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubaobjcv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzmjbtky.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gmbtunymd.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gthtjyaxw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gungqunbz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdzdskwk.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcgrdcgq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbampvmrb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grwmzawzt.sHtML


<!-- 参考信息 -->