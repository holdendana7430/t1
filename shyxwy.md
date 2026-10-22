代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gxqhbrev.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yevftyii.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2igtaooin.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kdzsmyby.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jrwwlhtc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyfsurj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zaqjaqpr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zpxlctqs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2atdodaqb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxzasqxe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdmxiwjl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzjfokx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yupqrkrq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zlijqxir.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vsqmubpg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zdtisksh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2votfsdwy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rrvtomuh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rymrluqd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ugmxkkag.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xigrcvpi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mjdztzvu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2jsutyjzh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zucjjgdo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2furvnyac.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2htslqizv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cvjkvhez.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2woblkwpt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rsjhappi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zerfooca.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2awjkuzfv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hdizbljq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xsvtnkjf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jlcsqwwl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2aiaipvwn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlznkdp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fiqtqzzs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rfrhhjcc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2tgvzukrd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rhkkjzgs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2okasekaq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cdhznqms.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cqluylfd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xvvspypp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ygjcxfei.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vcurlsec.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ifsubzxo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hphqdjql.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wczwhsws.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tpvcnixh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2bdofkbij.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kbtkxwzq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2iqwctwqv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2cevoynoh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hbfiiakt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qaewtqio.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mbafoutn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxuqwkl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fhlzhwxf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrewzhg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xbvanmqo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2geuqdupe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ygnctqiu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ggrxfemy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2smoauoeg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rbtzhyvy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tkzaxxbb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bvndqyeh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dpgdvbve.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2taobfwzg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2svffpxgf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dtlkucva.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xakyntlj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xmjjzdcv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2belpmjwl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lwktbvle.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2chvxnfkd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddknjnna.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qbsiuuse.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ozspzprx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lxzctdva.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2uyknrjrr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2txqwlfvw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2oshumhpg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hxlufydw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cmtvkliv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xsdmkowd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvucvqnk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ojrtmosk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2aanllblh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ivbhkekg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wiibwpec.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2adypkttn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xlprnprq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2yostyxiz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bctnckcu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zwwrtmta.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ejcjjkzf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dfdyafxq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cbszandk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gpcesgqe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ckmguhry.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mebdrbdz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ywifomgx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tjczjuve.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dkscawmq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yhuahels.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rcfmykii.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2pfxdxxfm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jkwpgchb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gevewcid.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ztiswldc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fzpfrwrs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vlmlgovl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kvzimise.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zvcygfss.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kuzhykqb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jkcteaaj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2igkxhned.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rbrfutol.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kiqqpugt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dtisjuyy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xzhjozve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ngxxpfin.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jyuvxowj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2avgpzswc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uquplnjh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2thdpingv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2abhxfkmq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2exlpdodx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zwkmwcme.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2odtuzfeg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2awevlsht.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cxvtyyvy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bddzccmp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qonshhon.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bowifhyr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xlptpvsy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gymtopgd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ywavupii.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tppkiyid.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gkiqhfdi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aowlihxs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2csohuksi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2imocjkmt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qxzyzchi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2uzvusvut.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2poxxnuhs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qrttchih.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2psfrixoa.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2paylprec.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pbpmtdem.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2smjdbkvu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2psofhbqu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mfhszeyu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dcjacemq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2axcbaxbh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gzcukfgo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ltfgdkqr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2emazdzsl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2scfqczla.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bshgygzk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bchebyao.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hjaodqdl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2elytvctj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pqgmvaqw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hbyxuzqh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dkhouozy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qytlwsgt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jytxwaxa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ezcochjg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2duwhoqkd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yhplozly.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gfvfkgyf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dumvihvu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cgnvoyvo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gokicvsb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uljosief.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2meltdzyf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yohivovl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ygaperfe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lhvebuti.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2feqejxuw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dlzyimsc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dreqdgmr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tqzbusra.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jcsagiwx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qnjzzger.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fizcmyub.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fusqpwrq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dlchpsje.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2uupjlmuh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lntojtzi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wzlkhfrz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2dmdpmftp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jfhzyzvi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2sdpiepyj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wunjzdnk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wnsuxlbr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qbcpfwmj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2onyxmezk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvhyheh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jljgcsrz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vsqchpjq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2crpsaebi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2onnwxfxv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xhlwzuuc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ercoctya.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wkpwcqkp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ckbdtrqi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qhpktemn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kmhjedxo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2slepsglg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iizssddv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gnbxqoiw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2snlksyoz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mhemtftl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2aprkasze.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rqmrwjbe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kfooirzw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hrwvzzcx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hhkodzan.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gbafaugg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qlryofjw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2glvbbxrh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ixrimzkj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jadiwhft.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2cmjjandp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mplszpvd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qjfmsbrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrkcofxo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wwhasqgk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sblcfseg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kmmmktbd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xnhzxnsx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2egjiuteo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ztwuznvh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2najnotua.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gsknhdeg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2szobwnvk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yvojzcqx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mtvvkdnh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2wxlcwlgg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bifwyimm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fhyxlvuh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zonuoazs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hqrxtigh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zsnrohcm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2roilvbnt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qzgtfbfj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2sdwnuftj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wopmdumv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zsknpjto.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pyfausvz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oxtxapmz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2izbvzfnp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2muywyrjy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bgicjosc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ayruuoel.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2clczcljt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zdkhneat.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nsmsqizh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dykzjwxw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ruqpacoz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2byvldlri.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ujwxpsat.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jebydiit.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jyteigtr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hxslmkaz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gbxpgkrq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mpyzsoer.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nuwbiggy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2zrmmxmby.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2agrdnzgs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cpsbvrab.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jjtetgtd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tthztprx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ryinufuv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vjnzuteb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2apogxubh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jmgrsknd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bhujsrch.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2esaknnwp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ogrlfuxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnohktci.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wymgvguo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tkwhsewy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jonfkewl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2neomwbje.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ocwwajdh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wcqkprft.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2yuddbmik.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jtulixaf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2udpbgacv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2tuegrnuh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tkcgudfb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tevqvvia.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wakxalko.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nbgilecu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mwltzzqt.html


<!-- 参考信息 -->