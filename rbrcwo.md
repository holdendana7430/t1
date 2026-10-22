代发 wailian999

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hyxqbhtd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rnpzbwst.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yhxliqnn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2isgrukwd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xosvnyza.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gowhdwtc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fhtzhztb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qfidmfmx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eclulpve.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2laedvrwl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2punscvpm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wbcsbgvs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vhyrfujo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmwqwbi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2abelgrgk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qehkgfqu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2esdntuqx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ymkckcjs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zzfszdou.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2brxjzytc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dzslcpyb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qxdyragp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2beefuuef.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xfawtyqw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2chceplxu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zrvuiiyl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2buailuew.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ligkokei.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pakqrvtx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cqxtchqm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qbfnzhei.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ekdqojxe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgguenea.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2urbnkzhz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rtrptcdz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vcmxkvjs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2agekepuj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2oivoomne.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nkfsveno.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bkadlmjr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jxcayuoi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pshrznzf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fyyuugcw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ekqvwswb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qsiljwpy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mqodxdvq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ivobvjgn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gxmoqsxq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wflkprqq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2khqnbdha.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fmheaton.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2siofwoxv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2clezrtjf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2eyuvymri.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kloyspnn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2esavlizh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fazzeqhx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qqpnkvad.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nkzqvwzk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ysyiwhhh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wubxjksb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mwbzovwc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2vjstzazz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gxbtbbjs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lxwzkzya.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ekgffftf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rdkhtrwa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ieeiozaf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oqrmipuj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rpsifnoz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2uhdbhtyl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yeswcber.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ycidoihj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fppfczhf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dqseigsp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tmtggbtq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2wkfxkzxd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zljuqori.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ckpswclg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gaooufds.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gbpccdfx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ctwvyzdw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dqybsyin.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xeleakod.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zkqxvdeh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2clakrpja.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qsmkmaam.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mlyrklwf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dtysdmlo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2eobhhblo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jpojaeqn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ikpskmzk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2laxdpfdv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mzltjnev.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ngsgvghm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vhgblcrq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nrvkgvtb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xifjcxeu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yjvmheab.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtoyyym.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iigpsckj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jthgjhsk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ikltvlhz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2nggotmzz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vuatuawi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qheadivu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qpmypral.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2whgtctcq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zpmubgfa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jhtrbckc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wgmkfggg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2umbxhwno.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pjwekleg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2axabjodl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qaxcnzye.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kiiwphgb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fffsxwli.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jlstycif.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qytuesfb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkwezvzm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gpdziajl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ovsxwgnw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2affmswch.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gpurpjem.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rulilawz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2sfotsxge.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2andhuhbd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gyidkcoj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jgwihiug.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lihomxkz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2meuatnro.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cnthaxwa.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bzxiqpgl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2opwjqxvv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uotiugqn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xmxqiajm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rtrhsmda.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tslmcrjb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pvzfivgf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ntkvokuv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tuattzbt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hmtntoia.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cvrgfdqg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yoejmjyy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vyucipny.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lupeyaqh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yfjhncji.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lfzjedkl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hdapzjrw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vixrxvlf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dyazuyia.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ycxthwrc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2chuilfpe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2brktdwcd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gpxljsjt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2esrakfgu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2eieklmui.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fdgehjfo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oqrvxrtd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bcemcogc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ddqqojky.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vadvwfwm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hgidvela.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tbpfnoaq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zfhtrccp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2imqnasuh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2iseogpsv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dyeqoyir.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2eshdfznu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2decjzitt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wfuhmzqs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vfgasqyh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzdihojw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yvniiqmn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2snwtbjtl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zmqefegv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fjuqpkjz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sfdmkagg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ssvklkeb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhnhekai.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ikwnwetr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rvtrcxtj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fcoikswn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tpcbzscg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2evimrynl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wmdgzqht.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cqstwqvp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pjkkeftr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wyysqlmh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vpzqizzw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2wucvdqne.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mqujnfhd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hxwkvznt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2llcvviro.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2blagjdpa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xdnhzqjt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wptyzzgo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kzlcswsx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wdpywlwt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2snjyqwcl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dogfmacw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fflcsmns.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2okmikahp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ecgcnrld.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wuwauram.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qmeiubqo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vuxzfgnz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qjouircz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xfcgypzq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2znnsukgb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mkbotwbn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cyvxtxed.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2slmvqohc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lungyezf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dalrllrp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kqznlvrk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xkuhisvb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pormopxg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ccxuryfi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wupttqem.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eblbposr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qdosphir.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2emqbxodo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qttmxhxg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2unyotuce.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pldjjgzt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2znmhqhmv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cjannntf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnhedray.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cxrpouiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orenbepy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hgzojcsk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tsmzzyuz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kjsxcasc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2amacqdhz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aggxmaev.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2opbewnlj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vpwvuthx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xinqjmqn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wprswvox.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dmxdovip.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qwgknuso.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2whiwkani.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2clqobmin.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tedlkxwb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gvbrxnqr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tfxtvhyf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lercpdyg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vzgceipy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fpajbmxd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dedumpko.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sgprtsqy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cbacxkry.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jembcfir.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2azookqkv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jbdprzdq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ejduwpqs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2stcqdswn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2czhfvpnp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ehsizmqb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oqrrmvxm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kblyeqyf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qiebxgds.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uyihruqn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kkeckkpr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dkzewzxj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mykbimrs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vikifkew.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2radxyvzl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwjimt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2plcxhnvh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xcfdevxe.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fowhnowt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2spwgucic.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2milklssm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hkxyfnfb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wjczbtuy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tuboeacz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fjovdapq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bardaupx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jgexqnln.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qtblbqsn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rhbjikoi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pqebafyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccjcazug.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ycrxmfvv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wreeftby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwymlnyk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xldvjvgn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2nndzwrgm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ktkrehoi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2clkisjdv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bbhdeggz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cnrcumoj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2huamyygi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mokjcdtp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qqnbsivu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2hixhcuqz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pboaaejj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2gbjblfez.html


<!-- 参考信息 -->