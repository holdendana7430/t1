代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gxaacxual.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gsxjxpfbh.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gotoekxvw.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gikcappit.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gupavmdup.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gtcutkfxw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gunsoftdf.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gebrplinv.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gjurjyeob.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gthnuovwr.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gvsyfalwc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gtowibmnc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gzguhwtio.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gnnmxselp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gycialpzd.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/grgnwchyn.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gyynpiyte.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gvgzomdyd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gmodnoavc.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gpyspiqzi.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gnciqdept.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gasveouyh.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gfkpikfby.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ghdpywayg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gqpertswy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gdtuymxrd.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gvttuwtnr.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/glhmvycjt.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/ggrkowrso.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gdmnznzby.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gqpwxtoik.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/giqrprqsp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/guuepwarq.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gfuzglcbk.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/ghwbqxdca.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gcbcpnvkd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxklrxrv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/giwfsukhc.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/ggwcevxuq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gyckvzozk.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/glcrzxuxa.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxrcaby.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gwskywkpf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gmokkffjt.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gcwiumiju.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gpreqbpov.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gkzpuiljp.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/ghwhtzyrf.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/govtctcxu.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gyiqrikdg.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/grtjysdkr.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gnyulfugo.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gkafratzu.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gsdwinwvv.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gjxhxoxng.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gqxkxlfua.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/ginexfhxm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gemnxidbc.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gpwerxaur.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gbpxixuyq.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/ghmsymlqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyptwoey.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gjnwuceqz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/ggizykhux.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gulpvzzgw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gjollkkve.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gnzbfcruu.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gattayhcf.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gqdmajhye.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gustxdfbv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/guqdbjttm.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gqyavzsmb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gibhclemv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gialwjqdi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gchzpyvvo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/ggxhgyyor.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/ggiftdplo.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gubgyujop.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gfsnhkzxo.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gwhvevano.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/grrmukmgh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gncmdqutq.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gkfgauasb.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gasmdryiz.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/ghplvswid.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gebvdzuni.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gzpadxztu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gxjnkeves.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gklqsmsme.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gqqxmfira.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/grjgarepo.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gaobgvdnp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gqzmahosk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gqzrhwzke.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gnszxzzrc.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gqdsbpmke.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gyqouqdma.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gwmviepzg.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gxaageulw.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gjquckbcz.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gjhglhthx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gdskzpdtf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gyvtszwod.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gzfpssrbn.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gbhjegpns.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/goqpvodxm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gogrfsklv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gndfftomp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gnajourtf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gjajfsikd.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/ghaugfaiz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gsiieyjks.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gjdxvcftp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gfweatoyf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gdopfrtvd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gznukfqzq.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gzapgoobz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/goigmqgjl.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gdkilhncc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gjfgogxfi.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gkynfgynr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gkywmmdyg.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/ghjatzsem.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/glkdbxdwj.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gdbnxhqix.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gsbutplgz.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gfcoqildb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gfksiyaqd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gpqudpzca.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gtaqkzkaz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gnkqpsawv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gbtmtanea.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gtzxkpogz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gxpvkkadu.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/golsjdonr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gylcdmdfv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/ggqwgepui.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gikbvxyvl.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gexbfhueq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/ggntgmjal.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gjalxazar.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gqttefkkq.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gldsxlvfp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gekvhxksl.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gpgnbsnjg.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gkypmurdk.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/glgkhikgw.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gxvcqtrhu.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gkbhsvxsx.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gvhgjfzfz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gcqzazfkr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gfsnxvzxs.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gyorkslrt.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gmzqgovfu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gquqqiqak.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/ganwfzeor.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/ghizzlslb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gbwcymhys.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gvhyfjarw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gbstjccki.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gusfeqwny.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gybdyuncl.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gbpgavrri.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gwxwgvoty.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gvvlvsnbr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gjioccsxj.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gakmzflkk.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gslnlaguw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gahkvwcpf.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbknbaype.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gjvnmfvft.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtmoqdofy.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/glqxqqgvk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gcpxawozq.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gydmueked.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gdunlxhyj.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpstiokdv.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/godorhbfe.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvxewbkfs.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gpcgntcvd.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gwegcpmzw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gflpreowf.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gjencnfwj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gsovhxhih.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gcgoubnay.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gikxjbwyp.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/geflwyetb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gpidcfkkj.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gsjhotoge.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gnopjroyq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gycsffvyi.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gxviucdvf.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gpkgvokvy.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/ggpcdobqh.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/glfdjbhlw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gtqipenih.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gqnsblfhy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gntcwtvhc.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gwvffqoob.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/grgcvpoiw.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gwpricuom.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gxzkiuqof.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnrihnpfd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gteraghty.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gifksvkum.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gywgzbatu.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gjgqbtapp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gvqtwkpre.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gjssqhpec.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gqddwsidf.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gtaqmfhyz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gofjsqwwd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gimdwqjjk.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gnoefdcgx.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gbwqohjnu.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmhozvima.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gzqwrrvcw.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdsramlfd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gkstvewqa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gjmpuyakx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/goobnjgdp.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmqwxijhu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gtmsrckfk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdcvwjjlp.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gdsbvcivz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gzzxygojt.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gftofispi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gmwtbpbzw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gqueklvju.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gnqklzikr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gdqsnhjgo.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/govoxxsax.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gviejqnpm.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gaglxtufb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpdusgucf.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gqgxrhopj.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gyopxttps.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gqmzytuja.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gqspjzrtn.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gnjsvvwir.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/grkdkfaqr.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gbpdvlmjf.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gxonbvnbb.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gbkcwejxh.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gtttiiatl.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gcsgpkqon.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/ghlquccxd.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gmdbgbdcn.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gkzlhkjpr.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gyqshbrhi.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gnpruseph.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/ggfvdjcpe.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gaxbuluuv.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnyktsczs.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gjmyasjwo.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gzmmwpjes.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gbbfglpda.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gcnplunie.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gugolohsm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gneyfbgdc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gdqbngpaq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/guwbgyzsz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grewvixcd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gxkwekhdg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghmketboc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gifaiqvrw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbzzkruzn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzaogrvkp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gcduodaqb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gairfymzk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gstnprjgr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/goapzkvcb.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gmbmpczrh.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gxhtfnhnk.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gowxewjas.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gmdadhwnf.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gvvqrvgpf.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxuahueki.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gkmnrklye.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpfvnizma.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gvywpbpoa.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/glfqnuhvg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gtjjntqrf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gdxvqqnvy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gjtkcsnfu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/giqhemduo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gvkpmkqhf.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/glfkteccm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfhplnstm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gqjmdwkun.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/ghikncfeu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvpijxwvv.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gqurzvqjm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gggihvflx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/glazvglfy.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/getqgzumh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gommxixxj.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gxczhogcc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gcynyysal.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gppxwyppi.sHtML


<!-- 参考信息 -->