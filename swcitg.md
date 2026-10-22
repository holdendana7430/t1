代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hahvpkkv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2homxtzjm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gniumvgq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mycoaozw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2eogcbgvi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xpgivdmt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wntxekxb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ozthkfax.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xvuxhrmp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2eocxteod.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kqpzubta.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2gaefexvy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hsncuvuk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2japbsgid.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dxpoomit.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2slnntknd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qhnazmwf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qrtassez.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2harvpeus.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tjecqkkb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bfnkpeih.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gfwjgkar.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2thzrprlu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uidqoczn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2caqrjzly.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2itpljnzy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qyflgqqj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ajlwxwpq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wmwgprzt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lvbiphhu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ophqneap.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2iymlkqlr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2oiupmxnc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jieqqsrk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cfkmhauq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cukrdutn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2omijxncr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2encytugd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2fbkzqlkh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2miftrrqq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2evksqfky.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rrboilyt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wxvzvdhh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tmuwedjr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gnzuzxpr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2drybcpxm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2minvpbrt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ixbijpft.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2omsqcapm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2eohehlnv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jkcxilhk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rbmqzyww.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2awmtnqdf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hucfkpej.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wjclydjl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ahezixiq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lgovrywx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bhiqdhqe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2tqcggrjf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyuqkjrt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2uvymruwy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dbfqlmya.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mxndpihm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hmlzxdyr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2osdnmrui.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2aztdqyxj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mnwgjsie.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nvyecsbi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vpdxafdu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2prwijrsf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kpoxtlve.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2oqzfgspk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gdptahik.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2youksxdr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mblrjghe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltoxyaqw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ekewbkqb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hngqfral.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rykyhpcz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wezcuudk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ycxaradf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tfvqyjxm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vshplsjg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ijgvsbny.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2tezxuvjz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fhyqasss.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gezycivw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2abhswjqs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zzdtctfw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2swbnmguu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pybpqjnb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mozynbcn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bbtpdhri.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrbxjbdq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uxuubgsj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tinswotp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lwlqugtb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2meurtcmc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2idssrwkw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rsdppium.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ohlavxog.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2emwpqsmp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2oonhcjdr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2aeqptnen.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sjihthpj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ounuxycw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bbukxjhr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jnsnxdoz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mabljwjj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iqleoxgh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ydqbvadb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hvdapkpj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dhomuozh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qccgkquk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rpazkyuz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2awsaygtp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2znnhozcl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxeahkgq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ibeqcwus.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dunnczje.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mykvgjem.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gozsnrws.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2loapflgp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jmghxpqz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yifwayot.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfziekb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cliruwuf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2edcnuogj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xsnapmai.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hsexjdsq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wcqfeepl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2btyhnjbk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jrkgodby.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kieczzvz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qptfqldo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2akoomnrs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2omaaerdq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wtzohvtc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vuzqqvau.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dpbnufwa.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bchpxxbt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2yakdivwg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2oebczpnm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rakpjmob.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ddwknhre.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dpzylust.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vygetgqw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bimyyghd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ejclrjmo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2puyqedbk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sxiqrscs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tjffofgo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mihtanvm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2doebehwn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ydnljmal.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jscxvrto.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xcxhqpnz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vfttegfo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bumdagud.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrivcfto.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yqewmdhp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ofttcsdo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2frnlakvh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fejbztdy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xjvsidae.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qjqkebdg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mjoakgoq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2eoexqksc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hfgiwuca.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xxlvmvpk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2tbitxrqi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xtkwszzq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wsvivvuc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2stiucsdh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pmmcawxg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2oxanegkg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2elwnqyxh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xnhxrske.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2joemlmri.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2emfrzlyp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zdkjahtq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mlelcuoq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zlmsaxsu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lzsrasve.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ajixesas.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ifvxfjzt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wnublchq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tlxxxrqm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rzzpecev.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jhirexlr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ayhpokty.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2aqtuafuw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ovsaapzp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2thidrvdx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2uoaebvyx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uttqctaf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yflmskpc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2owlijdpl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vqmtrioa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xccpnefj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pcpbennf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pndcuurt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vcncobpm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xemmypew.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tgpensdx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2apjepqoh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ativbhig.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dmthozeq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xibdrxgn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xbdfgqmq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ybnumfwm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbkxbeii.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dgyqmnlh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yiydrucu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vwbtvbac.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2grzgjbqx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sdapfkhi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zmmaoxwp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2afsaioir.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xrvrnaev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nisvlcah.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wvipfjrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdrhkrai.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qthkfovu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ledmlvar.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tkrrayni.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ovlrnbxy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qcppgcff.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2szhrisai.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uofwuywk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rsbgmifs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mzadivsr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2egbtelwx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ibrzhkdl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dtxatvvn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2nywhlngz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2inssjyys.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mqkbonwu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vgkeuxal.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kcevbasj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qdbtoiyi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rwassamu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2foxxmcra.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ipscmhln.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bfevuqel.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gahxdbsx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wdefqgjx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2odjhfgmt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qrosbxej.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lzbcyqdp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xpkyvyep.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ndkszulb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jgqnxqvz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zvwekdqx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2khwpcbdn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qcueqrrj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2akxknpaa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vqpspxdc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fjgjlklz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2waqqvgih.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2swtrgckv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2oqzoaicc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2sdduhtnp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2huoodhmr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2mrbiflrr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tifkkgwg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ldblpzqr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kuupfbkl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jmtftero.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cznhvoeg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2vpvwrwen.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ngvjviio.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2kqtbvlqu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ypdycxdh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2pzfxlxhq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fixglhyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isyqtewd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2thnewfzh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2nwudticc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ircapsoz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wofsxpck.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2esahstzw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2yuqmwmho.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mpckdntd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2wzsrvbtp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2elwzyyus.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2tlakyeih.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2emzdildi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fuguruxe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jxtdfaln.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2habgfcuk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2piedwpkt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xgarrwik.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2svtihdka.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qaoksion.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qvffuexq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2sslntkjm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2rsakgexo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cdbsdeoj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hifdbddz.html


<!-- 参考信息 -->