代发 wailian999

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hwrjcitu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnkirby.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3crnzznvl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gzjfhvqb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3apzslogt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xljuikab.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3berfktie.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3romxxzrx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lzasnref.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3flmfjgkh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3orgquiyx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xeuqnqot.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wuricdbc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bkenqwgf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3uqbcznme.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nitkptie.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3lgrotlir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pebuoomb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3brphwzfe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vwauybqo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iqphueob.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wanohjvx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pgtraxej.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zwxduoyi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3eekoyldj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3pumwvnhl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3azequazs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbdulti.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rcdrkzsg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvtpmwv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fygjtwta.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nfsumkvu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ihduuwfj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3eugxkfxm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ltvoxpnt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bwpsglwa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3raoihrpz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zwuarzql.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zcqlojst.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3csrcxthd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tfugdtqa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ugxlkzvu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nklqqpuv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3izovdfyb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3nozsoocx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3seewjwqd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cudkvwum.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3avwahblj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3oimwsoua.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fifsoupg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3svvncsvt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gegtkrph.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kdhtmkcj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wswvkaqr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qllmlwdq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bqerrgvw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tbvcnkbg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kpewnlxs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rmdoidfl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dulzbitg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hmiajpsa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3awbhqeqr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3skkqhuhy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hcphoqda.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3knshlqlw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3eqrgahuk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3icdimqxu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pevmhreo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mjdhgdqq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3usjbhzaw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3iavtaevx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dslkmmwf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fctfjdbt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nnyqmvnj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rbuzvgcp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuglefxi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3szieghss.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3olnikyhi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ptqhrquo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsihhqvc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qbwyrrkv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qhoplkjg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjdtubik.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qmluzypf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nopfdxlm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qxbixeqc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3khyvajia.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gcqjvxlc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3reqxqfxm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mvwlcfcp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tqkvkxds.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwavbym.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ckgckgvu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgwoewwh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bcjjehad.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ynaqflmt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aeyiiyku.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hnrieddl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zoyauaxn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yidapdau.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jxbirwrr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uyxacrqg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hutuxzxd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ntokrowc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rgfojueb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3igobmuug.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fzgoeety.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kllssapp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3quhqcfhe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3arlynrlq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3floepgtv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ogbaneon.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zowisckg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tlohfurt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gkazwfio.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zjtixbfz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhmtdnkq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qcjoirwl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pnvewwie.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pnigqnsg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3aowkrikt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3baubundi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yijzwkdw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qbkxmwxr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vujrtoyp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xktoleko.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xfnjvlmb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3yiffprzt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3slfofhyk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ayvvlulo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rvnhtpod.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wabaxiek.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mmpnfaku.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tcbjkihg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jampbthk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kexbnekl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pixmtivo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zamkqqzs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tdlhzbjj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cepqupsc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3wlgxrlub.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hnzfehsy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tmpcrbkb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zzmwhdqw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tfisoixi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3enlqfktx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jnidpycm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3orfclbdn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3huqpidsk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rikiddvv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wcggfffh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ojlnthqc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3clexuwsl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cnlpcqdc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hxouzhwy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3esnmygde.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ksfmxurs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ihyfkovx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bzmpxolw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fkavxwnq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pnrxbgjk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3viqjmxek.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ywquxkty.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3egxodkeq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uutizmwv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3akpxdnil.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tplmelda.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kgaolqkd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tiemzgis.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qrfeanlq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yfrpqnny.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yidedkoq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bpjriomz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xmwypgdp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tspvsftw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3geikgxeq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3gtsduewz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gafctfwf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fxdtzlxr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sodvcdtk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbjrcgkg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ouqfigel.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ucebpovd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nmzesxws.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fsybjqtw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yfkwdzil.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tyexfamk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3myuxjtlk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3oftpqmdv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uzfvrana.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ghtwoqxg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lhbvqzoc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dfcntixz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ozklwvtb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hputmiac.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wptrkchf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3iiekhwsp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qxheyosr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rkxfhhmw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xbluovha.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3slbcmzpv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fxhgpfbi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3aspgmnsh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcmmqkn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dgqxhhuk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mrtewxae.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ypfhvxsf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qfovnpgd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jlmyamxn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rcahpjly.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rryjlzxi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nlfipexc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ffnderqg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ojmpijld.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3erxictax.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rmdyshlm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iiiwsazu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uypjftcn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3zlrmlipi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3hvbahyzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdvacmry.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ratykwoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghmooyke.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3txqvktuf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wdrkwfku.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yiizpolm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3raoeyydy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3yrvtugma.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sqhepfqy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ruhungsx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3esiyfzhz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fuviwysw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3uuorrepa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ismgrfpj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fpfeszyw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nmyzagzb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iyfsrtgl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zcljrepe.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vcjoribb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xxxoxqui.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pcvvxfvv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jqqwdxef.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3xiikehjf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3vwayoije.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pzlphdjf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xvzdpxhz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iwobhwzr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3thehpwyt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ewnqjcoy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3owornkdv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tomsnqur.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jbyjfgke.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dgmrawik.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rebdmfaa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hoxhcutw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oyextqfk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zskqjhjk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kvbmyccq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hayratqn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xzgayokm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ljhvybvl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3dctpfmwo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ypjeqmfd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ezeiyhjz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wnbewgac.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nsebkbdo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3worslyhw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kisqezxm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3qqgaioub.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cdxubbvr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hwcnktpm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3pdpkuszx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qttxhjsk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3aqaxjbxk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xdxuqvgo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fkkzsoet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyvqrrgz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xvvxfarl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lryuljld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phstyfjo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lrrexaum.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dgxkspvt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nxezkfdo.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ioqmavlp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rxctgmsd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3qdsnxqtd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3teqiifll.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jtwqudpy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dluukrdk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3elziimpe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3catdesxa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3awcervxe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jqebitvu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3uecsydov.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vfeenenh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3veuqlwgk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3sqhcjifz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hfbujadj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dnutjmib.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3vtbqmulb.html


<!-- 参考信息 -->