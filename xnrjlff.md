代发 wailian999

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gfqrdvtjn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gpqpjybed.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gvvcgairk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gcveeomsf.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gctxosbxy.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gdbjkjbep.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gzhlniwsh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/grbfdbndh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gopdwsfld.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqvjmadaz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gacjladiq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxpsmvlpg.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/guhxyyyam.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gyfaxpjmw.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gjagcdxob.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gwpfynifm.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gricddraq.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gnlbjblss.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/grevcznht.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gcjfuwzjw.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gqzyygzfx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/ggjxgskia.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gwdhlebbt.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gpcbbxnbb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gnnskgtew.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/grghpweoe.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gwkkrxeio.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gjsgfujvc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gtenfqbto.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gnhefchmf.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gqaknsgnk.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gnldtjvry.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/giakdoiyd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gntddgsgn.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gbnvntntu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzoauqhhv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/googkmqds.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gtutwtqsm.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gghlcrfsw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjcxdce.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/grbszppqp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gkiezpthf.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/goidcrfji.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gjufiipdc.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/guptrjmej.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/ggdffeeeb.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gokiwblwl.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gvavqxsdl.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gwvstvxwg.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gpgjjxhfq.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/glemfegfk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gsinhdyed.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfrfzvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gbgautgfx.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gznqtdwqb.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gqyyucadc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gxxfsndzr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/ggokswazq.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gmcibyjcp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gvqxcwhln.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gbypeumud.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gmvoopeec.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/ghnpwiish.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gxyhbxzst.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gilbtbmxd.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/glqnmbkes.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gclgvkdil.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gcmufmpnr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gcfllkcir.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gnaoschrt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gdtirstdf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gfremvsmf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gkrqczyil.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gkritbwyd.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gqokbxzpp.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gozamqoox.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/ghpswajdg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gqdtwzpct.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gyuoalvfs.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gccxzsvit.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gflypvdfr.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gbztzywnv.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/grizfstgw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gjtfxainl.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gulnxswaa.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gicfcftnc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gsepjkjrc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gasyfbhvi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gzapkwkdn.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gydjkcimo.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gqfatceul.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gxrrtifau.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gkcxyeggx.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gkmwarzjz.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gojkdguea.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gcujmqvek.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/ggimfnhwa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gisjtavto.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gtarlssba.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gaaoysrua.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/grzhtmsxw.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gnrsixlht.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gbvywnroe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gqrzzroas.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gkdswzmow.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/grnxidbfh.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gnqfjrjhy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gelokzanp.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gbqbnhlfr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gyqsisnnf.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gaonblkvq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gdeebjqgb.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gpvuxiioa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gxwdgelnu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggwmsdkpd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gvyizqtvz.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gwzrwolpz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwonsmcdh.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gewugamhf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gafgglndd.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gukglmteq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gfdccedqq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gdmulrzbe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gziuuouku.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/glhibtese.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gzirbyzyd.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gvrqdjzrt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gnxtkdgsd.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gmvsjxdfj.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/giwfexftw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gpkbkcplg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gtiesgxro.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gnlyvrrng.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/grmwfdifu.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gdnvutvor.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/geeeehyyj.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/ghfpdzusu.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gugxlboij.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/glgsxmkmx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/glshprqst.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gyoeqycyz.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gebsxttyf.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gziazmuvj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/guuygwwsw.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gczuwikbs.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gtmkojkex.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gfprfghtc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gkwzrxfij.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/ggstxgdnd.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gzpsbblnq.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gvdukyihf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gjumfzbib.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gaunddbsn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gldnardtj.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gqcayuezd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gpnvhinqh.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/glhvtjtgf.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gljomsrpb.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gpucrxjow.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gatempwzt.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gdcqggqlp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/ggekdxoki.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gvbleqttl.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gqqjunyjm.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/ghakfxqrq.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gpsgddjuv.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/guawkwqou.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gdlweehbv.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvjhfofsk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/genywbpak.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnlviadtg.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gyozusyzf.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/guhrlwacj.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gukjelzau.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/ggrauioue.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/goozjnqsh.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/glwfjlbrs.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gsmdgqnab.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gfbxfpgvh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gkwatkkix.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gzdxmsgfd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gokdljkkp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gaegjdzfu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gncaiwhcf.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gzmubskim.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gctxrtnrs.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gxbbqzoop.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gpyjqxnmc.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gfrkiejsq.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gjwktkuqx.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gjnpechvl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gvevwsxek.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/ghndemxld.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gzvahrtsd.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gzxpbdabv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gxietqsml.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gsgljfppm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gypsceoaw.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gzgeeohwo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/ggsigzzbr.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqvkfncuk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gvhclbbut.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gcfkqsxrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gqlnvdznh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/guvdatvkw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gghhbador.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gwjegzlqw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gfgyzemwe.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gqnistlam.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/glzwmltzz.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gplzkqhjj.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ghfpxkeox.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gnsvgpfrm.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guxzbpgwo.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gkhwiupfn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gllycfwof.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gqgrjdcti.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjsmpkwky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gblpljrxc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gimjcomyy.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/guzynbcua.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gwiaoodze.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gutoexjlb.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gxzbcsvvd.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gdvvvddxc.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gdlcbmfmk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gflavizbn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gpwgfvtqi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkkmmwfft.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gchlldyuq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glmaqcpud.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gfncjcaji.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gfyaupkis.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvttzdu.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gvcgqaalr.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gxndxepnm.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gzeehcfzo.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gygiulsel.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gvwceahwt.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gqvzysnvv.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gglxcopqe.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/ggeechnyw.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gduicwqcv.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gvhcvyody.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gmfwpwmuu.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gidukjrns.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/govmufghe.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gdnaggkav.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/grtczerkv.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvyieuynj.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gkplmiura.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gebqsutjn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gyafajdqa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/ggutewuhb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gxdefzcxb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gxyelfrix.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gpndxafzc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gzgxorbwx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/grkfrzdgg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gluasucbv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gzcqecsnl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gprtyynrn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gkilsigii.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gmpvrwyqo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/guqqikoks.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gnwijcsls.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/ghczsioro.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/govrgyhrm.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gfjhusebe.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ggslghqih.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gqqjfrnjo.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/geoeikbpu.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/goatencvw.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggrvldozy.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gxhxostyq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gonnuqtun.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gvqevckmj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gcgzckipr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gkgxtyowi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gxgbpcoxf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gntcsyjta.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gqygrrxaj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gecrkjzst.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/grfeccktp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmygwbwcl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gpstlnufh.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gbknoghlo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsavmufxi.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gigqenemz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gaqnzikzi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gqhxotnnh.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gznzgxmht.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gelcefgcy.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gwxpzribz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/grpnfzgjl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gjgdftsla.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gdzwqohzq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gxladtvep.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gfwcdwhpi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/grmbrvrez.sHtML


<!-- 参考信息 -->