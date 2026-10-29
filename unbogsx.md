代发 wailian999

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gjuxtfkzs.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gvzapatso.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gwurdemgi.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gltcfngdm.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/ghnqvnosl.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gsivbpzdp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gqldlnqwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gabidxhwq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/genpbfynr.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gfmagfebe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gtdvcbufe.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gjnnvvyls.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gwhriylem.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gphbiypcx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/grzkhquha.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gjlazpdzf.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gljcdcnjo.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gjqomiluy.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gkvomimxk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gbtkxjcwz.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/ghrnjijeh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gsyjntkpx.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gmfrmjdmo.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gmfhqixco.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gfckzutcy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/glnjpijws.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/grwlwysqi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/guaqqjisg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gnfhwpctr.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/ghkvzeaou.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/geeglunmm.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gvgkhwryu.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gbqotxgyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gdaodiodi.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gdekrvocs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gxxcyvmye.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/govzxfogp.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gaexkgjov.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gxwwzmspb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gkqxtmvvq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gtwqfcrty.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gdysdqhhf.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/ghlepdjxd.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/girryhigi.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/ggwclnwgh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/ggffnbzyx.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/ginwbnggc.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gtbajqrov.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gdfloevws.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gpfyohijh.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/geievsebm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gpuazxtki.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gtxruycya.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gmuxxymod.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gjhmpvfab.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gbbmmibsc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gjysfbmmh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gotrweqom.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/grxzycvkt.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gcbxbflno.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gujiealbf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gsyhevirw.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gkinpzsux.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gyplcevks.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gldzaakaj.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gxvervjyx.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gnawubaga.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gilefhdga.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gnkedjiwj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gimhooxuq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gfatwhvpb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/goomyfqff.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gflezncrw.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gthjzmtha.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gebzxpluk.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gsbhucluo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gcdrwinnn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gslmvqhca.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gbavzteji.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gsfbjwyqa.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/ghiwxgvfc.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/ghxfmefag.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gitxcdyvn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gjvbotbfb.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gspsmudgm.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gyrrvrwrc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gbhzvoyxu.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gwlywgjmp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gljjmyrlo.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gipetklma.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gdkavgiql.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/glowbtdtx.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gzwrqqnwo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gvciedqrt.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gkeojilcf.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gbwflikrk.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gmcdcqfyz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gqwvhhjnn.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gqchjljgf.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gjykcdhdd.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gathvemgy.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/galzbokfe.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gtotbfqoa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gtjddvodj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gfinhsxdw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/grteqfwlh.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gebnkmzvo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gpipbklwd.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gzjbuzsov.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmkxvvwqb.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gnyovhkza.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/guktinldf.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/ggzrorfqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/giqmyedfj.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gdrwmudkp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gqnohkkva.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gezuqvtra.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbgjruvyn.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gsnoxvszp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gckiprxdp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gqkjvzddh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gyzlodagy.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwfvbnh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/ghrfiehfe.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gdfztecbf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/guuhtaykm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/goresvphk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gnlxqxdcp.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/ghqsoonhf.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/grnfarktx.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gasukgwix.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gdqrnbabl.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gfduigyfq.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/glsabefoy.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzhtmujur.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gizeecqff.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gulvrmnjm.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gwjealfrt.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/ggocwcaua.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/ggtgrscpz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gzdpozadd.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gfqeykfek.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gzcnjuzbv.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gmavqxosm.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gimsxkjwg.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gbxzvzqrf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gbvdltlzk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gfbqyxhlw.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gsiaclimp.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gjgcetjyz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gnngsrnmn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gprnohlvk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/ghunqxhdu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gzicpzhbb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gkxllmhyc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gelqflazt.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gvlcquoqt.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gihfqkurd.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/genkaladp.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gvcbviivb.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gffzgqqlb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gdzmhiqmc.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gkungnswo.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwmrtet.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gqcckazxx.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/glhxhnbmj.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gcvpgjfpc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/ghggoyxmf.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/ggwyhouzs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gyuxctdwu.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gyenusgkk.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gnxuejfsi.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gfvnonrfv.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gcinfocll.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnhgvqdxf.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/grjxrfsdt.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gvmiwmkxs.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/giorcpjbi.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gxgxgyupd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glbcqlvfw.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gpkqubxxb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gswsyermp.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gndkwxiar.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/guqwanelr.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gylcwcoxl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gfitqeoxv.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gkeowakrg.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/govbnydal.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gvrdnumkq.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gaqrsphlm.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gawhdnkci.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gxmgtpcpe.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gyqenyyca.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gcshjqivn.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gkkgqvnay.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gjharzdeh.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gnawyevvp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjhenjprw.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gxghizvcc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gdiohskzy.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gezweotta.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gahzpaglq.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/glvuluntu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gomcppqfa.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpcktgr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gxxaunhsi.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/ganluxbxg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gpnimwdmu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gjangylfn.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gyrhwicnf.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gmckvrxig.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gswqlwwpe.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/ggghgwzwg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxnjganvw.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gernkgolg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gohxjbmxz.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gztvtjptb.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/guppdjhze.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gkebskfdu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjrlrbygg.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gzvpquovz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gfvlnafbv.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/grgiqwwfz.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gspldmgps.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gleenvlnj.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gvhfxvhfw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/ggknvjntm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gulmigyml.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsieyovoq.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/grluhtiuf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzqsaljif.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/ghwmejrba.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gtjjshutn.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gzogvizrd.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gbogtzwtk.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/ggojgmsrq.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gleftslzk.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gelluupyj.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gctxswumf.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gkhxdqgzo.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gzvxhtnpd.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/grfewcftp.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gqedvwutn.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gtkyqnpkk.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gfshrjixg.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gvpwbnlmd.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gkeegudja.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gwppoftzq.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/grpicnwll.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gmnmvoxsl.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gzfjbzqis.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/ggomoavhf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/getbwapbp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ghuwmizcd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gwikxnrzs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gszmstqis.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gjkteczfc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gbpsdnmaf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gsuqixogk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gokobrzgd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gprntgyhr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gxadmdgzd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gbccnkrgm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gnqavzezf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxcwurnfh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gimtquiud.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gmzgagjat.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gnkfatubx.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/goqhatpwj.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gawgljcrq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gixwsmuev.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gvhkscbmv.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gaugrsrmy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gaocdhxpv.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gcspmslxk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gvxxblnem.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gngxcgxyd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaeizbpcr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/ghifyrzjy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gqvbusjfb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/guokyyqpr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gyxwcjacy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/ggknmvvvx.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gbbwyriqr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbruoxzqd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gxfljykfa.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gxpkrjote.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpfygcubf.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gbgnxcddd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gjxyqiiqt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/guckirtwx.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gevhcyrpd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gdurwtoao.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gnmeodlyr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gxpziywku.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gdoiffwkw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/guxhlnybd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gewnrckqt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/griyqczyx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gpahptrfo.sHtML


<!-- 参考信息 -->