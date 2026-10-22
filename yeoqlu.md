代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2injmsjxi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2usobvyri.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tzgxwnoe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kjrskaab.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ckopqlye.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2faqupvhq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2asgvjmmj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ilkrfzui.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qfawfdau.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wprgtlha.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kfarxziz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gvbkfnap.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dkxokthj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2haivxnfa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xtqoicql.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2umkntsfa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ihoclyum.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dfnvzsdi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jxzojdfc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ablgercg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2aacewlcx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2goljbazh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hpnnsoha.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lovlwrce.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ibhbjyrg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ojjpdgza.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jqanpcmb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2httrcqcc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ounlpwki.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2beihhnsn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fafqxisk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyyewnr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jxbxswez.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xhvfudmv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qwxuyfkz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fwkksuis.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ryrluity.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dcxbvijn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iuoftfgk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nbuaigbg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2udzlyict.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vtwzubav.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gxwmkacc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bpjjkgtv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2seyalkmz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vvobpbmg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lyddztso.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2usevscgi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qeqzbtyu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2izzqmxwe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kkgtqnvb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vsatapaj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zmlhcvzh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2oghquzvz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nzbiyjdk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qakwpapc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2sngsepue.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2iwdajeor.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2gsglgebn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kodcevun.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mwgymmtc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2adscpnhm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2brwlukwt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ofufcpdn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gfonkhkx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hvglbjbj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2umnputuv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mbaulwjr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mkcitvcc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmvchat.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rqivezpx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2loturlpv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2atgpyvzr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2oynpsuse.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wtxmeakc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rbdyujpm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gtgtcmeo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zprgpjnh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2keltcort.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vzfetyvr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ptcuhlmt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pqgwcuve.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljcqmryt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qsrgemcb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2sqtbkkin.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2utcmhlax.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kmbyvwbe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hsivbhfq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nyvqksow.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xexzfevp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2afbcxonp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2suwispmg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2seovyssa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hjorfivn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kskqbvek.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hklyafnn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jajdadcg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2phaskeqd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nlwmmueh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2eykbakbq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2firxjjfu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hwgwceml.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fobijobf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvbkbfoe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nnmmqlvu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2raqbrzmn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jlldfdfm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2eftdwwjb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rxlpgzbx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2glakxhsz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bmfmsxdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uywledrx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ireyribp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2amzzfdju.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tzltxhuy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gflnslvz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vqvgqjnj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oizptqap.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zwmckjws.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bxfswkbn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qqufzxuz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gisabhxf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2szcqsrwt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ehpydvju.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rxgwfhka.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvugobs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nxaqjbxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kkyuceku.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ymxjicvk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tgbatxxv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2acboriip.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qzqtcpur.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wkpugfhm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ajeqlbus.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mwhehvwr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wbvoxelh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2srfemouq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2msrtyepv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnkpyfhm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wzouzcpg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kcijkrty.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rvbsrbxk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zgddjmyd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2oyygpusx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rwztzpqe.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bzcqwida.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gwwarsyr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ohyojnwu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2farpfpzm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qelxxbcx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qjwchfim.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pxrlyrxt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fmxjgopk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2glyygjsq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2biqwttnh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvuvbwwa.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dkwsezam.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nvwqcydf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2iqeybepg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mfdhiycl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tknuxhtx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kfqznhih.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xgruxhwi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pfrhjrhv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xsqeoyag.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sbotnwji.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kiipuear.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnpmnlw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hdqfuudi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vkfdqnqn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2cxujixxs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hstnxboa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ocowaeas.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iktxipiv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vuqdhenp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpdwkaf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mtwocugk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fvhjrjww.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsmfjdzj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pvskwrey.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2asfmjvqy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oghrslqy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ydveaeja.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dtzygjya.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2awymognj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eybmsbog.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fmwtdngz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wwlasyke.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zbsdgwwn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yikwfkgb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2isvjouyv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2tmroeesm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kwnalyog.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uffzyzcq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ppxswtdf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hasqblxk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zsvbqrop.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jlpvrzpe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2twmhjapj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ubsnfnvb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bqxmmcrs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jgjohdaw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cxqxtukp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fnkbfcoc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hjlffizf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2orvlpfzk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lrxvkdhm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ftefxaxa.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ucjsmuat.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2razkyktz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vbcckmfw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pynqqrwe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2sgblmipe.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ocailsjr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wlxpnofz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kwfohxkn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xoffmzfb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rqpcdcsu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2akiudoty.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ufrvtmxj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lpwkbazy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2thtvgitp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zsgmwuui.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lzlpnrmy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2etzutktd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ypmkhfyu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hpgqeeje.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rgwptngs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zgvnivyq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qbqxerxq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ywhttemi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xwsunbeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjzuidir.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dhhzytgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rijnsukm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uxtkerph.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2twqievqi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2vihwxtxf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2brifuevx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tlpvtaml.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kbwtcqbg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ltfbsrie.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2migkcnei.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2oevjtahz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2usdnarqq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2aqzsrbmg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mjzhajhw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2htzyhxzn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ptzgtnks.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vftwxwea.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gccgcwzi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hvbsuytj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uqjvegtu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yjdlslat.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zwardair.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2issglike.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uwbppafd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vhujgwyj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ghasycaz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ebylktis.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hcfkmwfk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nqnggtaw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ojxpocvb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2eksayjuo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ymtditlb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uvqmtmxy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zlxdmtir.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pifhuogv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wjpwuulx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hmxeslrt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gsecghud.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iohclkqh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gihogegt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jgmqxoju.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2afxufkqs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kvuoeiyj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jpkiwfco.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ehwwqlud.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2erobjnzj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2olyhtddc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2rriurhnx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2emewjsjr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dzuftzhn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jdnhhkyv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fbtaddpg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lcbmqjoo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fpxeyouy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qmsityfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbwtajsp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2lygystbn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zyxxahwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pakyvryw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qjaxbvja.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yjyiaoou.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tzqzqvcf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2geptjmix.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rgwnagqm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pdfoagti.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2dwgmyiae.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wnlbffmj.html


<!-- 参考信息 -->