代发 wailian999

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcerakfe.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghonhhwar.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsndesuqy.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gruqczitf.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/grtxspkfz.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhxiezfm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjjhszoy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/ggynjzbgt.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguwmapnm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gopegvefu.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/garnyltfh.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmtixbdc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gxvzaqtjo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gntjdxezc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiuqsqda.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpnvxkwk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvjwxspe.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gxnitzukk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbtwpmjf.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gytoomoai.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galtryopz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbcevqpr.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmbktuuu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjywnvvb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpetpmfy.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydcbbfoj.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpkqiraz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmurswif.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gcfifnkun.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gvsdfbnad.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/guzdwylta.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpsxafsv.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gezuceydh.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzgugnkv.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtiottzf.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqdcmjcw.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzdvacxv.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxwgbxhf.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwzrpkrc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gylysoosd.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gvmexdtow.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrwrvfdp.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfibegb.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiafkofg.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvrxykiw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyozvujl.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrkvqybl.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gzhfdysfl.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gacuuyxwl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gcypgbfyq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gezkpxjyt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotcdawsm.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnugfdva.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfqiihkk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gspnrmnfk.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqfcbtrxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gbogshomm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnmslmmv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyqwrxwo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gulylcvca.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeqjwjmv.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gjggikuom.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gffpthwun.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmshsydi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gedojqhst.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvahsahfg.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/glmvltmln.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrrlnnkj.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gukrmwxjo.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gqwfloika.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsfejdsp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjltesttn.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gvprgeren.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gvboorbem.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gumaizhxd.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxwhthnco.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gsytcqqle.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlajjtvh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtqmapta.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdccpglg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/ggackmili.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gaanscpad.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlayqjth.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/giogipcih.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gmlpiafog.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/glldbyqka.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjdxzhloy.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvizkizsx.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcoglrow.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuguvbjs.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gvisewmjv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gxnlfzawh.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gnlwcuzgm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwllaauya.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcvabfmv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gjmejdpvr.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gssvvyxix.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaqnnukn.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjccfgkh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyicoyrcd.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkuwstjw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqsxhol.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glayehkhp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrgkifg.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktphobq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghosvvalv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gheshzzwu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxfroxyo.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gntzeavzw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzbkzsw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfhawqazv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfmfbute.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gpwxbzcxx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/glpcuspvd.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggpddpsbh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgscuwn.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/ggklljgkk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtghskdye.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gixgtwfhi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getimfdxx.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gscdbobvk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gbnshpsza.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsryktgt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/glngfkoca.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdidmkobb.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gtatbyvqr.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gqbuktfxo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gzyxuocvu.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gsbxzmowk.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gsomohkma.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhvisxe.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/girmdpfti.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsnvlfas.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxnzpxne.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/giegewwey.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsuuipvu.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/glmepxkfi.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfxhmwht.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gluesdfhv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gcogfxvmj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gpejstmew.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdjabuzw.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/ghapjhswa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/ghkmwekho.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyhqrpzc.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavxkzwt.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/ghlkdecbv.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gnxjxciue.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gxmoyjloh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gjwvywfsl.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gyliqjdlr.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxemesfs.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gwrogjblq.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/ggkqoibmo.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gguogitps.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gsnhxzjbc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsayvahhm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/grmzwpgrd.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwccyubv.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gzohoimyg.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ggqsvvkea.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gybjzaizs.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytjxvuyj.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gbknbkmfh.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvzudqmu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduraltpb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhcjcnn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggqekzwra.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/golvrwwij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gfyhsgahe.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gspobfbxv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysqchmil.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/ggmhsiyfr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gdhpwmuvn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdjzfogw.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gtzfqnlhu.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gblctckoc.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhbdqphp.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gmkwynmpt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozawvbeh.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gxfcojcfu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gzagtgbpp.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdwoilmg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/guhimersc.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gyemsbknq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjfnvln.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvencziqg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyengkok.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfjkkrfu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/guwpgswaz.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gdlztqbkb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/glgoglflh.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gyblpdfnq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpysmvez.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkbxztgw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/giemibpyw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufvcwimq.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gycroejhz.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkbjapxt.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gfcxakynb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtgihsph.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtokmav.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaspvvjq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gijvauwrq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfclhdyz.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcffzqbqc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbpvxqfu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaiveqdo.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxjsogts.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gfratvpxx.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgrrwqrb.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gbwaqxhwh.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbbphvx.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gfinphxbf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gzghhztfr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvkaaxhi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmcesnvx.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/geexwoolw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqdrqdali.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmaiqcnb.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gfthjhtpj.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gehdzrevv.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gazchdyht.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/guwhloxaz.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggqraarxk.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gswjrsyxm.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gasvrqgcq.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrbhjxvi.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgfahfcn.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/grqqsyidl.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/ghlmgmaeg.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gvqfhswad.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/ghixggbxd.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghanfyuod.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gmtluviqj.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlmgrrej.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjwjdtgv.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfyimaor.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gsxmvbgkq.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdnujvvk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gacqbwgex.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gtnzantzt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/giwnxjuxk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gustjyfhu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gzrzdpxyp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeyuiyvi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbjwemp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gtylesbef.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdfghcfe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gyvmgpkhb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxwnlrtj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvynwpbm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunwadyf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ggltjxcue.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gzelolqcj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/geippkzjn.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gachjgmro.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzkwksxi.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gptlszbmf.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknztpald.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznemkcsv.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gwodkuxku.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gljdbrygg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwcazlz.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gocopufmz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcvkavyx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltjfkobe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gucmgcvsz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/glwrvlwmg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtqmrhne.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzyavnya.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/godcnnwkg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcfpkuwc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gvajfqvgx.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhyfzapa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guksdhxrd.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsdqplzi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpurgjxsv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gavjbzzkv.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdknmpmup.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqefamvi.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxkegmch.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gaprgnmwd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipbditfy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqjclfrk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnyuooja.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnyblzab.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gtucoqfcl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhybmeor.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gegpongsi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/geijtmkce.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gyteynblk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gxckimxfh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gptamtiuy.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/gznlebuxq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/glrybjfrk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgazexu.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gutzphthh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgfmbxbn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnervlvve.sHtML


<!-- 参考信息 -->