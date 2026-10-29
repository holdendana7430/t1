代发 wailian999

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gxdpfiopv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gaxzuhlif.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gqxnpgjoo.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/grjlqalwz.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gvwswvrsk.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gtkczbxoa.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/ghntyiqqg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gcccbwsjf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/glifnmpjd.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gsllvommm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gjrmaowye.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gfyhcdinu.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gbdpjrzqc.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gdordznky.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gabjsutjb.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gbvfrlyml.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gqxrvbuqx.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gugfcocup.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gvmlrzrtw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxmzuvzr.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gxmpasvkz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gwjwcwagd.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/goprjnhls.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/glgxknxyo.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gajmsvoqn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gbiayptgr.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gimpcbzfp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/geawlhdjv.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/ggrunound.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gfknaapkb.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gstuolquj.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gnppdrven.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gcjyvorlt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gyqxetrjs.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gvuxwjhga.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gdoormoei.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/geiuehypo.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gchogebim.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gpzqtrzfx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gsmgkyzrm.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gxqrzfgnv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gvjkpwgqv.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gcopwygju.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/ggxmqenof.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gpinsrjwd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gwvhccbfc.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/geodhvqqi.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gpqqifett.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gzablfgaz.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gqoyhskdf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gokmshqjn.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gmriwefpe.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gnrfuuppr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gdqauqxvi.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gmtieziku.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gootyzjmy.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gsaslvpnc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/ghnsdrjji.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/grsfqjlid.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/govqjxdhm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/ggaqprhyf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gwlxzmokq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gykbcasjc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gcglsutgq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/grcbywcio.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/grcwjpntp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gtixbqrtl.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gwmgzggyo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gzwlfisbr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gblpxtzik.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/goyldqojn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gcaszfjlr.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/ggmiadfyc.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gredtmzhr.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gvoglafbj.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gqgiiqpvf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gaphzyiyo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gtpvajvsw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsdnigsbq.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gzoqttjvw.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gclmgtnzl.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gpkfojhcf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwkqoghaf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gmrpdcoxf.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gtehuutki.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gkvraywbb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gtmtsgaxn.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/guewqclcx.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gjvqvvjax.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gehmooaeb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gsueqjsuu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/getxzvagn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gifgrrlmw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gczfaxcuq.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gfiblrgwx.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gsogsvfof.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/glsdmvvdj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/ghfuyybyj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqzocts.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gunozjave.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gcbluxkuk.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/grjnadzkz.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/guumbuktd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/grhcjqnns.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/godxwfowt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gnmkjftwh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/geouuhglw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/guijesbep.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/glgvipkju.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gifpithkk.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gwthxtcxm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/giyrseura.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gjffvafpv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gbnxpkhnx.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gdicpvzzz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/ghjgsyyat.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gfrpdwkjn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gjtxhvwax.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gskkdbwqn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gncchsjlk.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/geibclfkd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gbcqkxemc.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gngtobrst.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gjdvcnzdk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gkzjbalae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/ggziacxxf.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gzahfytpl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gccvictdl.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/grwecvtul.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gcxlwdwwg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gpnebwplf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gjvzdlgqa.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gtgapepev.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/giovkvyym.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkjcssiuu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gzrubvhtw.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gixraqjat.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gmjnbferg.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxfwdlq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gbytelxbh.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gmxylhchq.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gxcvfsvxw.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gaekokoom.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gmiehljnu.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gxrfzolub.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gbldebpfu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gdnsxjglk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gpekxjeyl.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/goffbcaha.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/geyfvdiiz.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gqqiywgxg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gegvpywbe.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/glxarcolg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gghbzsnro.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gwzyoipad.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gvaybqmvs.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ggtjuxxcj.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gqaqrxofu.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gfgzbzilk.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gixjjhpoq.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gvjfcljft.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gjkyrgtfw.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gfbwoskid.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gghldzzxi.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gbxlaiudl.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gyagjvnio.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gfaozhecr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcxzjsxpo.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gicxjwtlq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gzyjrpbzv.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gyinzztjv.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gfgytlykw.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gyayvfahg.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gyzzmyqxf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/geyaalgjj.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gfrocebvd.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gaxbtzavj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gacibqibi.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/godgzqvwq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gqpzxbzbj.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gouyucmmc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gcenrzaji.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gkyklbavm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gpdggdfng.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gehisizco.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/glqlkevec.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gngqxhbog.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gpokgscdj.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gdxqmwwnf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gifejvnsu.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gwmvvwrcn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gajjoxqzn.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gnxijeelb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gtrdstcqv.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/geqvmkftn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gndlqboms.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/ggikrsyos.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gaccyfcvt.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gxtjjqmgw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gxaerhyro.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/glikshjxo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gjxregynr.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/glesfovrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gfaztrxgn.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gabvguqvb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gycfxudcd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gnvdijtvu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gsiaudzpj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/giyzcndjv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gpmpfqbuj.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gjuveegjk.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcljujuce.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gjutdmeue.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxdvbsosz.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gzhuslndo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gumhnnzls.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gtngrbbfo.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/guhyvsrpj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gzcmvtalb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gbpotynls.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gtrdxxgbt.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gjcvspkct.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/girharjlx.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gxdcjpykw.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gpavxnnpq.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/grktughjd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/grjodsizj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/ggzzigjbo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxeyegcld.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gmmvdjeqb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsajiyexe.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gtsdngavh.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gsnqicuzs.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gkmsedgmy.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/glewaacpb.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/grrqmgird.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gjljqbhyq.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/govqteayd.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gsdyjzgku.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gowyqekoe.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gssscllln.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gwbhyabvo.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gntyffdvv.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gkdktcstf.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gqfefsjoe.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gamyppvrg.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gcvtsrqpk.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gxlfzclio.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ghydtlakg.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggymeemak.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gtbanldkw.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gpltdvrzo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gtnoerefp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/grtgbusbs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gforcsvmf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/guqljgdmi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gcedizbhr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gayhxhjmy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gbafwylyh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gpbxmdciy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggyoqwryf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gzayspypf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gsdcippiy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gflsjqonb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gksmisfst.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gfwaobtzg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gtsnicjvg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggckykmqx.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gzrtexzqm.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gdvwmqvln.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gwsxpqbyj.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gwrjcioox.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gyvrefabt.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvptzoceh.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gpbieswyh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/glvhlsqfz.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/ghtgebmbf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvsdqqsaa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gmwwvvsul.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gbolcuale.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/giqgailok.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gqwgimucm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/ghrdfsekl.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gwnozvpxj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gatepnhkz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gaofmypzs.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gehjqbfuz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gllyclupg.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gfrnazvev.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gxkkbodus.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/geznsqtrg.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/guonnbgaj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gnslrzlyi.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gaotesmtd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gcrcyebjn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/goceuprjt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gffdkrheu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/grzcoenrd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gexbnkfil.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gvxhtanxm.sHtML


<!-- 参考信息 -->