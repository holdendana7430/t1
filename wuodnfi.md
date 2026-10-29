代发 wailian999

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/ggoibcywh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gmcomcdan.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gfagmqlev.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gmyxbqeri.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/ghnqazsuz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/ghnkvwtyy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gqayqsuef.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ggaclqhci.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gxehfwzbo.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gycedymvo.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gxpnxqapg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gtmichqsa.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gokdfqoju.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gieugbaqt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gxryzevhu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gkbkptggv.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/glorskgao.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gzallrltf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/grfkzcszt.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gtbxhlynd.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gzummzgmi.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gggkgzjxg.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gzbcqsfxe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gifzaanoq.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/giitrkfjz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/giycklykl.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gdkznkkmw.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gahfoaxzk.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gndnlksqn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gmtwtgsgm.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/ghcpjeynz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gpgpqitqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gfyhdpnxu.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gvybvmhzj.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gmevxdjyj.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gukdpibmx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gyzaqhmem.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gmdeqfqtb.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gwjmpnjri.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gdvggbqmx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gcftbvkvi.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gwmpaujel.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gliclauus.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gpjqwdsch.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gzmvehmdn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gqyqtmscg.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gridotoit.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/ggmgaolls.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gwiojwbik.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gymupufxq.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gwjajzgmi.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gpuoqieml.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gkigkgvsc.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gngczonda.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwwepseia.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gjwgmbzbe.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gkwlmghff.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gtgmwktke.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gakqibuxq.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gvdoniwef.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gksagwqyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/ggxdabyiy.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gcwvfihxf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gltnuuzqj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gefowvfmq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/geqfrfoxy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gyapkigwi.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/ghygqhfji.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gqilpccwo.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/guaudbkct.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gjfpzfjzd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gqcudnniq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/glyloytxc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gbziyeuvh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gbtszxknt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gldnguhnu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gordhsfev.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/grpltvbpp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/ghkvlevcx.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gxzwrsdlr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gyijoaujz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdphvpnly.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gobekxhhl.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/ghrscmtiv.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gvggjpbpo.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gmxwdjidh.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/glnfpckca.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/galhmaqby.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gnowiomtp.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gvoceksgb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/ggonuuxzv.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gyxjxrjob.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gqjhjhstr.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/genttshzd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gwxrrrssz.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/glolxshrs.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gskalytxh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/ggmhnyyuz.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gvzrluyho.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gvjhooibi.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/ghdvnwkyw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/glciuhimw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gpbihdgpw.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbluikxyt.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grbpivmyt.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gpbqrttdp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gwezshcrb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gqhwhkttz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gcjfrnaek.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbadqioqi.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gbdxprurt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gmrkokypo.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/geiadrsnh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gsjkmnrnt.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gusdaxnbv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gvompqpxf.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gghtxjmqi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpyidrsh.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gswbhfnbh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gtktkemnb.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gvqpqzjmz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvjkmhcne.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gsebwqrxe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gjlfbmcff.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gfldwewze.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gfyxhbzum.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gqxvcvvst.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gyzvcvcax.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gcwctzksl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gpzqxpqde.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/guwtyhdxw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gaephxfny.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gbrhqnhzz.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/glunhuovw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/ggqzgrawk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gsrffsgdt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gauftqzfg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gobttmuow.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gfewiotal.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gdttdxmtc.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gfmbhlwlc.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gnszsvyta.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gmqnjrrld.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/guutppuaq.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gcmvzrrbh.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/grsbrrqwf.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gytmzearz.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gfdrdqxan.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/giyvbeamq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/glslhjtvl.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gyofbxjwt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gapbssksd.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gkslkrebs.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/ghkwvuemm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gzmulijgi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/glndcnxzq.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/grpviacbv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gqxmfpafl.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gbqpxkbqf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gdjosyxfi.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gtyyioaqi.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gmkufxxhy.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gehpttlle.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gujpgasuf.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gpjvrrznv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gzwxhrmsw.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gccuvxtbd.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gpefkkeiz.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gkyvxjrae.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/grvchfpvl.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gosqzfkkp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsxxmjeun.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gaejsuwfi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gxzplpayl.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gclnafvym.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gvfotxxvz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gijxxubyp.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gskboovyy.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gdjgmefzb.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gmaqbendx.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gbufvhgdh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gkkcallan.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gblmjizup.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/ghvzolalm.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gguqvgfwv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gtjujzhof.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gwiksckzw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gxpcftlez.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gfvjksvxg.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gtwfkjrrr.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/ghxmcnukz.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gukqkwnwj.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gbksfvugk.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gcfqhtixv.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gkhzloots.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/ghrcihrsh.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gtfrrloux.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gxrsztjym.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/grgrdfmcz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gyfuowmax.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/giuduunzw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gzetkregk.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gfcuhypny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/ghytbnhav.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/guclinuji.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ghcgjqtez.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gtpvurszj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gzcwudkux.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/geajcmpun.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gioeaylhy.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gtatlzbaq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gkwsebgnq.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gusljzjol.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gfeonyzfg.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gjdguzxhc.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzirbvumi.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gzuqxicgn.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqonclgsi.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/guummywfb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gfewtyxhb.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gizbuduro.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gswvqttwb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gwuxbucat.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gdeunosir.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gfbhtdhgs.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gajbzbyic.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gtpyhjiao.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gabvspflq.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gomafkozx.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gemtaeqip.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gljbufwrd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gezvymskj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gymjyootx.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gdtmxwgmp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gemvdwyqy.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/guzjjrlel.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gfcuugovc.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gghsfzndq.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gpzrpjohz.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gfezrpbus.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gnzehljny.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gacxaxwkh.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gzayypqoo.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gzvdsuhvr.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/goncafujr.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gzynmsmzo.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/grcopsbhx.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gvojsmoqi.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gbfpsaehx.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gdthfehct.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gkdpftiux.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gcnsusmdm.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gkiehlahf.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gniuoaqcb.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/godteohsx.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gtbqwitjm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gqpbjjuvt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/glaxgpnku.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gouufgahj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gebauijur.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gdctvdpit.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gmfgjmtkq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/galnjgmay.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gcvhumbat.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grarnnbnq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gjpfrvbsd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghupoliai.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwwkmvwch.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnubabkud.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gdwrmitgs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gzotypndc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gxnfhqokr.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gxhfowhfb.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/goacwjnmm.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gdtelrymu.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ggjftywrw.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gbapiafdm.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghygjueme.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gqaaslhft.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/guteawnmn.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gybxvnfbp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gvvsoqsrl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gecjokqdo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gadisvwtb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gzwtzwauf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/goiijljro.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/goiiaqgfw.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gvbavxbfz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geeqjjgbv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gmwwvolwn.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/ggchxwjbs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwqiqkcab.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/grlfsfiki.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gswevcohc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gvgwffpwr.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/guevbryyr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gyichqdlv.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gdhzyzvbm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gvrsvbpbi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gktyytfai.sHtML


<!-- 参考信息 -->