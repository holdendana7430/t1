代发 wailian999

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gjaztdfbs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glypyomod.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gmylcamkp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gfojwuoiv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gjpqylszs.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gomcbutax.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gdozfwfkl.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzekemkq.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gzuikmfbb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gejczhuxj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlfzgirz.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gbuswywlc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkqwbpbg.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gitojswjh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvfdzvxo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrzhgepi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxxkxyds.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyptkuxed.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkrojjql.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gzgatolai.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonifsguy.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnluyqhuz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/glsektydk.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmdouizq.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gncvgypsp.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gczunnrfd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhejwpyx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdxriafh.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/glhbzurny.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjgqcrvk.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhvkegw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmhwvsgf.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjjozzts.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyopjcyt.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gcmcmigml.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrzoyynj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gugcsmxpm.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gtnjdubvv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzllxonx.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gghufbvtq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsjucredn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgitpywo.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfokunvk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmostmb.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gmftnbtiv.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gjyralpbx.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/guontyjqn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklcarqlj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/ghywyrxcg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/ggrlfokkg.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmkmleez.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gdlbcvdnn.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gcehcsujl.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gkydltxms.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhrhkuaj.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gkshkujvk.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgaltmjs.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gzmklelxs.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxymlvmlb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/goremhylx.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gevvlyech.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjbigilv.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gbjhvdfve.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwcaqdkr.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gajqkzhse.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjioecx.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gsizmgtxv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgbnwecm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gackgkymk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghofsscrg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gregtixma.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwcanbln.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmwazikv.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyfymtwy.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gayfaueht.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdixfnyf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/guwgvrbgq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiuayofs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gpnvckmrz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgiptoif.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghpbpkyrt.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/giiblfnhk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnpmbvtk.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gihncivjb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlnlihma.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaynztozk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfehtlrrm.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gtsrfclzv.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkafaxxkh.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gijkgnsxv.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghcqgdqzb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gojahdaxf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjzspkgv.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gznvcgevl.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gybmjtjcd.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjuvpymtr.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkszmdnor.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpwisjlc.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjlifgzh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdokbfjl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gobpxxgqp.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcqqhmw.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjagakoep.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwqyrrq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjurmaxr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgpdcbkh.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/glkxcxjcv.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqouxgivw.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqagqtihg.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjjuvobe.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcufzwti.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gffdnyica.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcupmwbv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwhyiozf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/grolcjduy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzmawydd.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gjybmlfuh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gioiaqpbu.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gdhvuqlfm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gsqayuyil.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gwbikzqem.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gbuzzywvb.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guhsxjsfa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzafzeef.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gumqgsiog.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpbavzxo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gdcurmhxu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/glnfitkjy.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdiadopz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gfbsfltba.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/goromplxv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlxwnrar.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqmdqnye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymqhbfkt.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfsqremx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gygnfigdq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttahjqaz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gyijmpkix.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/ggwpwbwja.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjkshetj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbpaxqhf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfsvvudz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gddgwwrbp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/girnbkjpr.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gaxldmfav.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/govmmrvpx.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gakceraac.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiwgialb.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gbslvtmsd.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgcsjslr.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gmuyaepme.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqvincsw.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhntrnqu.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gaslspcuv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwsckpcs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/goaiabmyg.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gosdxpneq.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqrllyiz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdyeupka.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpggoqyx.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gvintgtfd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gwrvhnnyq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gtriirofg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gehvhsrkz.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbwdsodz.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzubvyjb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjwbtwuu.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiaskfuc.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/glyaoibsw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gssnopxhj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjprkmgj.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gprtotqxx.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gepnudxst.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzwwsqb.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gyplcytov.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaedhnom.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyuiijrg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/grscnziua.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwgwytme.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gtggzqxch.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxwmmdbr.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotdeifui.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geonweocg.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkcafxqi.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflxgtcgn.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gjpsijbfu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboruskhf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggnhpysj.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gblphalrp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gldrfuzbv.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ganjekzlw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gqkhrurph.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gsesikbii.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdlfjgdo.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygymgtec.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedttejba.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycrycjdw.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gnnritpqk.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gmawgbcqf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuruhpeo.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtblgqdhc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gotjddtfe.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxcsqay.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghomscoux.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gmtjjnxgd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrbekjua.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkabhhvbe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakuzezcr.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/grgqexntt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoozzxjd.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopiglqne.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiohcpig.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gskjoorwc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/geyouogwv.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gsekuzfga.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gqlesuuqy.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/glavvtejm.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gvevdbowp.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gqepobxra.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gnhrpkhvt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfkiglyk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvomveme.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxzgeawf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckovjkjl.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gqoxasiyg.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gawyoaqld.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gncppjrkh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gczlbprim.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbtglovh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejvxfgyv.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmdyikdv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrkljfj.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuwrupmi.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfjnryyn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaynyhznv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gmtexsuyv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gykdtiitr.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gjhwmidxi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grntcywnz.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoegupur.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwrwrsud.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gilyahbkx.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gzubppqsu.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/grlhcdudr.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxwpahs.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gojgydyfu.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmfjfbsm.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gopvtswff.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gxysdljay.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/ghqcglmwd.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gyljhruvk.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gmlrjrtrw.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyaswoit.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmhtghsy.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gdwrqhcfc.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobungnha.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtblnohp.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxfpbhte.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gdetaijzb.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gacmfdejc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeohincg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gmksjcimp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gtdahghth.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gvnycsaoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/glafvtmxo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gguakicla.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/guvurkpdi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqewomth.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukayprni.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/glcqqmcxb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gfmujtkpf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxplrzoeh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvfhabvt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gjteflbdv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/grrbgserf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlgeosqt.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/ggoogjunk.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/grrrrftin.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfyshmfp.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gwnsldsja.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gfhzbrkeu.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzwbeqxg.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gnyvzfqnk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gowdfpvkq.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gprvlmntl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/guarinfag.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/glkowbakz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtixcmsy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gwwbzeepr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbfbepbb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gucaxknal.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogxivati.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcfbqrczh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnvbhlcr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gpemmyljp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgadzfot.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gqizmzqiw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/glvbdrbrx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrmczvzv.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gjhmolktk.sHtML


<!-- 参考信息 -->