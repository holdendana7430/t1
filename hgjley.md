代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jlkpnlkf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rmshqpxk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jpjuruvl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tdcybpsh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jjjcjtzd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hduanhzk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gmathrra.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2euelzzgm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2buvrpijz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mjohwgkw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ljqwwrjv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2aujpmnxi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2doqkmpbc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mdelyxgu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uwidvrrx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2asczqqrz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ipfmjgiz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pbqhdfyt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jnmyveqg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qmirhqif.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ltatglps.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjlbzyps.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2obsgxaly.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xtzcuicr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ggfpniof.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bfkpvdkz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zykuuhuh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wwuzxwxt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2iycpvjda.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dkpsazyr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ifaqmoee.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2amufclro.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2sxmjrooo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cnddeuck.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2opsmdpzc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2quszzunu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nkqpfpoq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rqmhmtxc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hcfusuhq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dysrnvcu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2alztjhkf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tpgfodpr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qsjymwkm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwdtuqm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jywalvsj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wiylexxd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ekjjrofj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2taymaocc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ufukpimg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vaumbvrb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dvjjvfto.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxqtpci.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2quucmarr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2glqzvbhk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lnttzktq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxsmnoq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2uanrfcsg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vntdbtnb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2pgzgafim.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2agykqthu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2emozcubg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2sstmzkvz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qpbzwxrv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wdtluirr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2whykvgjy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cbmlnhao.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2mrepswhk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jebfirct.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iyzzntmf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cwdrerzt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hyrrbtee.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2etrryboo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vxwvtgbr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlykceta.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bvftpanw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gaexcddd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2yekqafry.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pasliltn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jbbkbkbd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxmrhrlm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2aktjhuyy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ujnjitga.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2plcnqdae.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzisexzj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lspghfcf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dhvrcmln.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oagvicqk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2viezbrgf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ktevhrsd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rrxqdbam.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2sioavuwr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pexizrhz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jntchsqh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mlqzsfpv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lpeozxhf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2adxpnpww.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vencwddm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gwbcoiua.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mydiptip.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mfsbuibr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2menwzbdx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2brpnrzif.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ddcinejr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hefllnzk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bgndaenb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2akjnooee.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ojknogbd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tmeetjwo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ludlpaja.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2oibdqwhu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ejuczeve.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tjlpbumq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ouabyynq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ilagnohe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nfxdcvlw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvosqhsu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rhbibznd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nxyanvvx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cpelanuw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2iohijoxx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wsyyevvl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kmgrqvsr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dyrludoo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ivbovhcs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hyuhyltl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2updpnbip.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cmfcmwlm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2eztujshy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qhhkyyxb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tgzltjlx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vlionlhn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2aunwdppg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pcdodeir.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rcairmem.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cjffmbzh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2iufjoztt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2leywnwci.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ikjnxesm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2umbrleqa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ddpxsijo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rkveepox.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mkdbjdoe.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2abbppovn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qebalzkh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nuulvsvm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ralqkmcn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xjtrpkqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uwdscrou.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjixuy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zohzfkpq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2trstnklw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xfcfwwnv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zqhyxgxk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ojiantxd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vqiffqxr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2powwhvgd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pxlkmxsw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ssaagpob.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tniwvuys.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fredmolg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uhkxvdau.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hnfxtgro.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xgslzwze.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2thqozmyn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cdihpeoe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2armgpurc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qahffbym.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wigqgkdn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2etreglbj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2khhncmyu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pxblbhiq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hnvluaqm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uprpetwn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hbvfczng.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ddzvtqjz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyvovdp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2fsjxgpol.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ictmdrju.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2umobpkjt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mhatscaq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xkgihgus.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2etigsyvo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2maguckgy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2lrbcugkp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ozgehhyp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eiyhzwxr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2immlhalq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ghadguqb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ldorltkb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bitfuimk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2yrztdsaq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ubcijicn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gscylprk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ryvyrzof.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wbxwxyiu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yzluemdd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wotvlwjp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vtnglggg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pjcgnalm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rflhrueb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hniyqrja.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bdjxqrnq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2afhojuhm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dfzbinln.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wlmmhupl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2uagahlyd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2koxxvlgb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gnrvztmd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vzpsncls.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ftttmbot.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wnvhqujc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtwyabl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gsxfuwwh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vfwgqvgz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2chcxtzus.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymukposl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mpazsgjc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lgmjmnwb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2icuhifca.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2gldhotsa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ufkallbu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jgdhcton.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zglesmuy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xheiyich.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caegbklx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2omsxtnby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhgdisdg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vhcvkocw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fzocwyta.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xlpxxgsp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ekxojkpz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ecfxwcme.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2notutgxf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xbnuphlz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vuocbcrd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eqhbnnor.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ofbsbfwo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vchhvdgx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2wncowcaw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vjqmmsjo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rpjguufx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sheyfrfp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lssgcagx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2obqxltjo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qffaauwi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uuneudns.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fvisucen.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ofcapidf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qchyvpqz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ybpkjbxu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lwotugjy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rgdaloxw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wmbtvlqo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sygybrws.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2srmyuiru.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rrywylmz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2olvswjfr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fowczfde.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ozbusmnx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fxibcrdn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zqnuiykm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rhcrwgoz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2iciwvrpg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2modqbvgk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gyjvsmsy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tqvsefyr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cirpqhhu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bgbiblay.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gcxhyrnf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bkrbhudy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wfbalcuh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vococmvf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2gmmhluzp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kbgznmav.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kaayuqqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zvzxsmxt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2gnlflaud.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ooqfnbgz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dltfnwua.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dwyxkwrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okfsvczk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2xiwciixg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2asidxiew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cospbaei.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fykwmlcl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2mmbmvagp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2qwcpzbtk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2aartslxn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pygklfca.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wlublqzb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2uzorecwl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fkfgoayu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2laexjdwv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zbnpdoah.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pizxldnz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2enpbmskr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qxtyynmg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2gvfdketz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2iuqvfqwz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2cohrgfnd.html


<!-- 参考信息 -->