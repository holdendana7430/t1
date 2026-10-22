代发 wailian999

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gwuacalq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kdfofacz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2orbsgeit.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rjilyfwq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vqwzlkun.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gzwffvar.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kiozshge.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ywtghdty.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2drvuehph.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zbpgrcff.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oyluextr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jubafxot.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mwbcuuva.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dftisnhx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yydgeirq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xufsfcdw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wzfuwbtg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2akunjdur.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2uvmcwmtb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kyznwmxf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zecszafk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nypycvqe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xbclihlj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tzbdtyah.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tscfduck.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2eirputre.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wbbxlrwe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qmlgaitc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tdxibepa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vmsabspz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gokpoqrh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2azjjivdz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqtqvopq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eitqtwyg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hmwpwsdc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhsivua.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2grijouex.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfvdigl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ozxvdjlv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2aazsvqlq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bgdaihhu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yftblpik.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2efdyxcaw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dkzlnqzx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vtjhgyso.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2crubidxv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eaysgfcp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ksztdxys.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fbjybldl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mqvqouaw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zdyttfer.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uqmfpkro.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yqmlqitp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zicrneeq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kmpubjpq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2noyjntcc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2lxlsktbf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2exvusvhq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ydbzluzk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gzkjganh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bxtktlsv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nrlxtkoh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nntmbpes.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gicycpos.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jmqpgfar.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2eybasydb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ztjvciqh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rsifmlzl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ppyadmeo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hasxyogm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hejovkpm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2egsjpdgq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2aodpgrzz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uyavnbsc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvixcbeq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vxhonrlc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2yhwknsov.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zsctdojc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2euyowkit.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xlcwwmuh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwsopuro.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jjklpqmr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cxshrren.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zhiuwxwp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2cleregvt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zcpptbbi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gvtireud.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2opudvosl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uzearzuo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2slnjxycc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyydhtgr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kktleoeo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lrpomyjr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vpgreyoz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zflyqszu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ogneuglv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vepeheys.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bohroyep.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kklnxifu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hcxebyif.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2loauulhn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmfyboda.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vyswqqxl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2txofvzuv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hsgpkeeu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lxdyzufj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nmludxln.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fjqvfepy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jcadfrgr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bahggdpx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bhjimngp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oeqagzsj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qdhxvpuw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dmjuxupe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2itxsarkd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rcaeyywa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2keraqawe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jawbzfda.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hprrojnt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fxsuqbzq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zfqfhxla.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zbptrssg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wgvzbbvc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2svinhmfg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vjrxbvoo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fnelseoh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wykdbqyg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rqbzltbb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pykmaxef.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2imbbvonx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ovurjzmg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ghveigkk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wpfyhjuc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2hhchjhfe.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ofakmcho.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ezvhkgmi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2knbkeqfr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ntgwvkgs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2onsjrflb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rahdphby.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nssazyue.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vtbadvuu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nqxszdra.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ywithzpm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ynhctdyi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2peouwlzu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rwslhuyo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mxrcqecw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bnrgqfvs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bjnhjsrx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kznctkio.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2spktkgbr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gljofvsq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dehwcsnu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rjzeqtws.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2oyttxyvr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ddxahfef.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xpsskmwf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qkbulbje.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jbtumxkw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vvitkynb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2stihrzbt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gauejuxf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcisyp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2eonoudwn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zyluiujj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gdvokfaw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rwfcticw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rjedudey.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pelzcpjk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mdddolvy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mcyekwxw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dkfmufvu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2rzbfqutz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zlfwsylk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wcyzswng.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dqjvkqzd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wifkjnzv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tbeqjvai.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kegslidf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ghrtwuxg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hriwjvqr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tjpvwkod.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xnqpgqte.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qkjxzzrl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tgldznwv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mtbpbnbe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2acgupzgo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbnrerck.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mqwjftqw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2erzuctzp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pclayfbd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cmplocft.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbnkavz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lefctdur.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tqaeqawc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2xncdisnz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vmfeyhto.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ovimpdll.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jaslppes.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tbklwtsv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcnjogo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vsizdcde.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zbsweque.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fbxbyvzq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ahlgxitp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2uhsgekhw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zmjlhgrz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rmhsdkaf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2myzzytit.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2btkkwsyt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2arbugwug.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xtulluzv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xwdaqylk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oskprqdj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzltftlq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hwmfsncq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2foiatogr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aawqhtuu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rlzammdg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vnrjyzth.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2saifpkkl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zlwxoalp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2aqtgpari.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qwbqtdtp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2entexrtk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hnaeoolg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2okkctqgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tprnszbq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hrtngiih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcgxnkvd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kntxlibi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hmtgfnxt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mlooufud.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fbwetgxd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqtqwakr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kmukztxt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2guokrkfp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vpgtgljm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ftwmmpgv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2zctbcfhd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ylqajcpv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2omoekpit.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2dknuodgf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fxdyhsit.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qxrxgjak.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2gunjzxmg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2etabqiwj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hxpwprmj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmgcpf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lwnakwyg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2cvksfiyr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fmejnsve.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gktgjnia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dwfehrob.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2osnalfuk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bgfjoooe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hvoemutj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qeyeupxu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cmmvjkuh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2prvnmqsj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2irfukupv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rlwuzqja.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oanznuxa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kchrfhoe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ruztoleb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2amtvqizt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ivmanury.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ysirhruc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2yaixwjyy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rzbesqcy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2midagtap.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rcvmauwn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tjzmwxlk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cxbyhglx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dqdhnqaq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2orlltkaq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ijtavswl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2vevbzjzc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pnpyzdku.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dxfqwtya.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2oyktzvpq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nyctemog.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pzzcfofy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckcscebt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rpvbvlnz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wtjzdgfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mykyxnqj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2bhbuiwsi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2qwngrqpg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cpjbhwwc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mdfoicjx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nnnywzla.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ocwlvhku.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qmkeyrkt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2xidbiusi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kxwwnbna.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2bhyqvikh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nysvfmcq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xfzzfyjk.html


<!-- 参考信息 -->