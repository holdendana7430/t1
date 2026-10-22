代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cfjpmkel.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gjthdgrl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wahyleyg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fmxdjfvi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ydfppcfm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2trucbzhd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ohbtdwly.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lkwpfiow.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2psrgbtht.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mitctimh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vfemnygv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zikkpgie.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xdayoaby.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2apqepubr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2uyhafpxm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ogtjoxes.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2svmjvdig.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pijwqjeh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gkvcnlaa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xpxhvcod.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zsvgrcbq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2elkrdipa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hdwbqolh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cmuqexyt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wezogxfp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ycnkkrnc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mbjmkjqa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dirmnetp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mjuhvzyi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nooclmko.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ajjopeiu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ggpqrylz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2uhczhztr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xgfcvqir.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lpgfrxsg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2upsimigp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ihvzdfvb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2flgydavd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xdmzdgdm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdnshfx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mcjhjjhu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ttivjocl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xfgfmywh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hvqrosht.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xgxqjktm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2czixrfnl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wcqkgckr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hpqscisw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pyveqyck.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jmpabjag.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wbeyraio.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmytvxz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lppmiypp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fleglifq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2smcusybh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vovqwgyu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gcdgguzt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2eglxltiw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2yumubtab.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vigwowix.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qpwomzgv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsifjvrr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tesdyhcb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tghcxhgc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ejzjzmik.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vzrexxce.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kgycrxte.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2sedvcqya.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ecdmvhte.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2amdzrcox.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hrgtviqb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xjwmdtzv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2llfqfvye.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fqcifyjq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xfuyqpco.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mpuhzewj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dutyfikr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gpzlesqq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wcxfqypa.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qihbnqbg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rwracdop.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fqpsqzbw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pabftuoz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fsxlkwyp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yknwtqcf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2vtkwlcrk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xtawcqsn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2huaqeccz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xhqxmmbv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pghyaluk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zezsdxcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2apufkoqn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2djdsvgnw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zbzftknb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2iozeyhym.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jazeimcu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dbtyukfi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2iclcwhcq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hjjriqaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2itipwzws.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rfkqtkpt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tdfgoquv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nkdsoabu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gwemttse.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zykjcgxc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gkrzoefn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xteguonj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2devtdxlf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2acagikpk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qqzhlegu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yjpzvatk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2blbzpnnn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sssnvsyv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xrsxmdkz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vhblgbkm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pwgehgtp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2anjdxtpl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rhjnohfi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tzbwnprb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjutxw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eplhtovc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2bnobxetn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xjeedqch.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jysipqig.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fkoaekfx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oxnqwfbs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jzmgagal.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ghiweaku.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dhwuhaky.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kitjakxf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vnvsdwgf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rfuqmspn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2akogsxoc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xdjmxspb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qtanpozj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zokmzwcr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nbraxbph.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tcbgceps.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2guskqybm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pimhbmnz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vqccmpmn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2muwgzrnd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sgphyxkz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fxgxadlv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dfpxvlhb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fohbiuir.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2esdtfsgv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qvyzjrtw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qhjodhhy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2whohhdlr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bngyhbqw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tbxtleuy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibyctjvt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2olegciiu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wftbsdam.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qbdtjcml.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgzdryks.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2aqnotwli.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubfzfatx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jruwvayh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2eoinlorf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vnsrcpzz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rhfqlugm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbpkfjx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lsgajgqy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lqfmembf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pggfhwto.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2cphlaijg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bwuhjocf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tesocnxy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2axpmgzoj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2btaakibm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2tfgefvdi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kbrsotss.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2erwagoov.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2phoffgqt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uwqmkutr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bzssbnbt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2czbjxxnm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xywporhv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bnrulwqu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pzjhfnuo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hujkyxlj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vrxhkixb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wlnutudl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jwyukpsk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xhofrjao.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uswkiwyf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ueruobsc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wtcciahj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2boipfkjx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ykwbibbb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zdfvlrmv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dngiopmg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2afmrnpuz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ndxnffgd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cgwuzjjd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fakfairm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jiwfsxqb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nwepdxyo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lmyicnuv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2chhzbopu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zfnfgwvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmlawefl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2deotgtoe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cytlcjzp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2butdwsnp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2hdjtcloc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ldibnjib.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lefzntdk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zbciiann.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qgfzgiko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfcunukt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2olqdohvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvgfyiaq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2sdqkxtsh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fxwwwoom.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2niqgseah.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2bmggijhr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uwkoyhzb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2furfzdqs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ltmxvpie.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dwjxklzz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2onarwzkf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2brklrort.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gujfaaqr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2gxbikydi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wdaxsbdq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wqpanfsv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wfcvduav.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2auyygkun.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wppikoff.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2velewnpg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aqfihogo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ytoqjwlp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jocikawf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tycyicwu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pkzrbeyj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aemixoji.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jvqusmkj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ucseozbb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jdshhirc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2otrbwglo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nrxfrcpr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cahrmffw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tbroehzv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ygbevqpl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2luwhndxi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jvbbsmsn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kkcspbch.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2pclfyrwf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ebulejby.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ohetrfpr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ygzrmfwj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qtcibooo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kcbexiuj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vhzlwidw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2edmfkhwc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bsrjkmvd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cipauadb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2obkdgzqg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2anpzpxwy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vmuekgyd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jmqtrcoh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nypkorya.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2aflcrblj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zcxwblrq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vsfyywih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdaaphua.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ccwarifx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ieroatvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxxoyktx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gfsfkagn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qauwszno.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tysyibve.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2dfvfghat.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qvjwblah.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vfiudjal.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hshcctnn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hvizhrno.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vayuudph.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dmcwhxhc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ljiivaug.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qsqjrrzh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2itehdnth.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wanjxmqm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bychgsfb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2watlfpob.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2yhrnusly.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zlscaqzu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zjzlxofk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2msgveiei.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gneidlhi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kimcceov.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gnyihafs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mdzkbuvs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trgywdej.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lyenmjvi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owprquau.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qwkftmhw.html


<!-- 参考信息 -->