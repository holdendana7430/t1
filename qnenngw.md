代发 wailian999

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gputjccaw.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ggcntmvgg.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/ghjixciqn.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/glcbdlvzf.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gzpljtvwz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gaftuquyi.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gmpscdxsa.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gmpcbmoar.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gcxxaoqqb.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gpbfiehna.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/glcawrodv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gcbnlnnns.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gumolwgqs.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gzzhvzzpq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gwjlnrcbc.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gfmtclozp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gbfkvwtqh.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/guhmyjiqp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/glehxdhxs.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gbkdatuio.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gdqqdbkyu.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gpwaqeezz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/giryypkyl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gfzcifimi.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gilxzizhz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gwmamqgcm.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gcbazsyjp.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gsbdjzchc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gojdjmjrc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gprpwjlra.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gmzcrrlfi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ggjvaxvan.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/ghmcogdmo.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/ghfveoglj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gtmjhskbr.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gmjfjmoig.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gayfzchif.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gjlemfjtw.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gnprvpnhx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gpmmrrhpf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gbfjuihey.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gcezfkuwv.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gesmmusfy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gcwfrkhxp.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gpzserfik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gdjdtxtps.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gjwsdkqmx.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gkgurmkak.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gbgmvhjat.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gqvaanbur.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gahgjctpa.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gafijymut.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/glplbypvy.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gjbpylmxu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gazaejgjd.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gwzrecjto.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gjkpiwxtx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gvbwmclfv.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/grdbrcaus.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/giheiomch.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gcrxqwehv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gnhtpfpur.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gciqsaano.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gylzxshgc.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/girrbjrnm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gwfgsdruu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/ghbaxvidm.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gwzetjemp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gmabnpjgl.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gwrxmjctb.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/giovjmknw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gjjovvdqi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gpgfuvtnj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gqszjkejm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/ghpcmswql.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/girxmwxur.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gaschfuaw.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gpmnxvsxy.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gnqrtjaxs.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gbduswudk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gzrkrdfej.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqcujhfve.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gcjazxvgh.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gtlxbdngc.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/guwumohbq.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gbiahnmzu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gkzttlgon.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gdhchqvxl.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gchwjwfey.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gmbahivyw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gzxukrkdy.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gradkakxc.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gifmdjbzf.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gpwcfminp.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gjabfvzcl.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/glrlxlhre.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gtoustlec.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gvcenysyw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gsworkjhv.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gkgqjzhgn.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gaulpvtxf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gowsamjqt.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gjwhjyopy.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gfflroamq.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbgfkfkbc.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gjenajwca.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gfnosyypb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdduelaxc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gutiwktbn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/grfgnapvo.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gzlpomqqd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/ggjzypnty.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gczaxcbtw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfbuhuuxe.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gaeizjsrr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/ggtklqedd.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gkoflauxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gfhbtywqi.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gxxluhzsm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gjuqviuie.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gvbheruwc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gfuabgdny.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gooujpbce.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gqzpietgi.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gwveiojfh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gfymtgdwg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gljmcbdrh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/guahacvqt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gvifnvmrb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gbrdqhzkw.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gfqnlbuvq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/ghfbmnjmj.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gvwocpzak.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gknsgapvg.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gioxubsbn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gsbapgfyh.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gdiueamyh.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gfuddgmoc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwhwgxink.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gehlluobq.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gspomhcgw.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gybffwyhi.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/grmlxjnjy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/ghffurppx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gxbgxboju.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gmgoiscsg.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gzdkwxczf.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gjldebjqy.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/grgawuhop.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/godrlivsf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gumhufoax.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/glmqhknzd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gzvaefrfp.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/grfctevvf.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/giqyazhol.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/ghstowwnt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gbslikiyv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gjvutrgyq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gcmgzpywk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gsnwuognm.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gmnbcajfp.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/geeutcmbj.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gmyoiakwh.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gqzdyeivs.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gecplovcz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gjhtiuzsv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gsgxggtet.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaahratr.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gpcbzzcbr.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gsftuqyak.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/glwnxxukp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzejhzklt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gzrmkuboz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gfokekuoo.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/ggqaoevwz.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfruxfhdg.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gbhtjzdye.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/ghunnewrr.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/ggwgpbkgq.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gxwhiccqj.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gszmpyjom.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gezvzrhor.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gzvdqjfch.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/grepwblse.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gzbyjqzpc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggsbzngjg.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gchjjfjmm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gqodpnwlq.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gdziazdyn.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gpgruwlpg.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/goawbyyhf.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gpaogbdng.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gcbtiuprc.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gtuclxpam.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gjbaqonve.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/givxbxmum.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gyvghkzjf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/guqesqqey.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/glatncprz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/glbiuunbs.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/geieebkdt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gedmipzzo.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/grboabgik.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gidifozjd.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gflueubmg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gqllwjsfc.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gddxoxsdw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gkoazxxwd.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gsvtebuik.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gacgqwftf.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gcjomgypm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/ghgzhmjhh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gxzhgdheo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gobxokpnu.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gqkyntycu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gadwlwdlv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gzzjrloxq.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gskhtbjoy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gyptinicx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gafhcrmew.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gtigkzeim.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gndsearkq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/geiftrgsd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gtkgcblsz.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gcmpmchtg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gbdpfwkso.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gwdgaxaur.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gqgntrlxh.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gmlhkoodp.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gdwtpdwbr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gdgyxrsnr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/ggvwdvudh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gofvrtllg.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/ggilwcfkw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gafcukfmi.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gkpkwcxta.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gahgnwbju.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/glpjdaamu.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gyubxkabu.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gnvsvgklz.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gpzwfffzs.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gitxnluyk.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gncuydsem.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gwohmynbl.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gtmpfbncm.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gquvdyasj.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gnaofjoof.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gwtebpkes.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gqgrdlmgs.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/glqmtnuul.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/ggfqlgvun.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gaicqxzda.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gwqskgtof.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/grvgsylsx.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gefsqwrnm.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/goucbrbwo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gpxjirvoe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqbkvudul.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gkvcksdxc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/geomwfrvv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gdbqxptqr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gqyfwoyeu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdzetcvoo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gasibsfzo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gbfpoyyxv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gdmuwxmnf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqipirjqf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gnwxwayyx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/goamqvsht.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ghjdztbdb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gipaghqlh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gqreglsjj.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/ghmqkgoyo.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gjzflfhvp.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/geeraifej.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/goqubfazn.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gpugxovlm.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwatqiijt.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gqpwbgnzp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmyyhonpe.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gbhmakoop.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gtkbmjbgj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gofokzfbi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gjiucgfjz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gcnhslard.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/glkikgyne.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gzplawnhy.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gabvslcfp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmlqdrxbn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gbhgtijtk.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gzsxxfepb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gardezwai.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gxcjfsbkq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gtihulgzm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gjpnzgtbc.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gkwfqxuzu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gwlqnyaaf.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gziwtyhnj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gdyfgonoj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gtcupttxr.sHtML


<!-- 参考信息 -->