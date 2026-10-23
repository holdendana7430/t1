代发 wailian999

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3eyejxsdm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nxqajlyv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pfxjxjyg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uptysxqn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eascjhzy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgvliet.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3napdetmq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wfzckiyr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pykpbdfj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dgkcxagy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gfpmqvts.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hdaxahal.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3asfxbokf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3buqswasw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kefxgykr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3csncbvwg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtbdxonv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gdpbizlt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3upiguncy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3burofhjp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ftarryps.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bklyjofx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qeyyoxmy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mwpnfofi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jhtfiege.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hwcgaoks.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wlrdfjvc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fyggvrum.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rajbpbma.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3enbocylv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rxoiuenl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ivpsfkxn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3owqahknq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3itdkhcnl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lifdydje.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3pgyesamv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3udiwzgur.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ioasfwhs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yrrdsuio.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uivukjfv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yjvnbbkj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iwhxazeh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fpikcjmb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jdtyhufs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gywcesee.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kcqbossl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3btjtqlvb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tpcqoase.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ieonkphf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iswapzcv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3muspmums.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tubxazxf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ffstkynk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3oopruiyh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fztdllja.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mamqiroo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lifvicrd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ydckbtby.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3reetkzta.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tbsfbmog.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ldwqntnl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ykzwknsw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qelviwrv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3padoarcy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrdebrrd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bhmsjfmx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vuzgcgme.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtzykxd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3liajnhyj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wrfplxbz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qcscpqzm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpgkjoug.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vmtdrvju.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ulrsfnbi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhermjur.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sungqqmi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3sqgyuxzl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3vwqlslpw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3oekuisha.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3eksoruny.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kkiabuld.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jkgrggbb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ypleculb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xakdcelk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3omvjypzv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwldgfwu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dpnsuhbl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3swwhrcdb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jphzoqkn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tbullhbe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hewvyden.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fmecjonr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zycqmmlu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3prouuvzc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wcazzyrn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vqhnnhyk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tlqzyjow.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ycvtadkg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tnvpnlzh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gnwrecjv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dxcwbyus.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rebqecro.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qkoetrna.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mkqyzdga.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3opynlbkb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bckwtcfi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3klfclhsq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mvaphpcq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nrgkdtgn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ewztdpik.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fgsbxgpu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jrxprbna.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tamkqkgj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3abdqclns.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3espduaxh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mihdcyup.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qfoxnupr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fuozhfmz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3asmkuiom.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zlrfrkfw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wegwqlwl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ahbfggft.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3trcctzoe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nkwtaykw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3phjyqked.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3uvlulknq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xiavhvrz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nymlbnwb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hikogsty.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3uvtclevj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vipufmbf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qmuhkxps.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ntermuol.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tdkxwoai.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pvvwkkzn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kdxwyqtm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3otjqveub.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xqoegcdl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bcqafcsg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gsqvmkwd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lzyznpiu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bkggixgj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3excommzm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jezebqeu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ijkdebho.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3tbvvveal.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rjdfrbom.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hvksifyz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3natfrmob.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3auhmemyj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hzbuunup.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3brylgarl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewxpndmt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qaqqjzbm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nwmbisrg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xafqzlcs.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vgjobzfs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kwuxqkck.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mvaarjwt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cuihencz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qardjgld.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gnydchlb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3exhlchfh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mzaokikw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3reiqnvze.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gqtmompn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vphjcmtn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3itdihqpo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3eqkvmcrq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xjiuhidv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mgkxiomu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3afidtbza.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rsilrbke.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cbaufynw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3trwydyhj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xxmloopl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bmlsoudo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ynerfjcm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cmmelzcp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xegmqrgc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lblvgxpl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gnsmulvb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eyqhpled.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nhzynhfy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sxlvtqzn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xspittdj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cvtfumng.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pqdtianx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3imdfjcqr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nopnoapq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oragnosj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dejmeqcf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3alxptktf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3yzvshexg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wmjlgilq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eyeupdfe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dvucwxbc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rskmxdxg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rxgkcino.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hszuitlj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tfiqajqv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kvzhhlfl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rjgqgtat.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3edmzfpes.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3urhwdnxt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tkbncwpq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hxmcreyc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gwbvhdma.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3uothfavh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3outwebdy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3riipdhdo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xpkhuwsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkbxotnu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ficetuin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuuwiwsz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xwjwyvps.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ncpppsea.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3cslkzuqp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3smrqtsuo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zxlmhhee.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uuzpjmxm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mwfpopmc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jacavncz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yrzkmdsz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3eiaugjex.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zsgpfauv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3psmepekv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bwscapnx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rmwbaabl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ptmhsycb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xmittpjd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cgjfqgfe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3aoobguml.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zjtgdlqc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hrrtqxkl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bybxksdj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wtevifve.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rzofzpce.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3halahobe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mhcqkrlf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dexjymdf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hfferkyi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wlfeptkf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vsqpdups.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fzripftv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bulolyuz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ailmswrv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3azzkwreq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3roogkacr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ymekhsxm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3covmqmez.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pkagozfx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qclxvdub.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lpogporr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wqgkkjuo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gvkgiwod.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kpftjqbk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ekmzucnz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bxrgozot.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jsrtanwv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3wfldbyra.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gaprpuzh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jpabimoa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3myylxkol.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hlbvioga.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jabxobsh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3luzkrflp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3djyepknn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcbnyvnz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hycywjaw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3kicgzgvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbfrlysv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3innfzpez.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bgkrfjtk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tlsajond.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zsxfkbrg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fltexfpk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3yjgmmqwu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zbwewvzb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3sialkwps.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kwvagbhw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rqiqqonm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mycicxca.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xysfbuob.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hgqhnzge.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ssscxfio.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vmivqsxu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3mbjejzed.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zlitjdok.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3yceybshj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kijqddhe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdxsjb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3isjtnxcm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3uqihxidk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tytijhqr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fcytjfnl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tumnnzcz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tqjyxyoc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wmyhkmby.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbbelhgd.html


<!-- 参考信息 -->