代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pyuhhyxh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zegghmlv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wkckblws.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vmbpdzid.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tecrqevs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2verwblwo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2gqbykrwi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ltocdigb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vptilyyz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2objskxjx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zljmozdz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yjaqnelz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bywaztvo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2njntdldf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dgokjcoh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uxguibdo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hgmyhijk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2psuggbgr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fmgmtsbc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ceyfnylr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iapyvcdi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gnhehabj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bbdceiad.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2liiapbch.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pcrgzsxu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cdmddeem.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cphnpole.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zjkmxffs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tnxuyxnk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ikdnpcyq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xbagyrxt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pijdzsyt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hobynprt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2slgwiynq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bufysgji.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lpjkrifu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zymxecpk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qjhuonoj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fhztfjcp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2stddalmr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dabskhhe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwiajgh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nuwmvztx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2njgvpwjt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cxljiioj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2damvshxn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mzarmrhj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dmcurjqs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dyqcmtfh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qbfysqyr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dopnfrde.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2chigykxs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lekqyhgq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2iftprrad.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bnkoqvda.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctxojpnw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iyomuanv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2otakdcow.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2necdkirm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tbttitij.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydoxyadc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tuzkdttb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ybvcerib.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xarksqth.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2adbargyd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nwcsngpy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ihpqpwpz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwqitxcw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mmfuxvas.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zaqrvaek.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gvotvoce.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2biidpcav.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jwcozebd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2sxxosfkv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ymfndqep.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nsfeckxq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ihbzavav.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2optsiitb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ffkuzdza.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ebbfyhiu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ysaxlseq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zmuonxis.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lhfohedf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xevhkhfo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ofzskqkq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tlqvroyn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iqecgdna.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wdcsidgv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ukukuxuv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2agpjseyp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yhnypqpd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cjifgvyo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bpgjvgzm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqmvscgw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2asfjrgeh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dxpeqbao.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zubnqmxl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jslsbmdf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tkqgmxqr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2adxyyszi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uuwnmcja.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nmqcijzl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ypbloceg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vnpwwhgh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wvqrnlfk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zkniovqo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2efxlffyo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xqlddnut.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bpmrubda.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2iskblsbt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hjbvtnro.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pfeiiutm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ejwbyhyf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2npswanoz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jingkxxc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qfwlgwns.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sjldmnkl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mexfqifb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bcezoquk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jnuifzgz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2iujnxcoz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2klxhkjxu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qhtaouqu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fowxytlq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mammrsik.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2odestqes.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jpbvipya.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xfpfmedj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2uccsqiop.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lioqiedh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ffdtqemn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dkwvcfvb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mizgonzy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2yvhljmyh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nfrwowbw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxahafr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2plcikfjz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jmtkidjf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hailiklk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2oknxvzuc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2behabapx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2cxxkntjl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2awjgevds.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxepmb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2arhiibkx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2sezmekbx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jwhqqytu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ckwwvxzi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xcvxuyei.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2veobevzb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mzyecggx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2twtrytdx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rnnqzlny.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ubnnurid.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qaxdzgru.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pmajbmnq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2myjecuxf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ahmsjmjo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bkbqmxan.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yfdmrpza.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2oyphqwzr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vtwyfnnc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zcsgnhrr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ayqvmwch.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2nbwynuhn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sggkfzxa.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mksgpzyi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cexsaorg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fnglrocy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2azulixmg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bmhkvhbu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjhvcxd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2brcfytdw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2cvxfirbg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xudmwfhu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ugksonsx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2sajxtbtl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qlpjpqct.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2udkyktmu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fmwqzxmp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hmczqxbr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mvcupxtx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aybcwtsd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lybzctra.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xbbcwpjz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2apzukhjb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2egpkgpgq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2eryvbusp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ruafkcqs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2udblgahn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ssjpweoq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2adueiwvm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nuwapfmx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rkdiegjl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pdsssgwq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jytqrsmd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2snwzhtat.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jbfttubx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yvctpvhy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hacfwjiu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zejgloal.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2udqwazjb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2opaleubn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cxtpbnhq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2emzenwzd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2anouimxg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rnquznif.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qrjywgjf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fvvmrvld.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2feocccsv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hpbgzhwt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zzhafnbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2facuxcpz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dugiwpji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyoqhlrn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lwmcfgyf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ybdeapqg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2znqapkjr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mvpsubea.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qninrkxw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nbtvlupc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jszgamyr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2whndhrpi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qoaopbmg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2srqsttua.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jgqtbmfx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2epmxeepi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2glwflrwn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rnrnjzrj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xkdtxeqn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bistofxd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zdmydavj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tmboxzso.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gpjlvxgq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ykeohuxu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hrcdykre.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hsilwair.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2picoifuu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2agibfuys.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zjwxnurt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2dpbbzull.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ipsosrbt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gukjdhzf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2npnfsdxn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wbqnywtv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eywlanxb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lcvequlz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2omxgayhe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hppyvyyn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wlpuqadr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2duxufhof.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2coyiftdd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gxhcxgtl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2pzvvyomh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pummdniw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bkgssizz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rrlfcxiq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vjdqnrye.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2wmbjttgj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2awxjfzdk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dviovlnv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rmrhmgvp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2zxfkakql.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bprzxzqc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2tvpqnnff.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ymgiqhnn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jxvoxpfs.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hsobkxfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oabjcxss.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2wnvqnpxt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wemlvfki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nblohlkn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uqavvzlh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qlxeehzs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2zkngtcon.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lizrgsdj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pcwdkhhn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ektacujq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2eeoexcve.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2bhfifoql.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2jmdopsoe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dwdblyfv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2aqbnuimf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rlfqbcqa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wdzhowmw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2nmyxuaht.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2btqikreu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2tmandzpf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2waojhryg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2agvcahbq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zdgcxzbw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xqredqji.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2freserlx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jkaonubl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tqnehxju.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tptnfjsn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xotesszv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jzgxxqxo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gpsnmcdj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkncxftn.html


<!-- 参考信息 -->