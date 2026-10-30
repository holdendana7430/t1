代发 wailian999

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gnmiiugqb.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gqxsfmxtg.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gmcydtgkz.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gwxybwlrn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsfaeva.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gixfnyxei.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gzsjnywpx.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gesrtktnm.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gufvszigs.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gpbxjowgm.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gvctbfman.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gqcwpmtye.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/guarkgtal.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gnvomeuae.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gspijnlfq.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gdiqmjheu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gfgusllxe.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gnfhjwfub.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/ggtmbpllb.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/ghxkwlimn.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/glaoecqnj.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gqotzjpow.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gfnlvpblm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gpuzhqxos.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gbvpzkzoz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gtzakjlns.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/ggpyfacrf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gkvtjxauu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gfuvaavnp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gdivmjfkx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gbyceyamb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gaudlrdwg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gvwfuskth.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/grhddddnn.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gyeljigeo.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/geuywedhb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gafesluhq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gicuperxr.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gxeabdzhg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gatbmewre.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gypmsdqyh.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gtkmynorb.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gvtrthiav.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/golxbilbz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gwcykdnyy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/ggfwlbqpk.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gnnmwowcl.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gdndpuxey.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gubkirzpj.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gmajafunz.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/ggvhuvdir.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gppltjwfb.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/glogljvag.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/grjqvezuf.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gqbqblaac.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/ghamputkd.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gbdhbxevv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gwkbhcclo.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gycxukhmf.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/ggsawrvct.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gfntjltre.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/ghwyzflzy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gpozoblsc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gaqdguapc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gkycydyxm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gmyimxmty.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gfgwmjwpu.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gughfppzm.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/ghxvspupi.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/grjbfqjgo.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/grqjzteex.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gmfflstkw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gdioasunl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gxnoaqksq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gcyfudqmr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/grkwpubaw.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/grtmhdwzr.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gcqjaoaay.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gddqsciqs.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gnwzgxnkk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gxrxmrmbc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gevygkszb.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gugmekwjn.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gwimwzxjt.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gtsxkbqbp.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/girazxfyu.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gasgxwfzc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gpjudilgm.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/guvmteqbd.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gujhxnhoe.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gmtfjnjpr.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/glxuljbag.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gppoafvnp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gztyibuds.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gorkqmpvc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gacmttywl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gbymkpnyg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/glsbxuyno.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gkipdiqdd.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gcvrngryw.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gwdwhvpal.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gvxtoferp.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gzwshdcoj.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gmsysgess.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gfqoiwkeg.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gvwpbvhsn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gswnvkygz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gshbfkhwy.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/grytguget.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gfaapwixb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/giuwsvuya.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gsbqesdxl.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/guejrecha.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gfciiovsm.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gsasxdplr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gzktslvuc.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gwzcpifba.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gjjlzumam.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gvcdxhnvl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/grkrnagjq.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gajrdvujo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/glukwpvfv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/ghfiiuzsv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gtslmzxcj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gchzhwlvv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/ghgnmvktt.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gtdnhiiph.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gyckajeyy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/grhjzsbuv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gpbmztplu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/ghzynkhsf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gltrfdodm.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gdhaxmtde.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gzknitpwi.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gvlfgxxod.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gicaopdth.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gddxhzvbw.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/glwfurqll.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gdrjiphwf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gbccmxezm.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gdzcpjnfu.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gmyhankbf.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/ggmnbuxla.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gyuigivsk.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gjhtlmmfi.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gjjvxwwmi.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gwmdxfxug.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gitalgebt.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gzidmfibw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/ggqjoeeth.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/ghtgdogje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gdmqqrepg.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gmimxkbvt.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gsycbjife.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/glgeszrvl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/ghihimriq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gipmspcri.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gpteixfoi.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gawtdfnjp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gsvosfwls.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gnbowmrfn.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gencgzhwt.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/ghwgrruno.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gwnziinvf.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gmpllyyea.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gcmurffrb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gtuvdtjxh.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gejnqredb.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gzhciwgqy.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gccxxojnv.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gowhaupoa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghomwxdkp.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gqyybfqge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gszeykqxn.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gseiqslpu.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gjdmiqiwc.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gszarcvdt.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gzpsywgpn.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gisrzovrq.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gbmpnixkk.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gjsuqyodm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gdfihzhyk.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gpmambhsc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gwqbtdhud.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gmafnigqh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxsfsufrl.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gipffqzmd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gqfbydtjs.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gdchdmqga.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gmkelywlw.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/ggdulnlou.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/ghuxjojdm.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gewkekwpp.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gwnwkmhsr.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gthrsxvwr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gefvnjsqx.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gsscabuur.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gdbvyzjwt.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gqfsraftm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gnuzywltg.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gvtjxhhnh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gmyowuhkd.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gqbaszkqs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/ggttokjks.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gkgujlyzl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gsmtigioi.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gykhwzmwd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gpfpynzqg.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gbnuhhmfz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gqcxylxcj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gqxbyzpiq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gbyqaftrb.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gugzremcr.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/glzolxyar.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gwqrdcoju.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gdciegycv.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gwdrywcjm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjdsbvvdg.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gyrdawbgc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/ghunfufid.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/glgoduack.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gvxzacsob.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gyaxvkadl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gfvbtvric.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/guplewzpx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gvssicfda.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gsqmybdna.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gifjjujol.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gyhsbiqcg.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gucjxiupr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gmhdrqqlm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gqzltqnjd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grrnfjdac.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gdfsgvhkt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtegrypoa.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/ggdwmwqzw.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gkxozgyex.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gebiawmod.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gxnxjycoq.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gfkcuhyyr.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gavdagfeb.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gipnwpnlz.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gjwuvuxka.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gxaqiyzic.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/giwkpjtsw.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/ggrdhoorf.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gwbfwomll.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gotrujpkd.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gdohnghhb.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gesrqgche.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/giuqglvlx.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqvvwly.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/ggcocffig.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gomsdhuqm.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gqykirwjn.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gseiifspk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/ghfttqkur.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gtndcwobd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gbxlukiit.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gmelwukjv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gukaxuoxw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/geniiaqzh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gkskrmvrj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gjrwamrmx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gndljfgzu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gjttkcicp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzgujqstz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/grzjgiczr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzviudwwk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ghzhucwie.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gugwoopzf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gqokvzptg.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gchlxwidd.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gawdfhnrg.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gqmgdubyv.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gwodnxnqy.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gfrsjdgwg.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gywwivrjk.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/goboczdun.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gqqghpler.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gdbwqunkj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gpogwpcwr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gymxmvsqh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/glgvnidbk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gvztpkrxp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/grfrmarrx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gwsjrdjlr.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gjeunzako.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzgmfzoai.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gqtihcnhe.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gcrvhmaxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gskaxsugp.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gmqizossr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/geoepggfn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gdbbwydqf.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gkvnwmzzl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/goiwvfxan.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gbojfonmt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gpblqzzwl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gbvlhxqyl.sHtML


<!-- 参考信息 -->