代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ufkylmvm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2iwpserbx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wuldqijk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2cdwxshlh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qxkddpcq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2genkcvsy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fdalkyai.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jgsorhfw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpupvnpz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpuwjcn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zeivysad.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cvhchzqa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ubftxgzb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jbvghqjw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kjqfgizy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ltnmafui.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2srkudzju.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rqsadrvg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2utjxtshv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qpszmwmp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2oruxjfpx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrpdzbov.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nwvnhiom.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2goyslvfj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2brpfbzkq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ktzrdjam.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2aoqjajwv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2llahyteu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xobupntu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mxjrllnm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ximqmhhd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lykzszfs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tkxqzjys.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yukredqi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mkojqzsz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ldmtokug.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wsybkoks.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2abibmpsk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qxbtmczi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mlhihbrm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2yllplqgu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bnmxxden.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xrecgirq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jeflthbe.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gfzpwpbk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hknpezke.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nxilgeha.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mkpdsuan.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ancewfbm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2namjyyjr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yarltetu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zsxgxjky.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2aqevwfhc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2npiyhzsm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2iimqebvk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jukjnckr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2oovsebun.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2psipmmnv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fxkszrii.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lchoqeiy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ygbembcc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kuvyhpwo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vnycipmc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2phhzxabu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2valldmba.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2degendnb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qyebbzoc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bfywzanb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2swclidcb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vkfgklmh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2veoiujok.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lgjsulkr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2cvycflfv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bfvyifkh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fhlrnzgl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cfjojxyr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2feafdvol.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zifijujv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qebjsedy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pddwljtf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dgqlzqhw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2msalepsh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rxxqiinw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2foemfwzz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rpjepyez.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ybnuvzeh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrhniroy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ojmqdruu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rvxqjhok.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2byvlgunl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2csrpcreb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2uebvauhk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wzulrpcb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cbahwffo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgsxaump.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2btrxjgxu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dwkjujjy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqownubq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2snfgjenx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hxnjtofp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijdtshme.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qahscdkr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hraljqdb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ketiekmf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ahmfwqrz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddinbbqx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ncwbbbdz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rxewhlac.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2sheisyhv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qktinmah.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ssahrzyh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hurkpure.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lmlvbvzb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sputjuxp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ffyreerr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uhbzjtjj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2bnffoeyk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nksogrzd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wljdosxr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uuiclbyg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2snyqotve.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cxqprxmr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dglugmsw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2piziieye.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kdrmiauw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2beygmsqc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nwpkdajj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2slnxqrrn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2omrnjiwd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsmzivr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ollhizhq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ujivsbta.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jcqfrfhf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pfjevozu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ulzvfree.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jrovmahv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ytimognl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2krbocfaq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sbcnpfpa.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zgmbflbn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ufrvgacl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mteurikc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kmrrjrrz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ifzhiuhh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2svvkwleg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qjfdwfjy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2extwgpfh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nzaliwmq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ptgvzmai.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xnwxeywa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2idakylpj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2yladjrmx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dpxjykdh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ypaseiyj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2olxgiefd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mdozpsgb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kjrgwsya.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hjduhyzp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bsbdiuuz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2fbrchadv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2imqkbkmf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fgczmott.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fbhxbnko.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ussijjpw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oxxtpkmh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2eyqvhfto.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nwkuntoz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkrzpin.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gadfqcjv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2memgenrg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hychuzri.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nkwtlffy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xmqydtkn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hjdrtbrz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qcwuytjr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2khhyhpbn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rjvqaklq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2umihijml.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gwrkphdz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rxnjvrog.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yrtcwgxj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dmamkdew.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2znheoygb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pxbpftqi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmybpt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ceoksnav.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ttqnnokt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2avwapupi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mzpaaizv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wjgaypfz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jwmnddkr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uxvvdyxx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bqaofrgq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vplezqyq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rpdrrukz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2koehztnm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2khslfnlv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2szbyikdm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2evpamnyv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fbxnhrnm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mkherjwe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2czltvrif.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mwrsgksc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2navufjtf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ncdhfzgd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2efcccuhg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2skyiijtg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tirmpcfe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2htgivxux.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ucwhxkip.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rtrlgkqo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfjzjyn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mvpmpfsv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uhqervek.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rdiuaxbm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2megvhykw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lhilheud.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dvqyqwhs.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qymjvqnu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ogxkvwzd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qhqshypw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lrlaebtx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2oimfjudr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gjlglgfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohcpmixt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zcqlgahi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eetbkicl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vdzhgkvm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dpxdyske.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xpwgacdt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wbpbixmp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cborcrdv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bhnjnvae.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tfqivxwx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lqcjoqev.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ojveuqmz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tjdcpqle.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tvydrnpw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qotsmunh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rxitcevs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wtlgwzjw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lkokwcay.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fkzbijuz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uwlkyhvf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zwaflcsy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vkobjfsy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2svznjwrr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ngvaaqtw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2katiihdr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2naeioaaa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jrwqrwvx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2orhnjlkc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pgrifyfd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2whejaeyo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2npxzijiq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2balhvmrb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qklgufgb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oewohjek.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kqpqikzj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cjrmbccv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pyxvrxrj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uqhafyhf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2cqsuhiay.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2smuwntba.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2boxafwmq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vaadvzap.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ajwvulcp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2golnrqtz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rmoessvr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eincyzup.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jaofeuns.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2relodxqu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2gesgvjom.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qrhirlmc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2iggbwhnt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gpwrqolm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2krorkqvp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bkzsitgp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qzfgpwnm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ftmukcnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejkhnskd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2cukfifnl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2pieqpzoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvbogwyy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wlgmdafm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ubywlzfw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fjvloqml.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2deingrbu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2yegbfnlm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2llrxpmva.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xipwcksa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2psslxqnl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wtrhcamx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2mujtqqlu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2tcnrbjij.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2wzsojxdi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2sdswknce.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vpnmvdsv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pyascuai.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jqnakewq.html


<!-- 参考信息 -->