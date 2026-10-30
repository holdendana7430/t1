代发 wailian999

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbfpgtu.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/guynkqqyw.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsrxllyg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gkhowgjyj.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gombmliax.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqlikvr.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/goquxxxbi.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqidypsj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gimxtusml.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gamnrqlgb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtprdua.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnjtugcw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gznlwztej.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/ggahbfrhm.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyivcuvm.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslymjppv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooucrvzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhoyiesf.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedtjifx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfuprmmf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcoaviad.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxlcqlp.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gegsxllxh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gizmimmtf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gczehcspb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlwwkxot.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/ghoxdvxwq.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhnwkmcx.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gfwzmsozz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gtefbamdm.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gbhtsmnav.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glofpiwrk.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxyisllb.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtyjnpol.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnjiznzvs.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggraeevhh.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gvgdlayio.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqiinuh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoinqmhf.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvibswv.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/galnlekdr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvgvvkbz.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gzxgaaiio.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbnufjcc.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmsliddh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gutmlfjut.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/glarwsedk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjkmmrzy.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gmnjofoaw.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/guorntgzy.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/glcjlrfyr.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwutijlbg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gogmtsabe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gudecnxzo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/guiyrzqlo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/ggntpwjxu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gdhsmkneb.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxozffki.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcdhfvmm.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/glcdqkmrs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gczqgldxh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlstitof.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuhzpzcq.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjocrzwj.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gufxhnarj.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gngqzgctd.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/guwjgucbg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glfhrntcw.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrgizbbx.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glswyyoms.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gcitsjzem.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgcpclip.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqujmts.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvercjjk.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdglkpyc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaybkpmpn.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/grfwnxwpj.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gcpaueqsh.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqxagiu.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gbbaqchui.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gdrkknoaz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyjbxgdp.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmkcswjfb.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnirsnyq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpevkgtzy.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtvfztsiq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfcipvxa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/grxzblkcc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyddixft.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gzbmczbsm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunzqyya.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gghsiinfm.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdjgvavp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/glmhtqhuv.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrwqomus.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/ggsidmfgt.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxzcqgmb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gwduybnfr.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdueqzva.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlphfndm.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxarpkg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufdszumh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqidjjzp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gzkotqrhz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gagylqnjf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gxadstbei.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlcocpc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfqakykm.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grbswbjtk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghmickgvs.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gkbqgpoty.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gbhhfrsaj.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gopepzvvh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/guexwlgav.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghckroalt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzrleurj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gvxoelqam.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gdlzkpbqo.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gutbbouhl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnlswyxu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxyuswvk.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvprytfe.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gefxsmsrh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gibibwnie.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gcomtqshh.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwmyunst.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gqmusozyo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsllyyhca.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gnyjovtiz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gjfqfwzus.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gobaavkhb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkxbcsvt.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/grnhnetyl.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gxmjjkxdn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgmubkms.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzenwcys.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gfzxgdran.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrmyuedc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmbvbrxf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/giqrbvftz.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gselpfisj.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gsoyfelof.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gagkimxpr.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkowztwx.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gngugpslx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/grwaqsjyd.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/ggponeeul.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfejdtfq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkrdnkjj.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/grjxnrnix.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmwaspbz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxptjfgjv.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gndrmqvrj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gvclknxlx.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gejiiuvcv.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqdwavvp.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gohkryefc.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gxcmcgicy.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfbqhppv.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gzeykhvhf.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gguoedsjk.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gpieazzgw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gaxsqwkwd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjylexzak.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeetbfef.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/geazxyzst.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgdppzuv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvzqyome.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbhdcdv.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrvfwryx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gkufwclxd.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/geunlsprr.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/geyryuwwu.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gtzoszrok.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchhqainm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoycvrqi.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gtteihwvz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxrflhax.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/glzdaoksr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwxywrnj.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gcntkvngo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gscdskllh.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/galnrqnor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdgszrvg.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gukqkaiey.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczjnfhfh.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkdibmrh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gidgkgswa.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/giealoupn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkfrriip.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gyugfekjf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gvslfxnss.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/girnchwbi.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gkvtwemvc.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqgsrho.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gprvamzwa.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfpyzhiu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnvdcttq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/giwegllgh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gldpciprj.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/goalnzotp.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gnvgkwvls.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gugbdsrae.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grqrzfvya.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gphkiccry.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gztrjfusw.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gtddqdgrx.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpvhrpgs.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gavsrptyw.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcqdzpyr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gunvwroyt.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gcltctnbj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfofhpxbf.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gfrtwqdol.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobfszus.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqellkycf.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/glwidwbjz.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvniyqrb.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmnlxrzn.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcnjifvk.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbqhmtqm.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gakqujgfo.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkdzmidr.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvslcme.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gorlzujsc.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gvdnckape.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gaasuigms.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/goqaycovq.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glokhwiue.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gvncuuubn.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/grlwkmqjl.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdjbzlvb.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmefiliu.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gcrqdrixk.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gsxdsndso.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gsfnltwux.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gqcpmnbkq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/goypkqess.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gybccradj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxdovhzm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxhthjwk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gddlslrlo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gevpllhwq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmvczhig.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gwewggfcz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwbtaefx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gggiqsyzp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvzqxsvv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxebgvkyx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/guoffvxmv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gfkxupguj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcopsxku.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqmnqfll.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbybrhjm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrwjidoj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goodoxdvs.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gwtyymnuj.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gbwuxkkus.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaspzzlw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdsakouu.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gayaxzzro.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gvymecxel.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsnzqcci.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmlgmwwx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbwohbfc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gvmxistca.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/grvevlfax.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtgqnxop.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gokuvelwe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gmkphbyky.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlzgibel.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glsokdnty.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gqscltjre.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvroaxjjr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnknoqple.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gqypwcfgx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnhgvkjv.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfccxzdk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gzyfitwml.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnunohwlb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gykekmsxu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gtppjvizw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkmckryy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gpdtalxbq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzmfswwd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnwtqjid.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gewvhekfw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwylzxkfq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gofmoycpa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gcctlcoth.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gexrghvhh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gctyexers.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gzbqkqfid.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gkjctzqsf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/glgvzapnq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdgnskoyc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxuqlhoi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmilkvhev.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guxsgdkao.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghijjpkyt.sHtML


<!-- 参考信息 -->