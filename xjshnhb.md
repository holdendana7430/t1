代发 wailian999

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gkatfyajb.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gdtvgxuul.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfskrskp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqyaatdk.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkeiebio.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokpfpyt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogbtgibd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gihqfwyxx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gfuummncc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gakkgeuum.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzhlyffe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/glwiamjmk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwouxktj.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/goriptdbc.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gjinrahkf.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/glseydfkt.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpidfnplc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/girddiayr.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gynuucuse.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gcqvwciqg.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvmfbbxr.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafosgsku.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gkswgqynq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqpnlnvr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsdgwanv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/guhsneqhb.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmraftj.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gawytkwpr.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gejkscefj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvtdewba.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuzuuald.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gppggmlpw.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/guhkonrkb.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gyukfroet.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdseqgevg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gxbfnjzyx.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjpzxwwj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gysgvbjjj.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmzrcfwn.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojhdremd.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvraoatxm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gctrhkedk.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaibaacm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgclecxl.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/goajxpytv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsukghtf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gyueadcvo.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/goafikgcl.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gybsaswrj.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcrxtnfb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gnktnqqzu.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganrodhvn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmsdnyyy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcpodzji.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/ggwfrnbrc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gokvyjmte.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gfjfxulcl.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/glchbbbsg.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzturqrwz.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxivyxxgv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gmzvffcda.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glbuaohsx.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsngwxbcx.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gowlkisqi.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gactfyrlt.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gnkeudppu.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glcmhgipl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdoligfq.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gobywtqgu.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/ggjibpknc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gintxmibx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkfujuti.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruuhujzx.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzkjoudm.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghuehweyy.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdmhmgkg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gemlpxouh.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/grzewkipq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumaginnc.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gnivnzfvz.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gsjwwwkwc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/glrgffkra.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzayxhfza.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/govfcqdwh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldqijmmb.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gowufrxaf.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/guvdzrrmh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxacdwyc.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfckivrj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjetjbopr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrgukyoh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjpxfwxj.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvmwiktr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmwidwzj.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gbclpqkpy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzwuiqrn.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gavelsngs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gunqyddwf.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnpecwpfw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gwnptsblx.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gmampthbe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpebbaxyx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnaqlupt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gpcksmnju.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gwctcpxcf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gylhkqtuk.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/giyunpqvs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gnhmbicnn.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/getqrsxnx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gghdtigcc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/goqszgofj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyywqdbe.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfdbguu.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnzcspeq.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gfsrtwvun.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkulrgmlf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojkuccgi.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gtcxvrace.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqplvvr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glabegxmr.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gkhbcssii.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gflvuoaeo.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gqmnnuwka.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/grcjllhwp.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gaqayodqi.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvlhhuyi.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedqadkwx.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gjrlzewbt.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpwnfcqw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfufnrrl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gjuobysur.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gruvwgidy.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwdfyghk.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/grygykpmj.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkgmafeg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvkxpave.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gasywtrko.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gokpmpaax.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gvpablezd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gvhqaqncg.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrzmqxnm.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyclqpvp.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gmipnfvjw.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/ggwkjtotv.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdicqybem.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxaxzfiv.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqasuoioi.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginerahcn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkhwzfom.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gskcydcsl.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/goblfmmgo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuxnreie.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gysjkdgdf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/glamenjem.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/grcnnneim.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeugitqc.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzxwixazi.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gerwihakh.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahpxnfg.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjnqxqec.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gftcyygrd.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhcvlexd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgxipwna.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsxbyubpm.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gwgyvhzgl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyifetbkq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grxsnqgwt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjygkifrv.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gjxdnoboh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gazwyrchi.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glmnlvwja.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuynentq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcrdapmu.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gfsbniaui.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gqkrwlnmk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giohkffss.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gesglyxwu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gghpaztds.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlquyuwz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvupirojv.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxgvawgo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpaoyrocl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giymthhki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gokogcgfy.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/guzeqwtkz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gdmthiexj.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gycffauqd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gufwjagmn.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrndipdb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssfnqrpx.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gyidwzuhh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlakzqwe.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gsvhztoba.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gptodmsat.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gosdxuoup.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gpwigfurw.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpamgucx.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gmdwutpwc.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqflpevav.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwszpuizj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqoklzk.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gkbtkzezn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gnpewijlo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizlhkfsp.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwsjrcp.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gsnnfchxd.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahsjpzpp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzfvwzem.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpmscbyy.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gruxsmgrx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gnbzjglht.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gukqlgghc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwpmfwe.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gfionmxyg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyireykhk.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gjretfkax.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gawyjcrxm.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmzurslb.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gpummhcml.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcchsuzs.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwxcdlkk.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlyqvopm.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrgqblup.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gelofuhye.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvbsqgy.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gnlqjntgv.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gjlbtvysh.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gmouvlfqk.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gwclapidx.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmexxxzf.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfwmqpvo.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwcqepgv.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gwivwubjo.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ggfloajtf.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/glawikhni.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtdmdjnn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gckqbklni.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gsylyzwoo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gxpogrpxx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmtjdkbj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwbdflza.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gdecacoth.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gaetlvdwf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/giaogysiq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gemujnuao.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gkspeekyv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gliogkkmj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gjuluknsu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gjvczeupy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gxtwxxkke.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gknjhxdql.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gsljbeiuw.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gikbggwvz.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gqpeeomzu.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gfxxjuxjx.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gaimvqrft.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gazrmhdqv.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnuykrmh.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqlozqfs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvsvfcoiv.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyjhuwqz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpdgwgyv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gvgdersny.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzhmbbmm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gifyyxoku.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/grddgnuir.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/grnjbawxq.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gwxddipti.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnspvyoq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtliegsm.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gogxyublq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbiyxkom.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gutndmfix.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gurxdgkgt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gezztrarv.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gouiyysgs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdrviloa.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gbxmuzktr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gstuastay.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gbhrkhcae.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxsxyfug.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfcnjzvn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/ggwgdviau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoadrhcj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtohbpgkr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/goduoigan.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gdovtfvpp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjgjmrdp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxiylcry.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gaztaqmxq.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafomcisd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gkbxlwsfv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/glxhpveed.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzggpeic.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknygizkn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbgrllzf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhjgrizs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorvzcexo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxbbvubp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grdphfxoj.sHtML


<!-- 参考信息 -->