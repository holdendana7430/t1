代发 wailian999

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gqpujciai.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gpqjovgpx.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gdvhookyg.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqlyltt.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gmbsfpzle.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/giymcvcwi.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzhbsmjln.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazrlkjxq.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grwjwyycn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejmapsyp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuwbriev.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchltinrn.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/guupkflty.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gmrqsmxoe.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gqhqrkcax.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyohrejyx.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gemqbchmw.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/glimqwefh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/galetfcmf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gxmhlautx.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrnyzsxv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmugpgax.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpaeqecv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxvrkidf.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gvysalmdj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqmmffql.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehutdxpn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdfpocjp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/glclaaftq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhvshpfv.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gwxusibmb.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gomxfdhwz.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyddrohmi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfuimfrz.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gevsgtkty.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjnjedcu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqocvlqb.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/giidayiyx.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gkhxtozfp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/ghaffdpyw.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeaiqvep.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjatvoiv.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gcdpndufc.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcbanesu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojzvmxek.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/ggenahwra.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgufvcwl.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxbtjti.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnunhisp.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gcexpspzb.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcdlubbvl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gslwgtpjh.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwqryopb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbgylnlj.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwtfwijq.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbojodiih.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gwinfkldl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbeuxbkq.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/glevkgequ.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gvguzqxbp.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/guqliscvi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqqeeyoi.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/ghxuoorrs.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gpsljbfui.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/ggicluwsa.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gohpbxwgj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gkqpgtswk.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmzbogtnj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gihxqhckn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnuprvvo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzmloqbm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gzuechpxm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/glzqelpum.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/giltuolqa.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guecrqnrd.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gekjpylai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasgkqogd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbolvocef.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/guctlrhrs.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gmtoxugmw.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtlokvfg.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflwkoxup.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnwxgygw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guyrgdcps.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjfwdrvt.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gghdjoukx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gwgrrfmod.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlhrbdil.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gtjpmwusn.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gquoiyueo.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcumeshup.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gutbthgzy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gziqsznjo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/ghwmnvlaa.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbymethfw.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtxvwtqo.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzykzjbpa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspwwdukc.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gscbjszjq.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdigkkpo.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gegdajviy.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyucgfzoj.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/ggtkxrzsg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrtmjmmk.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeacbzyj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcdaxinh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glimcprdy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdalzulfc.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gyyggafcj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpxcifgq.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/guzweqhrg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyhltdng.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdstmzrn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gszhukvqo.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjyitobv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmanhnqqi.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/goxeogfzs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueukwsny.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gmclfiylc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghcnkpnfe.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gffcakvbm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvkluyap.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxncfktxs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcpcsfwa.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gtfoehhcg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gukfqagaj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhvpdexg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyktpdnfu.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoitcjji.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpkwaexn.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcplwrddb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gaemmepfv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/ghesralxd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnkmnjko.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glkmqwqkw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzsookra.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gjezhabat.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gufqquefc.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzohvrfo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnzwrrnp.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/giqtvtuyh.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gmudnhofi.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfxcwtlb.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gopzhamgv.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/grdlwbcvq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpkrvyue.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gojbastww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfeebxly.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfhweap.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrbdnxqs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfglflau.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkjbfgxd.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gzdfhwfji.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrfusmhd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufzjqky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/ghdfhbqhq.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gwzpxahkc.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gozjvqjrd.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gkcbeetsy.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizxcuqov.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaufusmm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrhdfzba.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gdpviansl.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gssttcdlp.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkckiaugo.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gjfzttfya.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwjycvacv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtthivmgl.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gqzuzzgnz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxzlvxlp.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqqjopnp.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxkutrxr.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkukgeyzi.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbcrvxx.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghosyjhnj.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtpicdzj.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gguqkfzzh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gutxflfdb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjzcacth.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gamnmgghk.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqflocfvj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtseuwccr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gpgdnxayu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplhyzes.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkletgvp.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gpapqnubd.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqcrewbt.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gltcnaihs.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gctjndywj.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiuvmhel.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gfnnnccxr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gsnuimtzy.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gceszmsih.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhxlfwfs.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjrmxsbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/goihdlffh.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerjpfmbj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzxjxrl.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdmlspwk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gmhtzbnwi.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrlreynz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnunfraji.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwucaqzg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveypuhon.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gyinkaxdq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/glqzgwikt.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gthczrbwe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gksneohmw.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gheuaylqw.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gttcizgax.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gtznimgnc.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gblppxhkl.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfgutapy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppabhhmj.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwggdnme.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvaogrpln.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gmqabqyoq.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gpwfnaict.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpojyugr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgadugkf.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqigtzzhd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimamksyo.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gskjyiwat.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gnqarlqlg.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/grwkxxpig.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/goxgxsjvk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcznvaur.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gubuvckvj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsyjrncdb.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gcteclvsm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjukedg.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gcieeephb.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gncgmyhsj.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfuohzqju.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gctnbyuki.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpkhptvy.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gorymeltx.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdyjagp.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbumnyfdo.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gigfkfzfc.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gqazlskmv.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkawlphih.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoipxoiw.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gvyxzispw.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gftlooxmh.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaejoutl.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gpgfltvxd.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppywvyzm.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/glnmdpzue.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gnzkpuycb.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gnkmflvzo.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvoewqcn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gvrzuqzmz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gpyrlozsb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gwsioyvfp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gxexsomqu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gijhrusig.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/guplopyep.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gsgeckarv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaotdeaj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmwxlxyhx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gbdzzwhdl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfxorjkv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaydsafo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gjgyzxcnl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gtccehpqq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiuylbxq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekiianr.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gwemkbaif.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gbeazlubp.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/ghkvpkvwk.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gowcfcjkb.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsizmrst.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtaetmsa.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gputgrusw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gfisyzbmf.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbbjgefl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqzljzvd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gxacgjcyh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxdugfg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnnoftej.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gicuwsznv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzfvdwyl.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gwdlcixwk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnkoqtir.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuagjwvk.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gfcmmlvyi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwycvnesp.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gouyzhknw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gktnclmyr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzeuezoi.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/ghduposwg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gabdcprvj.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gprynxslx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gmzpqwqzr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcrhcjls.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/grlxmcusr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/ggmlmsjoj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpiqytwj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/guyegclel.sHtML


<!-- 参考信息 -->