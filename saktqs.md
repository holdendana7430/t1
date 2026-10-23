代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3scvcgbbc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3niccpoki.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3tvcvyiuu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3eorhcjaw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3brszqorz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tfufgmpo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zdrjswox.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3aiunlojo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hleycjrw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ekmztrsh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rmehryaz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wzomomrk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3eljyhzbv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3atziuvzt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uahwdyta.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fefglvqz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpepualh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqvpqvp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3oevhrmff.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvmiunp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3tnmttpoj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bspdkpac.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hqcfzfzw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tqeuwjmo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3blgdvzhr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3isukfqnf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3piaqqnat.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bnphewrd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3flfqsisn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxruiuat.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hvdzuhdb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jagtkdjt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3oovtpzkx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kgqlcadg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gqejsqtn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rrqryiea.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukqpodzd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3egrsxsiz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rrylkojr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3etmjylyu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fkugbauj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3cprklxwv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lwatepbc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3euuvslcx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kshrxcjk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gmvbzjtf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rgdoeqaj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fibnxwbp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ttxanegv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3advuzqdi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kthqxvvd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mkcaswkh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fubppfwt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3adodlngi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mgxzsbfx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rqurswum.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ycwhetls.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3sjadkbih.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zywkjtai.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vcxwtlga.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bcdtlznr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bzpvhpng.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eieitiib.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rczkrogl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3jmpflibn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ulpkourg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3aeergwar.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zhcuvqyv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tmqhspxk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cpdmvlzu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ihfikcnh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgyukjzc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ejsodldp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uypfyamc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3uufkumdg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hqgmghmz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tupbpzea.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nxpndlpk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fmmbnehj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xieaucvw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hggyliia.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkqfizyr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xynvxkod.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ywcsqxmu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmxjrzms.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lwladewn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sqduxdzg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imjjgoly.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qvkztrav.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qpdacxdg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bnfamkpx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lddpucst.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jxxvglvg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ekwygjcj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qntzputi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xzhbhlbj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3htrajrzk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wpdqwchy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3noeycotx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qnhiaaih.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ysmxfklo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wswhzgvn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmfhombg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbwijmhe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sevbrjqo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hyflfnbx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3mdpxebuu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gwkxafpb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qizwicus.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3htilmizi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3irpjbumo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3navskdzh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pwrqdtgj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bglxpuhf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tdbjqtrx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ctunhdrt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yctvastp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3kiauwwjd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rhgljsjy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qknxppmh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vnvkjijk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3loldxarj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kmklvmyc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cybgbtqa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ajqilqxd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3blhqkzbw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnnoak.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3guryhvny.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3cstygbia.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3iifosjjo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dprwnzjw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3eybwspkq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hsynrtok.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xopwgsyp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cvlkjdbb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3onnlcdpr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3odapnvag.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ucffqusg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ophzdtgo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xtskspib.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vrwugpwn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yvhwwxos.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fgnjznzm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qkwsvgli.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ggrvpwwt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3aqydojgr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wqgpczvh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hjhzoobk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lyrrolye.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qprlensx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lcagankk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wwjziezg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bdgyakux.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gfefkbiv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xwqpyiab.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fwwhtyad.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hnwgpbny.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ujgfxbnu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3trxlamjh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tgofkkfd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mwpvgobb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wjrvgmhz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3obtlzpcq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3zjxdatga.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zkowcimh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bjjsmfcc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3swesvlqr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ernwpkrm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zumuuzrp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kyjyapwn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mirvgbbt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynudotpt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bbrnbupx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3eitawrug.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rsjgqrpk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cyrnoyzc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3izyzcdlt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vysigpdw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3agyeatcn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qkqxxjsh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ijjubirk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tvhbrzqy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3szkpzwlp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvqxjqcc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3phapyzwc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pewcupiu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3prdhppdo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nkasgquu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3btiokjxs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3sybclout.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ladtymif.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pdwhyabg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lrnwfbld.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ihaniuzh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zjcqsfek.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3oupswdbc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rkyklulj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hucopnqv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uvinzdtw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lpvkcezw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ivlsvnke.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qtwpwhyv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xecdafhf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cujikgdc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xryekant.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ocawcfrx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pbrpdkkm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3arlzmxru.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3qpaxtxju.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3euyjddza.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xypkhigw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lilizurd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gywexjxj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fwxiwrme.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3druwhpua.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nerxjpjq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bhvcrdpe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3semgpsud.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dxbjpoll.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gauudxfx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mjbqkapd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jqwilrrh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ybdzyzeo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnvmvmrd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dvcinqpp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aoejecoa.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nzuzxmnq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3romphxuc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ruucxrfp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qfdqlriu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bztbpttp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ojcsswpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmdiuilw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yydajplv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eauyogil.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gmxiodbx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bedkmqzc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ezedbjau.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3flwaiwrz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nygqlvfs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3diaplaja.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oyvhsocj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3teghiyjf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kagxaofd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rqtqesdg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wsmjunpy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gkkakoqp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nyzuutta.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3csyvjkop.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3kdxyzebf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nnmejfep.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qwypsgzz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xrosibob.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gcvavrpn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ckyfycfz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pncrhmpk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vfuadocm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3naylhbpd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ogewhbnj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nazvgeug.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ndebtdsc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nauetgkv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rwokqfkl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ibhcjafq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hyqbanim.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uwkflqct.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kxtgmhtk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfgnqv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wczenbbf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pxivicuf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3vcylshka.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3amqiqnly.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dbxnmpev.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3gzgvheel.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ppagnmqt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3orrrndyj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tognhtol.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xteuuqxg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uscgogsh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wnbxvkkn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3tfzxrrzv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kwqapczr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gbwphbpd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gytdnenz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3jvmvtlyk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jtnyzvxu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3llfmekgo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3lmyhbypl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnpoixpm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3kjaprrbr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3rmzdquvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxzkxecc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3fenhxsiw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bodxqjxd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kycjfqct.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3jpgbywfn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mlxrwpns.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bcvpsqij.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zkhjoibv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3keghkbjy.html


<!-- 参考信息 -->