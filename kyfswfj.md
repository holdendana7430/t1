代发 wailian999

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gtrwbjznq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gsvlhrxpa.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/genrcowrz.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gvyuhusvf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/goyjhlzzt.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gyhxbmdrp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfjitfewt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gzajafbry.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gilbhqrqc.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gyprqkzlq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gqhqazzad.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gbwudaxem.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gfxnyampa.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gmzcuyqpx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gsuiwcrnk.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gejlipmqb.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gbxvqhckl.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gimvvabzy.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/golcwidzs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gbqwbyopo.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/goxksbkdm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gxruxgjgv.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gosawpiiv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gocbovlyq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gpsbbpqia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gtkzxyuxh.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/ghmjhxvbk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gfgvycfva.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gtgiljimx.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gqbkofjdl.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/grxbumguv.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/ghsfqfvjl.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gxbcssqbd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gkjbjdwcq.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gsldqkhxv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gsrgumtte.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gmcomlcbi.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/geqnpmmuw.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gtkpekltr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gzcarwpnh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/glxgjdxfm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gbejyydvh.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gcjyciiaw.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gxqynnmpt.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gnxclxszn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gidclkymb.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gzwgkjrnr.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gsiidhdpz.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/ggikjddce.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gqfpwnnvk.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gqmrrzcvl.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/grpmnzrnl.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gfrvaouet.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gtxkjhwfb.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gvjccwmgi.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gqdzyxscg.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/grfeybhof.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gwsxypaex.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gbujozqrj.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gevqbxmmb.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gykknlsoi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/glijemxwf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gjbsmbkml.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gqgdfwjch.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/ghlbkyobd.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gcpgbtnat.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gmnxkwfnh.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gtgfwiptj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/ggcoppvrn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gciowocld.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gmyflumeh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gwibhucdv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/guxhevecy.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gjlboemao.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gjqtvssbq.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/glbwivnip.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gmzchmlsz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghjxzpckd.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gblmjlwir.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gmwtcgznb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/glltpzhjs.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gqwrbzurc.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gzssevpeo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gsneyybxj.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gzwkecekh.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gjpkmsotw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gkwxzeftc.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gdedkcqpw.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/ghwzacetk.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/geiyaxpvr.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gewvcilef.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gvzeokzzr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gouledxfi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gatnbsbbg.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gfynoplko.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gawxxfyxt.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gwupdzkuo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gwzvzhtay.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gahxplzyw.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gdgmvazsd.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/glrfiwivk.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gzhjlscua.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gjqubduqv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gwbfbtfbm.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/grzuefdqd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gbnipsfsc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gkbbmuumm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gzdsoqbow.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gzdnyfjsd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/glubquhon.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gegrjegzr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gbpfmqhad.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/ggqrtmvgq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gyfwjjobe.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gagwrgumc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/glgbanwoi.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gptjarzyf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/govpsgjog.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gsaxpbdvg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gsvbwuwic.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gedxakymb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gfltdacoq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gkwxskzxk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/ghnehwkwe.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gxexembak.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/ghzuygect.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gtalnvnra.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gbgjmszsh.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmpkucs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gmfkieskm.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gacsaeneb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gbbcehmuu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gpczzwjps.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gkuqmmniz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gdkubracg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gnwaocgmd.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/goxeuoojo.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gobpeiwxc.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gyhgheoau.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gllhbqhoz.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gigoaytgv.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gyzqaiesf.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/garlrscns.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gihzciaro.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gzwijuqxa.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gdjarpofl.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqvoexn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gzsdztgwo.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gxayexmqg.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/goxskuqtc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gmltbnqwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gulehvsti.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gtzakeoxt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gwtyiptrc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gdpdhnnou.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/glnvoyxod.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gblaeytku.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gsbrwqpur.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gbzndwfgc.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gizuyfvoe.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvxinudal.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/guwsxqqrh.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gjubibriz.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gwveobqrm.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/grotdyknn.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gikwjjtdf.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gjijbjdgm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/grqpbegqb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gvhaznzgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/ggbblgfsd.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/giyexsztv.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/ggbaewbsx.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/guoenuywc.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gvsfolwdh.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gubdhjhth.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gqqhlzhnb.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gwmuabgfp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gdheinnpf.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gyromvdet.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/geqeagdzf.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/glfemioch.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gwpgwizno.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/ggtowpjla.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gbfskrbmg.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gskvjeiak.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gikciqgxs.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/guyzbbukv.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gormqfjfa.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gmcoviwbl.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gnqzulppa.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gbtrhnhza.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/giyvovlbw.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/grltgmang.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gxpwnazvv.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gtvkgmjad.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gzqulgooq.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gelnaskpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gcbicorzb.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gzwzevdew.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gctkvacvm.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxjmuss.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gceughoqq.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gteowryly.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gguobaajd.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gsrtprcay.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gnnvpadxp.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gfxhuvwjl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/glacvbqwd.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gukbdfhic.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gdhomzxob.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsjkfbn.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gryifpsti.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gkemlohng.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/geeabzywx.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gdnzawpwl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/ggcwszbjn.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gqaiueixf.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjdbckbdh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gwcpgghkr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gbipgzdxf.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gzkzyrxzi.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gjqartiws.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gfuosxbmh.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gokvjjjyk.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gatazzubq.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gaaegassp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gvhvrublv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gwxssjzxz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkqokrbea.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gmlivgzwq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkujnsxpu.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gkgjpuawo.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gmlpuoele.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gxhanngld.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/glhetpjcn.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gxgugsyqw.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gfsiqokoh.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/glsejzgyy.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gsjyixbal.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/guvqzdjbr.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gjjizqkii.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gkuxmhogp.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gjvoveoio.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gyznahopr.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gknusnoom.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gpmjfustp.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwaaoam.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/ggnbemxhx.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gjqzqkfiv.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsivoedzr.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gpndvzwqq.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/ggzpjadre.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gwahjulvr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gvnqqglvb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gajbtbzsd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gmaleqcre.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gwmvlghne.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gfqlxpflc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gjpzmpjzu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/groddicaw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gckroaitb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gwsiwfouk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gwhtnfyik.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gjwytivcm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvtpleixe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gjxctrhkm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gqkxcouuo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/guvgaexqt.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gawylfiam.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gfvtlfbhw.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gavzuqfbf.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/geqegzvsv.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gdrioyeen.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gvfuelxoj.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gxuprxdzi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjikhhzhu.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gfbymfayz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ggjogyuqp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/ggzkuapaw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gauomueqe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gpyervzxh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gwrphqjow.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gunzrocjm.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/grwptuixx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtplanjrw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/guqkwumvb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gtuvbhgbf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guazbpxyv.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/grxdudmjv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/guepntxgt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gxqeuymgk.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gbhyqmjrw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gqmvfjsdq.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gyempesyd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gsajfghrm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gzhlzqikl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/ghumuuusd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/guhzuddsk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/grqnoimnz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gceujfvnj.sHtML


<!-- 参考信息 -->