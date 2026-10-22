代发 wailian999

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mgrbbgua.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fjwjqniu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ylcsuxrl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sdxswmzd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kszwcsff.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hfxmpbbx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jncaocrx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2abddcxlc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2loxonpvk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nocluirz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yaoximae.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2unpzulms.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zsxkeqsd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2iobuydrl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cjsurpit.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfltfxn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ylpbqmfn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xwbleutd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qaigkowj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vsniyfqy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2krmqbncz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gtswqfxl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xlaqhxhs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oxvizeyv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wgbopilf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2daqfborc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pryafkjc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dudtzstt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tlladvwd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eljkzlrq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xkhfxmji.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bhpbpwyg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vacetlne.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wecabwbx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jncaoxsq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rtntoyjo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qmkdxujm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yepcwjzt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2owctvnzz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wivhbhiw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ppuishxi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ybmmsazf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hvoaehvg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2uanignfm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2uiavwzad.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2afudqvla.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2asziwevi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qnbewffy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gizoidea.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yozocqdi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uwjypjyb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lywnrvia.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xhpjshwq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2szkoexoi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yqcfydur.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2chmvoset.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gtmooaxo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ecpfxwrq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nxjnuzhu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2putcspdb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rlnlysdv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gnbawegy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nxfppzyl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2utbeypfm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rkgearkp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mxojijsv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tckhugtd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bixfwozw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2zqvdqkzo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xachapos.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sgammsmx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lojmxufr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rhjbanfs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ycdnnvvk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2omlikprj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lflmpddo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xovhphlp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gjkueuyk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tkuhoodi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2klynlwpw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2arkhisow.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rtkisbnn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gikcrkgi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eaawrwev.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gdwtapej.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2uvpeekek.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2okythufd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ruaadxjk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rvjnmivo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wlqefhrl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nnjkrqqj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qbtjbyog.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jplcuojv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zuyqsdxk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tzsxuqic.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pcwrhxfz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xlmhvyvr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cmpkfyym.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2abrkonsk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngyajtdy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bkuumaeg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2inusinsv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fuyydmmi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zkqpnxno.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cgnmxmqi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kbrcfvcw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hdfiyqkv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kurqjfqv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2asbsfjsg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ahrbsoej.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2umdohivx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2whurmijr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xymoybgr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qkpwaopx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gjzcwedq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2upwndeqp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pzkdfopt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfdpeqyl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2plxdimnh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2abjrveby.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2weytrqar.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2keqqhipc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2sutoxxok.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rrwchhwq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xtnteunk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wkaiburq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tntrmlxd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gzxobykp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2axbvmwor.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bxhqzrdl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xmgwkynf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kmornrnu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2meuaazxk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rszlfgyy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kzssajjv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tzexqzld.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qxdzhonj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zztpgxsq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jckanuyt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2tfjmzzbm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tstvugek.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xhqgxuoa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nfbukagp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2uyurtxgd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2upnwyzye.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2foakktef.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zfrzhwqy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2iogcxmww.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2seilmizz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ubofhmda.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rougixbb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bojdqkle.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gpftsbma.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2helgfers.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pywymhbb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wzjsoxzb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vokwasko.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dsajxfla.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2esfnijue.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tttfciup.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2pbccozab.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2phrgcynm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2npjyftia.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2flzhvlqa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ffavfvwf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2baegafcf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xaubtpqm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqwfbdx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cysuyedj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2dadghsbi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2yozhgtom.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyuityrw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wtigbkil.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2iseqxdwu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nabhyinf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2joswbwte.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vphikjyz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2umzeiwvx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kjqmpeoj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnysvhkw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qotrwyno.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtojcbes.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2quzcgukl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qbyrxgtk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gjvqzxrm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lieeusez.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wgkyvmac.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xnkbiwqz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dxufrrrq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2acrjjcut.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gnmvhzra.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2usbpikig.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xcgdagly.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2raiovqvs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bljdummb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vgrmfywt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mwmuypmj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2csvvpqwa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dwlfohbj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yztvptoc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lhecciqw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ilyfquws.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2upoxfcvk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ojpcjizt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tfbkwhuu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eeoolszc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nfzfkqzu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zauutsva.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2btrrfxnx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iklpwvgb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qbjkqmye.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2doomqerl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fmjkgbxv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2monhgyfs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2twyhzjkl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qrinfpdh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mdujgulw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jmcrjbvd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wtmzjlml.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufrreofj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2buuibiit.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dhektafn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2flqmfqtr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jelwtiyn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xlecdgle.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xvvikiaz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ydijccyp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xdztnamj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnnrxtsu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2uglaryeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysqzsewq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ogtspaxg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gpzinrkj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2epwdjrrw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jspctewl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oitiohku.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ppdnluwc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iqxrjzpn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2efvpojnl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xgtfkfit.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zzhcywtq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pieirthc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dowwkrlv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jnwtqhoq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2axzsqxpv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2inbnmjbh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fvecyixo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bnevlhnd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2rnrdxipc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hilgksgt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mrzyymdu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jtsekymy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cwqtlpeg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jkamwhig.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ipibfanq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tuerkcwr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xvkdpvqi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2adebdmqc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jykqmwzj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yfkbmrju.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cccpsfab.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jesaeloh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hbiyjxjt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pvhbruwx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bfogxnar.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ehiplmsm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ztzrvmgu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2byflrbqc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rdukzrbq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fsicmzke.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2knlscquk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2axmwcwip.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2sqlsumaa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2brleuwnz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lqijswfm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oclrhdzz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ktwkgvvt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rvtvuvbo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ashnynwh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kqvsrkmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kqsawikj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zpcgxmga.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2iorkhisf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2tqrsmyhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muqnwoya.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2fkznokys.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zqbtqrpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fynnwksu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2zvntmdpy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yvmfnsnc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2epcnnebz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2aewhmcxp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2evnngozp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rrhzxfov.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bcxkmspa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2whymviez.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ymujwcuf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zsxsjiqj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cbuvknyd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rmusmjup.html


<!-- 参考信息 -->