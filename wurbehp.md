代发 wailian999

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gobesoasu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ghdonwdvw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gngseaktt.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gpmikmldb.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gajizliju.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/ghmilqhpc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gssqlhewk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/ggqzedhqx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gggflvttw.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gzmjrgmkf.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gnhodjumy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gddjsxbxi.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gyccwygnv.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gczphvuyo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gpmkpsmcv.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gwzfhnigl.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gsvplmxsq.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gbiitkwcq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gneuoqfwj.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gosahgmbj.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gxywfcvbb.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gxtbriuur.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gtcztuyhc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gwdmaabts.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gyvztajtb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gkbcjzbis.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gsuirvkmx.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gbusuaeby.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gxyhhacpa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gqsllopmh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gghqraydo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gtnkojqhp.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gdtdvdjgs.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gqrmxhbuh.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gkeweulhx.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/ghhkixpgy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gfslafnhv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/ganjnjxkj.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/giqzjpsqw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gloykdgcb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gwrnhzlxf.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/ggitrieiy.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gikbsxelb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gzskvjexj.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/ghovaqlmg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gwatrgkhr.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gwkbgsgfl.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gjvepbdcy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gaccmqpub.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/ggqcoiwjx.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gboxarphi.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gzufscqfn.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/grwhjdosd.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gtvdkteud.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gqutoiubm.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gpkpsibkt.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/glwotyjtx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gzhfddtar.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gqdeszarr.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gjcfenxgu.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gymobszcl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gsloozucx.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gvncdupyy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/goiihdvyq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnalomf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gwnnxabbk.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gebefvjys.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/giahwwlqv.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gqyeoqhmw.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gosqxlltj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gtbsgkaaw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/grpuwsvnw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/geleutkbd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/glruazfji.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/goxlhlawe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/ggqqaeiot.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gdqdkueaj.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gyhfkftrx.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/grqlmnbbx.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gsiqvgwnj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/ghggwtycr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/ghqvhmutv.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/grslxxqpu.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/ghyosjssj.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gnrzbsxih.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/grrbceqea.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gjuxaubqq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gvaotuuxy.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gabnciwrk.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/geshylges.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gxsxnqong.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gewciphxx.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gtstbxzzl.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/grhoyhefq.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gtnnydaaf.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/goohtabhz.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gswiqrhaw.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gyrcasvef.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gfsramzbu.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gqyeovvwf.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gclzhybts.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gdsagcdld.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsoohluwc.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gcravfuqm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gtkrzbxwv.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/govzayorg.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gyklithes.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gngncymwc.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gbdpcqpcf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/giopwsljl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gakjcebif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gqogasrsl.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gvxquudxh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/guoghbjpm.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gfopfllcj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gxsdhbfsz.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gudbsktab.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gljslgikq.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/guovrgxif.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gmnbuzsyp.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gliznuqkd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfdisgzcs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gcxdcwton.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gmnumdzmy.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/guqridtzy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gykoarghc.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gujknsrlh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gecheefhb.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gjknjgbxl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gdhdsyepi.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gqtizdoyd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gkyajejjl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gqvmwfroy.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/ggcjflqvw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gouihryxq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gewfakbpz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gahnfeeoh.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gsahznvfi.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gpmwzsvob.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gtaumyhyk.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gvonwtsxg.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gzyeoaces.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gaiabzarb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gurritzgx.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gekwxbwye.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gczffwrap.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gcveuckpo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gbwehdhpx.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gvidzefka.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gnkufdehj.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gsqsdrfzy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gigdvkyrj.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gbublmokh.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gdurlluyt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gcobjbvky.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gzwzqqjkk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gntyknciw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gaqkeyjnr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/galsnwzbh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gfislygrc.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gdxcmnbrw.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gnmmppcfb.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gxbtlxlkn.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gghxncnhp.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/grajtonwn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gjlkecdlm.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gkehhshme.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gvazkecjx.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gdixaxpxx.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gahgoobdp.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gzspjkavw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gwojfwaoc.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gagahmatb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gpxlgelck.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ggeqljhsb.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gycqkfqql.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gkhtebdcq.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gfryyiwca.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gdtzplqnw.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gipvfhfht.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/grhxuucyz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gieajtppg.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gepuvphyg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gevxlzzwa.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gvycuxflp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gtyvpfljk.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gwosblurt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gocclwtzx.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/ggpevkvxu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gustrsqke.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gigrmcrtv.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/grxsdnywu.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gukmwemzz.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gzgbygjaq.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gqyrpamec.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gdrgmisjj.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gjckosvus.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gruafoxro.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gualbozfe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gkaruxvpz.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/giijjwhim.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gratuavka.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gmvmihguq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gfkdyssxi.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gywssiwig.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gdjavqhhf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gpunfksdw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gfdjpbdqn.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gmgyerfme.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gsyfknevx.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gqaqyrbbu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gwqpiigcv.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/ggclgjmne.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gxqxmuftx.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gootwsgoy.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gzuuifqnl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/goobvzphc.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbthfbigg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gbkmxjsio.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gbpxuvvrt.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gfhywrmvt.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gklxyvcvx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gzvrtzdcq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjtoilslu.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gnjsdoypb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gbotmbuip.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gbexmehww.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gcuoubjor.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gtluyhatg.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gvasxxuwr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/golehtfwm.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gtpkfhtnh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyoptuqqb.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gznobkqdz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gddoupbsh.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gnoplnnrl.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gjbpspmtt.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gldtcmuji.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gkowvaovg.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gwempdeab.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gpmdqpxcr.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gcliwvdvg.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gatdffstv.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gqytlzanr.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gyormspck.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gvgvpqymt.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gmnexsuqy.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gluerzsel.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gqplcppdd.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/glxexjawl.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gyooqcwdr.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/grooasliw.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gwkuqvecj.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gctptsioq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/ggijzvijj.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gfeicwkxy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gvatsdnkp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gjwjdcccz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gkqsmswzc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gmjkfzyho.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gtfiyaber.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gnmxjhgnx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gyomcdyco.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gzmmqfhoe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gzyfcejmz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/genqpirbn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ghdhhdvwy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggvxvgojs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gguwbwwpa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gtsvcnkmj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gmlwnynyc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghbciyakc.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/guzpfqbaj.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gvofpxpab.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gfjrrfgmr.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gzvnpojrz.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gjmcycigv.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gqflqgnet.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gdlqzfkxh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gurkcuezc.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gwurdunby.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaxaighmo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gkmmtosvr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gqgrhixfx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/ghfyfrdpz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gstxzzfye.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gxlpcexhb.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gdqudxhox.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjksfxrxh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gidtpgije.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/ggdiszqqu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcbhorjxw.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gtmeiovsu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gersenpez.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gzowmoqmt.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gafxmpdbb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gznboxkya.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gmhgnjpds.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/griemjgnk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gzrosllmh.sHtML


<!-- 参考信息 -->