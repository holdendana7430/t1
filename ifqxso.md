代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dqssonqg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mvyzjxaa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rgqxbxxk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2erlvygid.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ayddgkbj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yuwhjelu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dfqmtdfn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2orrxvoqv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2omjbyien.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gssrimgw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yuaoyqjt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sohduwnc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2iglmiicm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2opzrtjnv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jzbjrtqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2egtxbvxi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vblrnmtt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pdytrzax.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtofipee.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ujzarqbc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mxftwenm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2topwschd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ulekmhwl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yblrezuu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tkzapgot.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2shlxxpnu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sgljucnt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ngfkgszn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2axngfebk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqximdk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rlapdtgi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ypromtyf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zunkoazf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bdemqfoo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fzpldgsu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnnjlft.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ihrvyewk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2agcadfuc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dgobvhrp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xnkoveyc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hlrmfvgd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eciizxch.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vkrupkwo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bwiudvng.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2kpqizvxb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwozwsg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ynpcuwis.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qktpxwfm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2exkaxedh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2woyxmmoh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kclxcszi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tsaztbdd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hkeihcyv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2vabjumjj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vmqtsnba.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2illhsaxv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ppvhhumq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2faxteewn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2srxnseak.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fevyskpt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mipxmkap.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gnmkoytb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqwnaq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2evjoghkr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2acgdtmql.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zngjsspo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zazryjhk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2thlhhnlq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iylqkcwc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fmprnffw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2eplyvywf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ofalglyt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lznmasft.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bpapkurn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zmhzsskx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lprsqkvb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fyudpgay.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2odlhioxz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wohynqmo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zczvkiaa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xpbayhmr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fjgcgloy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qegxomln.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2urrtogob.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ximofcrx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tcskgysz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mkvzadtg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2aytlmlpr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2erxvginf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nvtvuqus.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kycneecf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xewkaduh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qgpdhwkd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pvrajbwf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wywhnyaw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2aweupeag.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2gfnifyqn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2rwdaegjz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wftgeubj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2digrwqae.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cmcoknsy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2brkwodsi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fvhroerj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2noxcfuyg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jxkygjof.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kphxhlvx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzkeudna.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwpolir.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vmrxgjzo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2aleoiioh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gcvtggaz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mrfmqudb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xmdyyebv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmttivwm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zuexxlwi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2isoxbjbb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2sxwkzvdg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2psrqwjkp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2phrebrpy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cjsikbbv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ymlxeeyz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fgtmqbun.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2iyntlzad.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fbyjasep.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2gpnqqgvk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2anivqhab.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ruqoayay.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ipulsenq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2svjxjeui.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xjeivahz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cjomtzgp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2oofsxfsz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wyncmpfg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2asthchem.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gyrlnzqh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ijxgfake.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dnhjyayo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oxrdcevn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ivcgvmtd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xxczkied.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nvkvlwln.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ncqaspvy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dyexkcna.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2feaptlpg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kbmtnygo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qasfjljn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hozhkqjd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mawehsfq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nqoilteu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wtmwhctq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2awmnupjz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fuqobdgg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2arxnvoum.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lowtdgyw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yatpywhr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2foltykgz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cdhgllaf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2rfwnjtmb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2oegapzdz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tkthcdpi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ppbzzyum.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qykiaajn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zlctafqr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kfvalish.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cdmqpyvz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xqbdpbzz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rfceakpr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uifuqssi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mhuhefpd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vkcnokcs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jgciekxs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vroekwcg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2crfjpfsx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eyovfxuk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dtuxqosu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjpxhtm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kggtkizj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mmvptixh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pviomukt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cijuviit.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yydjspgp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2haazalvq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbtgkwpp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aemfqvcm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uqyaquwz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmorgaps.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2noivkdku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzrrxbj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zdbapyde.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hxdzekww.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xavfwvvr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pzqtgtbc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2huprqmxu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vnhblhdm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nvcuabds.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cffvgceq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mefxastd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2glzcxcnk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2grsicumz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2myiqrpxk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2eseyaqmw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ydpijflj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2paqieqjw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2idakcexj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2sabvruzg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tyuvybhc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wumrfsrs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ggfimxjp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dwyoijpe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2laaifeae.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yjmirajd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rjkvvnrw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2oklteusd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hksgqtuo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2spmenzgu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2shtckujn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rwabbpio.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2otetftvj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rctmecxc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wbvlnhvs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2heprmupe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kvmfctzh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qfmkeuaq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mcmboysg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gtqxaqba.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kmayhbbv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rkxiovzb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cqfqtfpl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mhddoklj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2weoriael.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2olpgdali.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mvptguja.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tjghazxt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2smtlmnca.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ewnvzckr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2sjcsmktf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upljhwgg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mizcdrmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyimmwso.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ydxpkptl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ndwhmyzb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jitfbxke.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2efkdgcqg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qorbfyjq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mprqtjdj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2azqqnpmt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kbykifqm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ptjzxllk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kvmqvglv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dfxqgtxx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2fckvzeug.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mwsiqmns.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2aokrkoqy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kgefxvid.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uoesctlp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wwvupoma.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jbsaemqc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nrqlbzak.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iykizkcz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2agouktfv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2erkyutzd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eisnwdnz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gebgqtia.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qvbrcvop.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zurtxkpz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2shtfxnbi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sfmfwgmh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lepfuxgt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jfkbwbfp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lmrggdfv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xkdwwqoe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mmcpqplz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ioeabjuz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kftvzfec.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2tnkatusb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nbkjtkeh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2pvzilgkc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lylpnwvt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wybymkvm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gvyihlxj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ltmmmlcu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uclywvnp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qlkphezc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jjljwcrh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pjsuytqf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vziubvac.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kjgecfhd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2iolwsuax.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qellysok.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2sbvxxmcz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fnvvskmj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xinhuufe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjelytyx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mjzpwcca.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qdjpgysw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tccabsoy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rtzbqkwi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2okttkbmi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dchqbfuy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2rswldkag.html


<!-- 参考信息 -->