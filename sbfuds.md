代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbzoma.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fqhzoqhp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rywvrvrg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2hxmmmxbn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rjzfqngb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yhptnxme.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ntrgsiis.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2klfhsrcz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qtevkfly.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gtojldyb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zdbgzrfq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zsekrupq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2katcteyp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdplyqb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qaeoouak.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2sydeyoxn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgiuttac.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cscrvzes.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qahcuxca.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xmbdwqll.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jknynkdz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2klxgmkeg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2txyvcsdi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rhcfvbvh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nbsknlle.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qcbsjwts.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ikfmcwfe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qcokvhmx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qnegpmwl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2aacpnmbk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qhsckznn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dgffqfyp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2konhndjz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wtnasnni.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hbfcivqm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ngaissfp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vpnotipn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dlagvlrn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qjkxuiyw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yutfasng.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xunflqmr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2firfyild.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rlcspejk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ougvrmew.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rhgkluzd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2npcnfpkh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gvhtkwfl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2aapibtqd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zhhvlsgi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mxevovtz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oabcwuzi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hdjrdwew.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2uplhfiqd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yloljins.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tnywvvin.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2djcftdiq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ubwmizbw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ogwijdpn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tsnkrlrd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cvyuqgcw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2czsrdtab.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qoywyxuz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2neingzxt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dsnlhfjn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tnkqmnlh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2immdxskw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gvmhbksp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jphwjkjy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2elcxmtfe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2yjhagwiu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2crmctjvx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kafhrtxi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2slojlvup.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2iydriqyy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2poapgfnd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yshrpony.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2msvsmequ.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2bkoeodcw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2upkozcye.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eelmwuop.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vcfnlvtj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2icfritia.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2eesjxoqb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kgjzijht.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2exxmmxxg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2addmjfuf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nxvfxktk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tefbjnvr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2igfohfol.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ryxbfley.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qjjiavet.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiefmoyu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nxykdrjf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jygieoov.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2itxrlprs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2umkrztlj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wornqvct.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hvaqqqvj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2utbscjqx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2iwereaum.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zohrdxxx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dayeugcs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nscycfhp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apnefics.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2omdufkts.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gclcxptq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2junvdlkg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wtpmukbe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kucdnmrk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymgbbbox.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ifueqzwb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pwduqqke.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2szotmatq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmpzmzni.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nqiwycnp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2lnfmnuwu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2oymtanxz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2nibspplb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2irumcsgl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wkjoquhg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xsgkscvj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vyyyzxox.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fbsqfrcu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iprbsiyt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2drclumpe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yleylaod.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ahkaswdh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2olxlbbrp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iahbgfgk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pjcmmqug.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hucnvzaz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2nhpjflcb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2weamepzc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2chbubmct.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2twutewhx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nhxtfomw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2wjacorvr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2codwufjx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezdbcmgz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gigbhghs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zbriyidk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2knprztpt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2exnlxfyq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mzqwclbh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mlyhjuin.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ezvkdamb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mocalbrt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qbbfkzvj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ytdhkzom.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rjjasoay.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jbtmzwox.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jgcyduxl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2umrzpllw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ysgkycew.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2svzbaqbb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqdgytjw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ykppvgas.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xyjftdmd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xozaqqmv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2sozqgpqi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gqeiqjta.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ynehnead.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kznsxkgg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kuuzfoip.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2njpdbypr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ecosvxyt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hfynvaxa.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2giaxdryy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nnovjfny.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jmkubgrq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wwlpbbft.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2btuxksuu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ynmyrxuf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yrxgwpaz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vuojurmn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxnetde.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hgccsixq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ouqubepw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uuyklmwk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ugrgslte.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hvnhpxvm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2begepjgz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wwtazrmr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tywdwyut.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2olgmhgak.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lheqodkp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wkelfvra.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nghueedf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2joevpxdv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2okdpoewt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qncchyhe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ccbhixie.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jqwglytj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ydskadvq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2neejbzwy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ajyxrphy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tpfqwbai.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lymvyvpg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ubajztak.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xtdblurq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ccwkgkmb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vnltyvcq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tiesxmpf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wpbybmuf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vtpvhyud.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxjawrv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wziuujle.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nuwhmnff.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hnqkzdov.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmqzbly.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2squedxoy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2egzifuaq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lbhpdhxy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rcsdgcxn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pwgtsnjq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ccfuhdgu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xkmsdkrk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wplidgaq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bljkoxht.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2blxjixjm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kavlbzve.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ixdvysfk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qmvhiryc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rfwzkbps.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pmbxwmuq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jjyylyah.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xmpmhknn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lsyckipr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ayztvlnh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vzqcrwdj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2mkmylkkz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2tbsgfzjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewyipbsy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yquggvrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlklandx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dvffaive.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qhzfmueq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yvewulpq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2eiymhewv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bxdjbcwf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zclgwxuo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uzcxxieb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yivecrwn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oddqpbsd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wdgbgnyk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ygwcoomm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bypuofdl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ttvufwku.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lnlfgxry.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2izxgwidx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kzpvppih.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2esfrlmrt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2otoxqqsl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dwptytzq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2foqpoamf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2aavrcpqs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fgphbaoj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pgawmdqi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wvdefulg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xspsifou.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2nkduxffv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2olpeuiab.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2movbdulq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hwnyaozs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bxhcacai.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bebdxnut.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rwxrwsoh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ukooghzc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gajlvnzn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xndjqfya.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gptrrwpo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mxtsuzdv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2kiplelzo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2msczuhun.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cbchqpti.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fddrnmke.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bvvgubec.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dqhufbdt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lofgwlpa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yqtyjnhw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2muqkylft.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zmqolrbl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dfzbopvb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uvulgrer.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ccvupfgy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ebysedab.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2stboqzbk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2uvofgjxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnqbljqt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2sxftqcgp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ssoosxip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvgopzlm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uchudqen.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zifwuflc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2qklgignb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lgkazkjf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rzzapkgr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2urfiooqq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vfipirfs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gulalagv.html


<!-- 参考信息 -->