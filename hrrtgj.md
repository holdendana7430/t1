代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2azhwnnxu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vpeqaayw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vsqtfacy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2eprapmpq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qltimopv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfatyjes.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2snfsxuks.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lmpuxlro.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gnmoiqix.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bquaqqwo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gxattfrr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfwsllw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qkmxwiha.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zkmqdnrl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2areddjvb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bhmhujbf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2onmwnuhb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nalahrpk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gsoqdlud.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mcntimxz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2utnimnit.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qwagytzo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tewyadze.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjvfgpi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2athfowuo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrzqcl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mldwbcdy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2woksbeyf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rykqejub.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2brrxavwm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2emxpvuig.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qyjgmofw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bltdoqgi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2axcmrhng.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rqdgbfoj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fkogbdbf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fkwkjbbf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mmtxukpi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fsuhznmv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vgnsqqwe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oojwlnav.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kdhnnhqn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ngabdupy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eoqpqile.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bijmxjyf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gidlmeus.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2asoqkoly.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zdoznsvj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cpqbejum.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ogngnntn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mujkcafz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bbbodkyy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vaipsqan.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lieqpyxs.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xscxwkbg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jlbusjgd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2heymeieb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xxulzxen.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bihzjams.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bqgldjni.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rndijvzs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qkitlanr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zzqocjzz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qcohujdn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2iuqlhdkb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fdxpzjcf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vzeebusc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ikgwhlgd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pvupboxw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nzytonib.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2onuhelzr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qaaurfpp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2guricikg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uknatuzw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ehbckmqc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ijnchkaa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ptrguxvd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nczqvrto.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uwyoiotd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jondkbgv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wwmzyuoq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nlydfcnm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kanrbhew.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynlfoton.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ayhtrelm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xdsoxysu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2elqloxai.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oetnolgd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wvfipqwf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ydewnsqo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aexrzdov.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2skrqoovq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2meupfeuz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bcdipfvx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2npeigftr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2phfhwaqy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2slcekwnd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cfsdgeaf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2igavbsqe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2arwiqwbz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dparxcsn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2szjkqtfa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2aoovygsm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hgwlroyi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jipolmwn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rwsidgth.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2iftlrcbo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vzxotggf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2avhdcbiq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vcjrcdht.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sroalvis.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bmwithqn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vwnjviuq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2isxmpwqm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ucmgyylg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mkvsetlg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yysfnipa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fmbbhsip.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yybabiqe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2aipxphzi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fuhxckew.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bdsikjiy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2swmdidhf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rmhescgw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hvwglett.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gqbvmlbb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sijdxejc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mqiyspfi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ebsdituq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nvixtnrd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxyfrume.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2maidcyhk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mrrkfzlw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gdhwtoqk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rrxsvevq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2retbrvmf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pgghczia.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pfnxumle.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wzxivdlo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2whnqahsf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xlnkjomr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2nihxrwcr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2evadkaho.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bmknzxgq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qyvxuoip.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vlfcdjkp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zfyhhxcz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vrzzsfdv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qmdorgjb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xkpojjxe.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ihlcarte.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zvfhgytx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2smfupugf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wibzvmus.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2grcdknwu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jnwwwuyv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dwiioiqv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nmjknqxz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zsveczoe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yoofzfba.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ziqjnpfu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2snjddxxn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dwpnhjuf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmpvrao.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2illxkryc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hstuipyf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vdmogole.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxojwknf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrewuwvn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2dyydsvlx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bjossnoj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2izcwluxq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zwcfdsvf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mevdepfp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kcgpofqk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dxzeprzg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zhmuhkaq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ajneaqcj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xtxcqqab.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wgzidjcd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2toowsthx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2gczgntyq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rmnppqlh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ovqluzcz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2trvrpfyf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwiahmw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cnmwtodp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pupvjstz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2oikkcxoc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rrpqmrky.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2siqfqvee.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mxjuvsxc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lgmrgknq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mxprnbzq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djszfdsh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hxjxzyrf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fbsaddcj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ictcugbh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2cvvpvmut.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2helbohqc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2abbrcbnc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nlhlqfzm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bvtalpef.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2avjshdrd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bamrhjod.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pyndgioi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2thxlzkjv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2epgarhsj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aokxgtyp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nyyhscwd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qicmnsot.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdhtxcl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cckyruas.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yryfdqey.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ftxzdpvx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahnncsff.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rvcuwuye.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ynkqybtl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sveylqym.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qwvcyvxt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bhzvgcqe.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jtrxrvin.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hamqxjqk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gjldbwtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxdhmlcw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bhyfnacp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myjafnmz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nibjptas.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jkormbxq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ztcnsnnd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wiqfvxvw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ogikknzb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uphiiami.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dcqdcijk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2geppfzlc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2efizoegj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wlodjzka.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2knfxvrvz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xsxdcgrn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pmyxlznt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2noqhpogt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kyeghokp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hutqigyo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xbyiuuti.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dotldmrf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nbghqqgg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2eaytwijo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2klvbynln.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pumditev.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dqsejovt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2flodhbsg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2einnukki.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2sqmoirxw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wtqflama.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qeleaebs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ugigecld.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uvwuwjbj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2djqbxtmz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jkeubbbm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iukcngiu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2glmyxwsv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nankguea.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qnjmskrl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uywvtlws.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dsdzjqjl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2sgigfxzf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xktcwfxf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gysyrczw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2nkttfdvh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2apstblsa.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fwiqyzqh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qvusbqvl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2osayksfv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qudisabc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ozppjvlm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tuzlqlaf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2tczfbezd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mrgxjqkt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2frvnrgjb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qgjvqzuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebyelube.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2czhxnjae.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gshhhrlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rftfrlye.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2aroubpoy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2abtkyydm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yvqjqphh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uzywggmr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ijidullk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2thtfhqsk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2jafktqco.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lvshtdzh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wtdzqpsy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2weccmjwi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2gtibiwbm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kypztiya.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2farbvzku.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2urhuognz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lnrusshq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lomvvsob.html


<!-- 参考信息 -->