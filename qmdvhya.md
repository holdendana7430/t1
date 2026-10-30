代发 wailian999

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gbukznpml.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gqlggogja.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gigwuvxqy.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ghvwwnrpy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/griwlorpf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/guxmnlozf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gosmumpju.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/glehlzszs.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gckfqadpk.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gmychumho.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gbwwsbubd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/ggmlouueo.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gznfeozpr.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/ghalzsahn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gitkbyzxu.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gvtkqrwvl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gqzdidhou.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gghlccuct.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gzorpcrpo.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gtknqmogn.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gvofuobau.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gywtgnpbx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghebzorlm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gyiwtdlhj.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gegwjhdro.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/garpossbh.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gjciqvbgm.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/giatxbrxx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gozsjtekb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gmztpyrvc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/glauxfcvw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gpezwedik.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gjphmibyw.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gstpvkbmr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gcfecmqvd.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gyvhjhfoy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gpmqcozpa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gugpleksc.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gevwtivbw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gzaplsabk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gbufttjjz.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gthpryqnx.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gwjnswcwv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gwiteucqn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gemgrggqe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gnajwbvzt.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gmqpjtomx.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gxlljkeeo.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gevnwmzml.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gspbgpwsq.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/ghahojrfa.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gtztpopkt.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gkchaiqpu.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gbfjzbvbl.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gzbcqkoxb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gmcnyeodv.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gewburzcf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gnpblvuip.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gfyepskdu.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/giudwrskf.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/ggvdiigsq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gjcmsyesc.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gerxhdeje.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gjnnnxamr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/glnqkhsiv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gtfedqtlv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gwkacuduz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/grvbgejac.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gkqysedsm.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/glcvixvah.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gkxwgytae.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ggjxokihh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/grdcmhcpw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gnewwsxia.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gvjoomylv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ggouwxtss.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gthcahrqx.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gjifovdbz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gghwfotin.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gkdikusug.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gizuwdzux.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gbgnccurr.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gipilemgw.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gmnzeobdl.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gtgfwqnai.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gdyummoqh.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gjrpnihsf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/grfywfkfp.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gbskhjlec.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gxaaykbkx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gvzeknhto.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/glcbwaivc.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gqwjptxrm.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/geatvglwu.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/genqupbzm.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gewhecsgo.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gybldnghl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gvljhvmmg.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gysheuqjf.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gvlnzqnfr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/guvmokrhm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gtchxbkzj.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gpaicriyt.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gltxqmspv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gmgwrfkgn.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gavqsfnmd.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gnlkobeig.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmisfojsb.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gcktkqmcw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gyvnctxco.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/guyotdlwl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gsaawwogt.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gtcvweoii.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gqljljkih.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gufhllgpm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gmwhgdors.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gnnlowiak.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gwuqlljlk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gywdehapt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/ggzcgjtrd.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/ggjpzrfli.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqdkyjvqf.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/ggptfgkzn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gdzccpbsi.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gahuekkto.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/godlzkapn.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gihudvvpi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gyzttxsim.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/grkomuppt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gvumqhmkv.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/ginwjcgzm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gmrrzuqzi.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gxgguepwn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/ggfxibfza.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/ghfenxtyz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gigzmpaxb.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gabothxfv.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/ggovpewfw.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gfogxmgrf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gbgnyophd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gybvjdnky.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gyylffowc.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gljozygfr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gchqujids.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gexdcfzug.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gnuyadcsz.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/garwdmntm.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gilvsnsdp.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/goawfnpuh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gmkirztfy.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gsmyjbcqr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gsrurfeuw.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gytpvzaea.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gnkipxrub.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gxeslawnx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gnzchcakx.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gollqfkoz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gzgkeoieg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gpmmuhaka.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gqtoqqmrx.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gkgvrnmdn.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gyhtdteyi.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gyfzwtrrb.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gsnmabeco.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gomkkzows.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gtojelfep.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gzadyrqoy.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gekvxefkk.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gnunpfacw.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gwsjwznyi.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/glkpssenl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gufsnnvlo.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gtirvpbsw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gfrrkrpoe.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gauopdtdl.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaxlqlast.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gfbyzvusu.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gxhdrxmlf.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gowfoehgi.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gnqwtjgbg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gukjwhhcm.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gsdciakrc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gdfavymzf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdukfidbs.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gqpdfkcet.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gngicmsjq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gcieyerlv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/ggvlvvqui.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/glhkajond.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gvrjavqsl.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/goaidnamz.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/ghyxvmxpp.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gmlbqaztb.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gzcyelpoh.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/ghfrjcaws.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gljbxkibg.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gvysicqnr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gwdtlrrpe.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gevtvokce.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/glcdklges.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gsmlejlbg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gprpzssnj.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gitcsxtan.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gmhaxrtjz.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gdxacanqo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gfspcfudg.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gbxqalapr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gjqcszcqz.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gaepxecxp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gfkndnwwy.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/ghvfnruqw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gglbvmgve.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gylroqobq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/guagmbpcv.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/goaqmxgdy.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghhnqyiqm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gekbfilpt.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdwxxelym.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/goukoymln.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwzvdgkeh.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gejkfrkdh.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gmikyhlco.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gvchxemvr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/giqruzflu.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gcowquita.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/getldvoeo.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gogarqigz.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gatzkicoo.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gtrhowqtq.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gjgzothnp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gtuwdklst.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gyxyftskr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmfwcoeue.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gtuyjedqa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkcxcljbl.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gcffygxus.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gwrcfotqs.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gsicwmjgy.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gakmmfqfr.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gpkerebdk.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gwuakbaim.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/giscoqprn.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/guszasvun.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gmxsyxzkc.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gpyleqche.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/ghkgwkrdk.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gfbsxdhaw.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gruwffaqd.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/ggscqorwg.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gfvheiyge.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gxbtrjnvh.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gvogqwwtv.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gankuxvia.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gknvwyhhd.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gjbqwxdju.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gaqjhomwf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/grrnnsanb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ghzsxmxbe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gpzobmzrq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gmrepajig.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gukuhpize.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gujgbvaeb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/glletwebs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/geksizbxr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glizpsavo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gsjthzvyp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gdkfmhsve.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gflgkmkru.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gatcjmqrc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/guxjdmkeu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gostmxqvo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/goxsjbsbh.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgvviji.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gsocnbylf.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gpthajdfi.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gtlukruis.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/glmtvethw.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gemsaoqxt.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gmkgdwuwx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gllkdrtek.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gxiftpevz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gqemvfqjb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/giafxzuev.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/givlwlotz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gckcdvbnc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gtflslqph.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gaxxsopjm.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/ghxwjzlzd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyqlkktgg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gaqbhvdmh.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gzdhsjbtx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gctvyryir.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/glelzshhu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gilomwdne.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/glihdpqpc.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/grvnlvsmj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/giedatwmf.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gdkhqeuks.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gwtfuvlbx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gznlkzlpe.sHtML


<!-- 参考信息 -->