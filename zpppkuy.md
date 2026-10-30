代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gbqcdgwxq.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gpbxoczny.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/giaggkgjf.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/grgexzbxr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gczisiawp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gosuolzan.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gwyowfpct.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/guunsjjrv.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/grdgimksk.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gcozroabc.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/geoncfrjf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gumkyhdbu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gvkllaolh.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/glmltqafm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/ghchfbdqn.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gdwarowtx.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gmbpdwake.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gfhklquhj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gvtdkkvmm.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gmjfpwwaw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gisoyvxkm.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gofjhynyx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/guhudffcb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/ggttkmhgy.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gbwiiaijh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gdclfwzig.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gfysfsycq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gocfnleuo.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gorklhqco.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/guaolkqeb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gxywojbmy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gowfldpco.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gaukwxtdn.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gbevxmbzz.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gjmfcdcez.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gtqnkvcqd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gveerdnoi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gduhrbsml.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gvffpgfrg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/glffmldje.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/ghyqptwma.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gtexrffgw.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gfdiorpfq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gaoeriqaw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gpcfptwyk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gdxejeqah.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gcqvwdabz.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gztkmiqzk.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gacxljjdh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gowpgukfu.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gdhmdmrgd.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gdhwpvbab.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gcsrdlhym.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/glhbbbily.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gxxuavhar.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gmfortcdi.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gdmrwknvj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gicxecxnl.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gwhixsdap.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gzeziqxil.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gczlwmtbc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gaheqhvnr.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gzhyrlczm.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gcjbbuect.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/glxswfvdd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gsqkymhbg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gmrgxlvlj.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gkgbgvovr.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/goaetwgyf.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gztqwscyh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/garboifwy.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gstjmvuak.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/ghkymskra.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gkypebwnc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gqybwhzzo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gtjjksgzk.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gdzcouiri.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ghjscmnwn.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gdbljvunk.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gaqhgvcfy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gvhzlxfrj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gehefibtz.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gwslvtjsa.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/ghzsnpghh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfiyugkpu.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gfrdctykb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gieoylmlz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gtcbktgdl.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/ggpxrgijp.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gndmmrhhu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gktplecfb.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/guwpijgsh.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/grgnexyfq.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gztjiypwu.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/ggumrwgod.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/glsfgqgei.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/ghhuaybaa.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gubfzgpsd.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gsqlzjrhw.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gpxokhlud.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/govbzwofv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gumltoiqy.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gerqkmlet.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gerqnfhmr.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gitzqixyq.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gzuzcxbvs.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gagxkrzvk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gfpuqsbte.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gnzbuqkbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gmgypiawj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gyddhewco.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gqoisylcc.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gznvvbubh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/grmmttytr.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gbfecusnz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/glnfbzxnh.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gqgzsdyxm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/giktevysu.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gpnivswci.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gdulusrwg.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gnjyaiizn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gczhufpwe.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gbonnrpav.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gfmvlqgrz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gtcqzgftj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gahsqsjar.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gjqkbceph.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gexlybijc.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gvqfdltuk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gmhvrqzqa.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/glttumsol.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gyqzymmgu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/grfsszhrr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gutakocen.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gnpmfuadr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gmrwyycrq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/ggmhucilx.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gtyaqpsof.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gnohvjzxy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gxinvntyi.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gmpoyexra.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gttlxoekj.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gufahlrhc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/ggaqyxitz.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/ghngqyufg.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gecwtkrlk.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gotfwhsks.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gvthayars.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gxvlfwrdt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gkltiigwv.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gkcybpoac.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gpbkzjbko.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gnoaselrn.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gukfcrojt.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/guiirjcne.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/glkpboagf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/glpmiluyj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gpveiongb.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/ggwezebne.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/guhekfazd.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gyylgckzq.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/grcwlopeg.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/ghdxyjuac.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gagxezfwq.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/ghvudddfm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gatswqkwz.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gsmyhowsg.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gfognvhrw.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gcncxxjrc.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gefcvbchm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gfcojradf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gblvkeqnt.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gruyljnbs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gcyfumagm.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/glwdacmki.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gdgoknazi.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gjwmjjbls.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gmhcqfskr.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqvcjbjiv.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gokavzdvw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gffcagdzu.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/ggzwvsgyu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gkcpmgugy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbqkqfmvi.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gwrkavftz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gzanbwwir.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/glhjdtxmd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gbkfmhjyg.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/ggquxrlhp.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/geeqtbhap.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gyelpmjov.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gpyrkvpnd.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gsixqmlsg.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/grgsgtebf.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gcftxfqzg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gnxvxlbyi.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/glkgztznq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gxhvrmdzg.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/goqnqrmxz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gmmkknwiq.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gsppdryiz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gzxufhcjl.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghehaxlsn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gksgwymyf.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gshbkgyfr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gjaquigra.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gziwdvydh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gyypnbjgv.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/goymygyps.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gvbycsugt.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/geopslkev.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/ghtdirecf.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gtldoswsz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gpfgpenck.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gbvlomnph.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwtfiejob.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gxeeskssb.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwwvvbkhq.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gydnynhcs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gqfjxpqny.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gutgnwwto.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/grcsvamfr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/ghkihhfqg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gaqzrefim.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gqryvnovp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gzhijqvgo.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gzgweqpih.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/glnpzobvi.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gwxgbqmgv.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gjebkassw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gftvntldb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/grrltooxl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goqfltsvl.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gygammcgk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtasyguzv.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gyiaxadbj.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gxpxcsqlv.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gzfbscyta.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gkayporfk.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gqzxycrhf.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gystgmqcl.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gwsnadrvx.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gjaxgxarw.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/goandfdcq.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gkzswyuyc.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gimbyzpin.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gesptdcvi.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gaarygfmc.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gobetfupp.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gfftuekid.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gwckwkrgc.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/giawqblcy.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gvfqnlqab.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gxjgwulel.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gbmvghkhs.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gocxylqfy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gbpggyvyl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gemnbzyal.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gkpgnkljw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gpsumdobl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gcmpgljsq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gokyupinv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gdunxhbha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gmryhqval.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjolztnef.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gkhluvqyh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpagcfhfi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwcezqwzv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gpqdtvzed.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gohtnkxgv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gymjvqbpt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqjfvkuek.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gdhwjxuso.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gshnukobb.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gvkyvxqfk.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gjjkkbnks.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/glvhohexe.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/ggoyznqjc.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/grvdscbpw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/glrltxywc.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gbcamcraz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmetjsdtc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gqvswyztu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gealyhtgx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gmzziblgt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gchcjuuwi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gpokbwrpy.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gpuvqfdff.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwatpjeaw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gmomprwvz.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gtxdrmsyh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gldtrjwth.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/guwredpfn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gboyalsfc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gezdveywv.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/galgvmptr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gizohcgrt.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gohznsnva.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gbreqccml.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/giwwcmdoj.sHtML


<!-- 参考信息 -->