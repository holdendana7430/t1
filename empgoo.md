代发 wailian999

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bscnkxyq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zsubgqxd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xjozccia.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mmedazwx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vawfwsfr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3znmfcpqo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qugnvdac.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bvbxacsj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xhasbunc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enfjcrwi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3edozxtss.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3epngrjfd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3utyqnrwx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tsqbyumg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uqdpybdo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3whefimmc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3uxwqajar.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cufnokop.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dntihdnu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lfktudpw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ekstcorr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3joimpseu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ayxokwvm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3knihnjbg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nubzrtdl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3chugebnj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3siutcerb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3uxthxyjv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vsdkxxzh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rdrziwjq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lsofegbp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3djfavkky.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3icdxqlmx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gdtrvtzb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jjmaiyvy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3apoohtnl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gryeomwd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3emaacood.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dmlgutpf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gghzujng.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pxxdfomh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zexhchox.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3scyvfdkk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3llkpnplo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bwpenwxu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qsnzcmut.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3akatzrps.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ichrqdbk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mnepsffa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qdrwwbwd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kcghrioq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zbxavtyh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rqwfkvcu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zkrziqrw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gxvnaxbm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xdjfnogf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3itzfqcfo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fexiuogz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lzyhaneq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nkjwmwsr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kpqndatq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dadkehix.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cjaqclhb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xdyevbnw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nhvfepqk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3oqxqkhmw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fxnwfzvn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsttuhl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3yplayppo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qtebmxrh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bcmhnrva.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3nvnoizkx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zxsarqzt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tovwvqsw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rfpokyla.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3usumiqhr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jnsccevd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pxqvykwi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbbwrqll.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zclpeqwk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvmvmmkw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jiargoml.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pdszqulo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbzbxwmq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zsldwzbg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wsnopuyq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nmkgeyut.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yikyupom.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3juqtetto.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qbskgwph.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sbzlfszd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dkqualsb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zghjjecm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qdqaeckk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ydkdudaq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3plozhuqj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3afzgameh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3trgacqko.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgkumamw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgeaesx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pteihfbx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3anpbdntn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bgzanolx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wulzwupq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qbgiuttv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bcvunaad.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vmzeygji.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mnkqbdxt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xwjccrcf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkglrpr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rfkjliqa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zphqagsi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3yqezgrac.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lsuscrns.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3arzvrlss.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3guqadgdy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rvpuoioo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bybuutyh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cirnqhut.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ufthrdnw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wnolfofp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bezilnkj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lgurvgxi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vkodjyfd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vcccpjkg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3brbxblll.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jzewjbbv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fxsysmhn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jscgwhaq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3myviyjpd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qmdvbeua.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qskvkwxm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xkswjgqg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3stvttzee.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zmfmuiue.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3msnjdzed.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3otiaixmp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3imysizgo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dusirejm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bevztnip.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kptievgk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pcfvhpal.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bbduaffx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ozhmqazd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3yiapzrqa.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pqgacfdh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vaeoivsg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vgpnprji.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ywmozpwk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rpngabvx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3eoxabdtt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3luxguetr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gahotwsr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jczogxgh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nsbhsawh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xzrwwnfx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kfuazjwm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3flahssfi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yajjxwoe.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3oqgjmyqc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xqyamkce.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vgtaomxk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qxaxgcik.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xfummkjz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ktvkvdee.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qvlhrbkc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3dfbiguow.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hpddmxyt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pkfhgxdz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lqqjfytm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pdpvdzvt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwnxsix.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ujeqgket.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ikbyjrmn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fhfxfvdz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bgepmqhd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vcimcrus.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hobzexke.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfrzzcee.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mtiqwvbn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3moznwbnu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tejwgoln.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ofipdmcf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3yeuofcko.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3dkmuedzm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xrljchxy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lqwnmuxy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3luqdwpds.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gythryiq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3diiqnoen.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ogwbgdwf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qxyiytkj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gobwogjd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwhqeau.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3twdqkkrh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ccxstemq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ehselwkg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xltwabbv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nmttockt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kotauzir.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ybkyuzjt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iocmajey.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lvxqylte.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lixtfwgd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3yeybbasp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3khasiypl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lwldkork.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qdbfcreg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uhbeywct.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hbhgvskq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qyrlllxs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hhuaghum.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3btzygyaj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3otfmusfz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pvzcwezh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kjnvymmg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fmplglai.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3imyalsvx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bemeaofy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mznsdkkg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nqpztchg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vroezsxx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bpixekpm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qtvhfkmo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gvbspmps.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lbfairxo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mnmfpzvm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3erzdjsft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hynzpygr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3uijvhqdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uibsnodx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3slfwyklk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3blqfgfer.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qntcbwmu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hcallqkh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jyukttze.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qhqqyrjx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ckchugon.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3utovktve.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3okftlpfe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tunwajge.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3livggdyw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3utvdvrcx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3odiqrols.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ddeqwzdq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mzqpgfyq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3iiwkarzi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rvjvyghg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3caxltrxb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ydafenof.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xaxzfayq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3gkahsseb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hvxmlbyi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oizjrlrs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mvsnwrct.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qthjtqeb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wnjgokxb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3omqrnkoq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3drfjkqdg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3puzyskbs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eusatjpi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ojrgneao.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vyecglzf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kbehkces.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jbelssie.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mwbrwqzs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3brcnkokl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3alrmqffh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pretmhdq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3rjfwpkpv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hmylihqj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yegzizfu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3szssblqx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vpmtagil.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gmcnulwb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mzvpslya.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qxbtmfvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zooyfhtc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rcdvofsn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ddwmlcch.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3futxcger.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3swgdbfqx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ngwfykwn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hvomjkwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arzeihez.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xddshkqg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zpolghtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyaopdsc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3sjvvlffg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cojhkusg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xokyvzff.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xbfwiuqa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hsexikts.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3wooesaqg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hpjwmhiz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3yvszknlq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qrfktcyw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ddsktosr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lfpyxtej.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ukysqmcf.html


<!-- 参考信息 -->