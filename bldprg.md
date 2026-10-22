代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gfqweaib.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jrspymgo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pyhwgkii.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nxwauuwv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2olhxgydu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbvaxtz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2iptrkmdm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qutinrxx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lyaptsfn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2mracqiba.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kxzrpmbc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gufwqxdn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gmfbnote.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vyaxycek.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ngkeveqc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xzgyfecl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qfszgmsb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hkbiazup.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2adcamxvk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xscdbqpy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oelhxlxn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xwhhhuij.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2sfpjdypk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ntfsdaxp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xtysobai.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjlcywey.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ixqyxmtn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2iepuhway.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2diuqvbbp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2uxolugwp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wxwfkhyl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pemeygja.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2klklvkzl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rgdlkata.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wlxxggje.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2srlpejmf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2hhrtoqju.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mbxcshav.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hdeoipsm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xfujlxyj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xmdalicl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xbcqnuzp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cjafjdyt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bbznnnwb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2sevuzbwj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2cebxisqw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mmkamkzc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iuknvfdj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2libdftvy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uyfwspbl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tkuaxghf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ntwhredw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nneycuwp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2njnatlzv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nqburcgy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2owucrztb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ejwyjinv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wwmfaopp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lkxyfgtk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2uemkpwao.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dpzptatu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xillabiy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kiutzayh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wllngbim.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gasljtvh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cvketoqj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2namjotwu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2twisnrhm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2debgjnlv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rfgixkaq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ademwrek.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ljbvauct.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hxjqcysu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gokhoxrb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hesukswm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iisthdhh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zhwyiwtb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqggikok.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xvgifzox.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vmoqpbfv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tcihzgwt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vldstanw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bmloptjk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2fewgtrhf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vkgsspjo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hpnhfhme.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tcspwgfq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pzuijahw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jyjgkzal.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2udqjmwsf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zlkrjwws.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ypobrpyc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qijegajm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ipwfbvin.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pholqxip.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2larskcyh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ctgewfln.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pqwqfeoo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2idrcslzn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uemreafl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aerydcyi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qavslwpp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dbvvpihp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srbhftap.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kazmfutv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ugjdqalx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jvwomaya.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pqluvrwn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qrwingnz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wjbqwwbu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2updzfqrw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sgtyrtvf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vndzifiv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2frwpjhbu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2fcuddxsi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jpewfpqi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nqyuohpc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2witsweed.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2yghvwcvd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zqpycqlp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2amhwzpyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hrkdepui.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tqucfmli.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mctccxjo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vumisckv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fwlzvgqs.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ssrtlhjw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nykyztfp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wkmidbeh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bfbxonsz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lcsuxfcb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sqktgcmj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mveczjqr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmhxppa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2evdrqykh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nubxofjo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tpqpcsex.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lfbmuncb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kkxabqpd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2veihbbhi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wxyfmnyi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zmxaerqi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ckizubhm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fbcwxkcx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2argudlbs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2apogicsv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2cqivlnly.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ekfzfrtg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rmejhezf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2oqzuljdy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2snmjihjb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jojoujmj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2abthgrua.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kibhunjh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2dgbrjice.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wqhdwnfl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2irhkrbun.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lfbtrpav.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hikhemeb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2juphdian.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ypbucdkt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jrlrfypo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wlsniyys.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2khrxcrfg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nmhnislb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2reixyllm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2eysdyrbj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhifbgng.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wsstcluy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rvxzwirx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2oanuxunj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zsuwaqaj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvwykyeo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ctajuucz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtlwyfsw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2crizodvq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2appqgqjo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bkmuscko.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ohpijkqm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vfkwcszb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yusblnhj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cewzsyko.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ynnexhrm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2aibgdlrq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bjofyvsy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2urfdnydz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2clapsaiu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dinbxcao.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rokigqdz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rdiloibh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wvzztfgw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nbhmxous.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hhovxnig.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2olawcvan.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lldmxzey.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iszzqouj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hwetsexl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lcvzoxcv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tumwyfrv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dtzrvocm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rozvsaqc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrihnfg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kxheeifv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2glngdvvc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hvzbyofd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bbcciign.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pkovtpvv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mbuljjgs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2uctzrxjg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ngdkdkeo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gcgeykie.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ivjruxrj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fijqurmc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uisaakwu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hvtynquf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yuofespc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ogzzrhmx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bfnqvpkj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ctldhuvv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pyymmgyz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gioocgei.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hutsatuj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mskstqpp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fmoyjvob.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2hpkauenh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zaiabllk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2unvkiltv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2aaxhezfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjrcjpad.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mspctcuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldetmqzz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kzegonzi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vellqkig.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gmqfyuxz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ullranwe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2avakjbee.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ybhmeoev.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bksrjwcm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xhkyosie.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wdeizyep.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qrqteonn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2thlttwmu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2fdonagpj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zdlkcupk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2djvitccs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wxmurieq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mznmwztr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ocrznwrq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hfqcletb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cdujhrro.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2quikxcgn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2vwxfpxka.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dymuyaee.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uiqsfwte.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uumhwbww.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vzsamajs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2iwztrgwa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gpxlfjyi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qbxrbxvx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hutkrepw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dfhdnelf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2actvajag.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yxritqho.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ftiinkfc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xxlcullx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ldnhklbk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ixqrcmxm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2emajvkeh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2strrmnwx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bvvhtzuo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qykuipfv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2jmofdgau.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2qwcwciyt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fwqsrlom.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lfsruonm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fqgcxgbe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tutlhqop.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wjrlkqyy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ppehvbgh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cumbvsao.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zvvcxion.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rqjkpoyq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2upmggvod.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xbsvfbsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwwfljqo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2znnbtbfe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2juileyer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqtbicbp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xhmtqsay.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gqlspdqu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2mtbqmmnm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tapnssjm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2tzomlhmv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lxdbzgsl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gfhmpxbf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rsszbbdg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2sjsnmive.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2pskrrsnv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2tokvnghp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2eukgceaz.html


<!-- 参考信息 -->