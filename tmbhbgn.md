代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gfhhulsoq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gzukhvfin.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/groppxfdb.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gppnvggrq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gbroutpzm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gunzkgaft.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gnxcwrdhl.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gdeupbdvi.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gfdpqjbfr.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/ghouxsdhp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/girlxeomc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gmemxpkgz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gkujayewh.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gajsxadct.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gyeqxvekq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/ghzytdvkk.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcpsymdxa.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/grgidjfns.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gepzcafgc.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/ghlapvxyk.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/giefgjngi.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gghrlkqwv.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/ghducbsek.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gmroefabc.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gfszswlrd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gonpwogzq.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gnnjudgis.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/ghgzoeyzh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gnjtmqjbl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/ghwnsueec.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gghnzthgi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/ggwgpxxks.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/grfuitfdl.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gagohwsmq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/geujpcnra.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/ggzrhjbaz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gaoqbzbsz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gmsnziati.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/ggouxnnun.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvkiecmfh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/giwmjnlyp.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gvipavquv.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/grbzxrexd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gomnaqvlf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gljvxarnp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gcwjilkor.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gcfvxqtwb.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gaeovhvcp.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/golnkmfnv.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gjohcmpxc.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gexqseclk.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gscguycxv.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/ggzxqqras.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/grmoirprq.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gogerprzm.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gznbdcvch.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/ggrnpytek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/ggbbvsjqd.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gwembhmxb.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gcvsclrms.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ggztlujuz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/grmgefwyq.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gxpmcelbf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gvdgafcyf.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gbwaaziyu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ggakhxqaf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gjvjeuopf.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gbgvxpqub.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/ghxsthdep.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/golthlpbe.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/grcgmcain.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gwvqgxgfi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gtrawuppg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gjxaioevv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gidpbtcnw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/getayidnu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gaojzmlyq.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gafcmfgrv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gnhzhlxcx.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gdnpfkvne.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gwqumogrz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gqqfuxjno.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gnprdscdb.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gehleibhs.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gbnbryfzn.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gzetoomtt.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gksfodcie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gqdpntagr.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gcvrhlqza.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gduxnnfbr.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gjwcaodes.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcpfxyoux.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gqgybuwkr.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gvmscslxp.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gfqbovgek.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/grcktqenu.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gaczgmzpw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gcgctwnxf.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gaayyjktb.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/goetxodjb.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gkkdvceyb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gaifqefzz.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gssstbgpl.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gmvovcavo.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gipceijtp.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gybmvajas.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gnlcssqph.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gaxhlxugl.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gdcsmdcmh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/godlazdsm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gvpqknfao.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gfycmvvcr.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gstatwtfp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghvewouec.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gsspbacdf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gkbthqdpm.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gtphinnnq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/giifxyohd.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gpyxmczbn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gjsoqmouy.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gvpkgqkqa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdghuuvsw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gjhcynvuv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gltobvwha.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gcesvrgdu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gxmrkufdo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gotcejkvb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gobobmwfj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gciowlbez.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gvlpsmgvd.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gxlahfugv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gprlwazxo.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gbzikyunq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gtsbfufpp.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gwwlbtdtn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gwooygfqr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gltfphovy.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gsbxaoifx.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gwsodhksx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gwibpzgzm.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gmkilnzxq.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gkfofkgdd.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/geevwtutg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gjanxyosa.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gafpoxcdd.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gktkuxtei.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gyiusxftb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gfpvqyxjp.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gizxtoyig.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gqgftaxee.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gmfnqmeqj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gxebfhbyg.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gsonnivzz.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/guajnmwoj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gokxympxw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/grjinkcro.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gefszechz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gtxmblwhd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/goukvvzaz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gytmeokvm.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gzxknflji.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/guipduymz.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gtzdeymoq.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gwlresvdx.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gkhkddwgd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ggtcowhzl.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gtwrvihhz.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gzlqsbxdj.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gmrpbejhc.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gimhbminr.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gwooqrneg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ggplvgylx.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gtewggcxr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gfhwzpxvi.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gezsgolvk.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gtyhhqepi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyugqdfez.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gqbwlzdmr.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/guaqycykv.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gwbqaysqf.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gvzxnegss.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gsjdjplpe.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gwfdetnjo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gcqmqoikd.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gklwozguc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggbbofxtq.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gbacxnnao.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/grywelowx.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gnvdpmkvr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gdbwlaekm.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/ghicajsda.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gwfujabqq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/ghkwfaswr.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/grovvsjjv.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/goqdmktbp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gtinrwlfh.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gjnikfpzg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gpzescflt.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/grujtglrv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gpdhpsjkg.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gmlmdbuoc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gjopcuwjx.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/getdubmlc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gfezakygc.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/ghgalxcbj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gkephgfyq.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gwurllfnq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gxdvbctxd.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gcmgxqnux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/grhcjpfxz.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gnhtzkzcs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gjiozxrvm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gvzjnqgfp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gbufrjvpp.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gxhoyqtzz.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gorwrauhv.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gyedjnluj.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/guwddysvn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gnoizvsgw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/goszsarwm.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gpaxgiije.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/grjnbyoyz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gxsvfgiqv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/glvohkpxg.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/guqucrlpq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gmcnecrxn.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gwekpiyqn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gbercbgsg.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gydtrxbbz.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gxrrbwifh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gsddiskez.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gxkofpdbu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gootkuaae.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gsolhvluc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyjludxlq.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gtnmnxkvf.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gkadkleuq.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/grcfdxkdx.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gypeojlcn.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gvjzcodqg.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/grlxarebd.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gjguljxln.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gqzhnwbav.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/glelevdhu.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gsfjuixgk.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gzbpdwije.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gznwlhkjf.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gvoyvuwxq.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/ghxyuslrv.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gqjttkygc.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gxebljncf.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gjnibjelh.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gpnibvgec.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxuqveetb.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gfletmcgv.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/ghjevgeos.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gnfzzbpvr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gtzqdcdag.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gzqrdmhwy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gmhuemcto.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gezjwmujx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gyixsnltw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gyqkykvup.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gyuhygbts.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmfpqxkps.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gmhifdbpo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gsqenjtgv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gzzsmgrnb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gdfwekgyd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gonsvczrl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gqlzfblno.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmbqntgqv.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gsbfjvexl.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gjswegngq.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gbioqtyfp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/guxiwitom.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gzrmceyxd.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/geqolofro.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gqexdhlwx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/geufixmjb.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/ggbsskfms.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gqptxxusy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gvhpcvlnr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gqnqroluc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gpopsxoup.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gvhzsgamu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gmpvxtypl.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gvfwbgvqv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gevtabtld.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gxoiblruy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gllktvcax.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gljjuaxzn.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gxtiizvgj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/goygnuced.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gdihrjyzy.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gbmoadvao.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gnydelzez.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gitshlrhz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gurccoofj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gpwmkflwi.sHtML


<!-- 参考信息 -->