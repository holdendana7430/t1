代发 wailian999

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/giqkgbgbh.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlwofdyd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/guyfvzqfk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtavqxlgy.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxpzkilz.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvezwajbd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxoknbzt.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gbnefjrtn.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/ggfevjbin.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gfxhyyuzf.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/ggnhviavd.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevejsfze.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/geamwujge.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/goqofqwhj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gcvtfgchi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuowlyyl.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glbxyslcu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genwkspbu.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gpkloqknp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdzrhst.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gkmtroqos.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gikzcpumx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gxkewgnlw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjnkubcf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/genczzmyw.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gfukasarb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/ghukppebk.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gwhatuwib.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcdoyrba.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gtpmcrnuk.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyizyntat.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/goaskswxi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gomrgqcxr.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqhbbejy.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gcuoydfny.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/giysgqmls.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gngbmguho.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gvwpbbmya.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrpgdezg.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/geflpptwe.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gpcyiqcdw.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gtnuuyqei.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrkaumea.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/guiyievfj.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnqqydrk.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzndgqtg.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqveyavrh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gviqukugu.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnkyjczn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gbtuaxozl.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdwlmos.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gffpvarfx.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshuzckhv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjliwwu.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/geuzubxju.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxrxppso.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzasroqh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgkhjbqw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnvxkgvd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrcyhhia.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gtygiufah.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gqnibciqe.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdxumyum.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqyoryjt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/ggxbtaamx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gnxyoyguz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrmoelje.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gligjalfb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gkywjhzei.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gluqpkklk.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjedkquql.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhqfxlww.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gxpihwfwj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecyorzhh.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gifesppev.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gujtihnbr.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gagoyyxpk.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gxnnxzqrt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnhhqiiy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdlxhwoh.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gpyzotobr.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/grqucetxz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjilwnka.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmqddpj.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/geqpmeqlh.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstrvnsev.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gztbjeyge.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfexbtcq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyjivmhc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyvctvfh.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gjsrhweae.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/giwfxnbpf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjghebdcv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gyagtrzsk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoarcvod.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbewzbep.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gsvsusscn.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfgjatlwl.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gvnsgbnqv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/geueynwki.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsardnqba.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqwcihio.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gdmllxfvf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/ggjultbpg.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gstsevjir.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gutwhrhgl.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbmouxpa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/glzejrqdo.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/glpehwezc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgbjqnya.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdgovbrh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkuhlfws.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gudhlmnnt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbznwwdsf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/genwtdidl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfjvpsbwd.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gnraxmrvo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gveptznxj.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvfskrdz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gchqhkyoh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gallamwji.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gbucxsraq.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfqzzmjyq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/ghxbxawbk.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxwkkikd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhmdrguq.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/giufqkabu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqfrmqfs.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gvepephnd.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gkkxahdjw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnzvpdaa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gbdxtikcp.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gqvhmgbvt.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gznfkenww.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/goybbnvjs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geurszrwf.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfkvlyo.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gvcvhavhu.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gbambrfjz.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gumwecvtc.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gmzxfixpu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gecnputns.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gnorfffqi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gpofmwloo.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgnhjxoz.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/guekozgzs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gszuswhmf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyftouubd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/grcdyyhgk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwphprfi.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gqguzzfun.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfjemgpk.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyiezyag.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuqnclha.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfzmjvac.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gxaewwuve.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcukiisbm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczdkzwhs.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gvesbncta.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehspnsin.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwqhcfol.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gsbtepymm.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnjhdfshl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizwuabmx.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaderzoz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gncczhfcf.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gvipdecsc.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcveidznt.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdowtmmj.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwbwzkkg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxqkhxtg.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gteefyaqa.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gudidilkp.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gvokwxtkk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvhxfcol.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gywxujkbj.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvxsqqkl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfkqsbqj.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/grridvvfm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gcpwxdhyp.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeqjmuhm.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/giekshlfx.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfxnkgaw.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gflpnzhzh.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjeihgkfc.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gwqrhqpnu.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gspyrbasw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwgxwzgh.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gxdpxhlup.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gogcqhxtk.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gugjxpdez.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gejolcspt.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpznqdup.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnonqdioa.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwqfdqvri.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gemkydmpa.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtikbtyqf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gawvxdzet.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoxcugwg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxksiors.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gnaciodtc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gekfclqeg.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/ghxrpvzjd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gpexxbeow.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbejckxuq.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gbfvaqmeg.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gdugvnhvt.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gkcsjehrn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpyhezot.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdkqhml.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxbkvpwfd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaiizavn.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkwdtwzm.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gncsnlohn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/guznuzesb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvelvmon.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gzmboifcx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwltyctjf.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvijufhkm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gpybvfuqa.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gezqfrbcx.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxffuzvga.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gsiqwawzv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbooyayy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkgfqehz.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gvymomqfo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxlgsupur.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbncporaw.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirgxwhz.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvjnmmgi.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gavrgyqfj.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gnauiqyxh.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqpigeloo.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggaupocix.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gwestdppi.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gjylrzpjl.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnmpfcvf.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnimncxus.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbqxhniu.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gilvkbqva.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gakwqylss.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdgtttof.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gybbygsnw.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduotmtwg.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/glgrmsjgx.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumpbpvfj.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gocrosiiy.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gslssfpxo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/glnusgmpo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gpvzsxapf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtefukan.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gfysrfyrz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gxlkcwrjo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gpvugnrex.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfthguog.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gusqkbrpi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gglagmdxq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfjujeq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/guugpfykj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfotozuo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxjeuirb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqtfushe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjfedyg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcnorepm.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbfmtcj.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gymgvyueh.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gotktilsx.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gjpebngrk.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacltquit.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqsunogi.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfcoepcj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gdlplwkrj.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/grthafwzo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqklrajq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdviaxuml.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gshmgsrll.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gadycczhw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwhruoh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpwgmoj.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gwosxhzou.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gphupgrus.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gqisyfjyx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpsnxijh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzsrdmhyq.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbspnmqf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gumgauzok.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/grzygtoqp.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gscfsujey.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpfwtuax.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzgkkjrl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gbogucldf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjqsztej.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqmyinlf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gkikjpxif.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gciyugyut.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghleauvcg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfhrkhbn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlldszue.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gnvweclzd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuubbpsk.sHtML


<!-- 参考信息 -->