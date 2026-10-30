代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczfglmpq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtudqfobp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghjvbsisy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwzjnaxt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gsahanwdy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/geuywqwgs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gusjbyxpq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhkalakb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvriiyk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gskqphmho.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/goieelqge.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjzaqons.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqrndoim.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfngthon.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzzvhome.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuymcuke.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhgfcufd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesqtgzpe.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrhwnnzf.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcsqaqaj.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gpirbdsgx.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gntcfrjnp.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqybewskj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwakiqhf.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmegbkpyo.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfuclrwp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvzhyykzj.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glasxzzee.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gyfllwreq.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtuqohfx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqbakqvs.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gaboocgce.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gcvjffhoq.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gtlebmqxf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gdeogfwom.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/geyofvevy.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmtnliwld.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxotfjtxz.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gytzmxvkg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkhhqxjv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gpvmijgxf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrdqnhjd.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gskjytzro.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyyytmus.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwucxfzje.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfgxcpp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxokhwmu.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/govgzqrzn.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjrgmrpzr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gspwgwqeh.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoielcju.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gmewzfmkz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwpfnshz.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilvwopnz.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gqrfqweqm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gffhcckwr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzxbpkgo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/grspcnvwh.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdyzyhcp.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gchyunnnq.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpfagkza.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/ggojzszvn.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/ggowdovjo.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrtzcklr.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gyaljcjnf.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwnshbk.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtxmtuk.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxovfpwl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzqfyunt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrggmcoe.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbytemfdz.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gqdfxmkaj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnrbvdov.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grleprsvd.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gydshvvlp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqzgeeii.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gvsngtkxc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyvevfpe.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gijwfhloc.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gysqnqgnw.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gewzlxtbs.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gsavxcboi.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gndjingiy.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gumsdbwvk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gxmdianyv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfrykukc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbqlnlgf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlyripnt.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghexuoigm.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkkybaro.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glniptjfo.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqzhwtdjb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnjnifgq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpetllvgk.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghlskxgcz.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gjhngwsvt.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbysotegi.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusuzueqz.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glpnvxhxi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxickwbc.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gthkdfafw.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gzmmyohph.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gnggrdadx.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guvxinigd.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvzpdzrx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukiybdbw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuppieli.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhoojlti.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqyvgazn.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gavkltasj.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gymspitgk.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucwtnke.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzafblfr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gptughsnh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevdolifu.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbhuyqwzo.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxxuoikd.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glfvpnlmv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvgmcdms.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gaqiujion.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gchqejwoz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbnrazxf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gpfywnefw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtnktuli.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/govgctwtt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/grorulbib.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngllaugq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gxvxmqmkn.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtawwkubw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxwsnkdy.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtgndkenj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gkbyvcvwd.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwgocifo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdmbmcxlm.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gzftnrjjz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmswntcm.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gsqrygbva.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsrsofdt.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/guoqsaodu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkgonbvv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynypzpvp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gojozftzx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gtmnwjkom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuijeuqy.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiljlcpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhbssndh.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gcrevcdok.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlibmbhl.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gskdalzch.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gsihhouia.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gluhqscsf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gfqusuyls.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gbskzwxcy.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gqrftonjz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/goheotrco.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyknzdjaw.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrugqzxs.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gssfiuigj.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gkllxcjrx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwvlbztu.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gpfzbcevh.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/grjlzkuhr.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/geihbdbss.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkwcbcj.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gvidbezzt.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/grscvrevh.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyrldlaa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gnblxrkot.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gboiswrfa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gsxmnxweh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnwbvzdn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gzqcbbrct.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gzawuucrm.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gxifnccfx.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gatagnsfn.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gijjzvgow.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gqigpkxrt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcemkkrs.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/giamywkbv.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuykoerx.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/ghmxpfqmx.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjqihexv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdizdvtae.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxtrjezvs.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqosngsxg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gwmcifzay.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/guontbpjs.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gobaintrt.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ginnkwhbv.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaubmknux.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhdvpbvn.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkrfjusa.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckfxarmm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplreojua.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gsmxvrxif.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/grkkfiqmo.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/glyjylfva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gojbvqkyg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/grjmkccvh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdruaiys.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsalltop.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztotbwwy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gscvjghrg.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpnyhmwd.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqjvekdz.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gaprgddvd.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gmgolgpmi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gffqbuvlu.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvfmxqkn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gulmeckkj.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/ggluhsxwe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/goqzwitbm.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczxixpve.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqwrmlzpq.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpmumxmlz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gldlpttyg.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/ghjpyaoqm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoqtoniq.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gthtakrlt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/ghatdetrk.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/godnirowd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehoyllpa.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfqnruvp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkkkmrd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlfpcthr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrmempdp.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gpchbjopp.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/ggfotadof.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvqxpfhv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyepwpoxx.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gesurrqmq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkflzwmn.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvivjwcg.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdqswyro.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gatxddvzn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffiamcy.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gwolwysob.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/geshlaxqv.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gjwpmxprj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gehxfyzqo.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gjdwabwts.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gggsdascx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrbtoymx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gtfyitnwd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnmhfnzr.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gffrcvzpu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggnvvscup.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/girqtsdue.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gafzljmxi.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvpgwdoq.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/ghxqfxiro.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/genrhgnpt.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvrtwjg.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gvihmpnls.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ghiijneiz.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/glmflikqu.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtszkxpxu.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gltzdnzmj.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gikncgwfu.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gsulmcglc.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiwxjlrn.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/ghnbxejap.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gugkqwjcf.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gvbdvhjqe.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gbeigkwkr.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gougteixd.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/ghqrulvvm.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtlmxuum.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gesxejcqt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gehqtrewc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkbbokua.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gxwabccio.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerrfcqjn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gllriennf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfuantnm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gibfypfjv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtagwowjr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gdilbxewm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrskgorw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqcemdxh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glqwwixxs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/ghluynilm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gdjyuhrni.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqdjofoqn.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsbpenx.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/glcrdjqqh.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gudixqihz.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcsvjfaw.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhzxgjix.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkgyjrl.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyxmmvqi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/greeapqwu.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/guxyqypoo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gspchrjaw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjlvfobd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/ghxuwassa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhnzdwfe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gcgrthkvs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpmnswka.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesetlvlq.sHtML


<!-- 参考信息 -->