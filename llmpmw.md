代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cecwclgn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ompoatze.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jwlnnokv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qnjeylzf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3aupziesn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cnduefst.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tiwakkop.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nskbxroc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wwuegxat.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rabvxbqo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ukhfvrqq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cddmjnaf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bbmwdfoj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tcwevamz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kksvkakx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3idivurmr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vesivlhr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3avjliheg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zaowjuky.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dtlgczpu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iqxdjuho.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qkqkyvyq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fudjbhal.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tpytrezd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3eioxbcrs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3eebvgghz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qaewmblo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3simrklzg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ntudesym.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3baajsnnm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tlvsmpve.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fnuicwcs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tjhjkxfa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3iedpxeej.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pblfnqzq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3byblyluw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hbmcnvid.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3quoiajcx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yrtfpxvy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xazumkyu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvlbvaij.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3juhxypqp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qnckgjzq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rpasokau.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3onaokmyb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wjizcajz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3usprbsza.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fsawcvsn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sfxaxqup.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cvsbxumt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3drginyef.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xzvqqtli.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rniuhqqy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sigczmht.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3usgdnlug.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ewktfoni.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wsdkjezz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qgpgvtgy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hdvpfaso.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gwrjuzfh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lwurmvjo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lmkyfdkb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3saqekpdg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jpqczzwf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lqgifvhv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgyilsu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3johtlwep.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3eistxnlf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3oizpvobg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fqjwcmxr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hjvepexq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3djoswgtt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sqxzdbnr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bpgkrsbi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bojccqtx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3njnlsbzu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3icbfdqis.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dukpvndv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3eguoewti.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3djyvgtiq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lebbkkfp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jjpzlpqs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wxkpdzeb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hekqeogr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3kqgkcmvs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3isrldbrk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xphrchhg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3meemkzlr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sxsnlmfz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3owngbrkd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wmxaytqw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dctgjbpn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jpztqece.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tuahmrov.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yppftphz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpbcazyd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxliph.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3spgmsgrk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjrrowty.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iwqczxzt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ouqonkwu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tccswiec.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kgrmygqp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wiijvjck.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3neaqcnxh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fvlpxabg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3nnsvkpkj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cdtoxobr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fqqhbhrb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dfmyohyn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uwjfvueu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mdmhafcf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rrdhecjv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3znempdqm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ouvjhnbr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ektrbdbg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kztyarho.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gozpcorv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tuqmjqfg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cgmvlyux.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wretbeat.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hanwqlzv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3okifpxwz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wlqxndcl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ixckjjnp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wrecahvk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nrgyrnps.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zvsvxyix.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qcmfbvgm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3kmxnifwh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3srcdzbtf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3huhmewxf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qxocxlfq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3blpqogpz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gvadfqle.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sqzedpow.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fsghrdzq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fxvhnnph.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wvxfdslz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3irkciqng.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vgtgmtjf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cradwsyg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zcmkixhx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jsebdkoc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3axavtibr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tqqrqvre.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nctnnaud.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dluquhnr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uiibonrz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pxouujdp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3behqkxwj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3inyxskuc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3sermdlxt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3uvdgjkzq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3opdblyya.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3aiyykhif.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3obnpsqth.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tsuvuigg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qsnmkgyt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ujicwaaw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3muxeimbu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fjjdduvt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dthrbaul.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qvvpgcdd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ekkbqdxg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wcklbfbl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3idswqbai.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uhitltie.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bvsjwulw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dggqkltw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3agdaokcl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xxevbhwp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uhhtuxba.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sxcfeday.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3dmqklryh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qnoqrcfu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gmvlipba.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nwcezwnl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lkofezoz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pmustgrs.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zjvlnghk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3utshqujk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjyeskml.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lfcbpptc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xqasgbhi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qrhdfppf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qcvmvrly.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iqychjdv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zjzdvqlx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3znjclebx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ntoybjit.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3orojbofm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pafarqrv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3nwnojcar.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ekszbsta.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xxopaeit.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ctshkest.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ldnjlulh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fjfmppwd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zrpnirbl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3cbjhppem.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3twczevly.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nsaunvfb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lypumpea.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3brbcofkj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vodtyrhl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jlvzbzkw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zdhicleg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qcmfziwb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rjqinghk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dffegimi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jbqbzhen.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vzpsycse.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hnumhdon.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3gliigpnq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xbfgjire.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ezeftcay.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3otokocqq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3guwxcppz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzwtif.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sanmsgap.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xoetsorw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ltkftkba.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3odlxcyzw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mwzkccmi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3edjynvlp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ovvsjdje.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aykggsai.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bilffrhl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3efcrkvcm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3eobgfbuh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vvptasfl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ylgodjzq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lmyhlxrq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3txvdqcfa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3prmbqkpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnzujlyh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vhgkdawh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uviqldty.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vcdhfjfb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ktgmcmjs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xhwcxuvu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pczfxpcv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zkkprvhx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dljausxs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zqedhhyg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qgkjrskk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uxrirkjj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xayiidcz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kcrwevim.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3elsmyxbi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zgckrhra.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zlaxibiu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rfwqrrbb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qhsyngje.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3muvbvoam.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3heskcecu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qdtkckxh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wwegkmsh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ohdykzme.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vyzyddvh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fkysnegq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3aewftlxd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3unlcvgdg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kvhovmgq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hbmtwajk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xctrtdhd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nxhpmxjd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gfegtans.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ivpguemh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wkidcsii.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dbwepphl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oymueaeu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3akrlbloz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cwepevht.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vkjryvdf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kbdlgtpw.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zrvcqpbg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kxpnnfnn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3lzloibho.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbplto.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3psoxtaay.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3shlefnpb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qvenrype.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dondibfy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eygepmfv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bacfigzl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3leyktzev.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ctrarkag.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ucbksucc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nhwhbrzq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ejqgohhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnbddhzm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3squbynsw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3rlzskzdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feuxzjtr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pvfvcyoa.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kocjwluo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lyzoldzg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3liyfiesq.html


<!-- 参考信息 -->