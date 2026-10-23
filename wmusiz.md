代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wzengmrq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fqhmanhy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3foyaudqk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3scglnhiz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tehzvabg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3grjqfzvi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gilrqqqr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3krsqccsq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cwsyslbb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntgykdkn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3njpptrci.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhqxpwm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hjslooea.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yvwlirfa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xmufbazu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ffqeiqfs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3krgayaff.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3grhtxyrx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wnijshhf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3brhkmjjk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3iidzrvsr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gtindnue.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rpbnknqy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jxbxbivx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xbvfixhc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lquysmlo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3znqhvkge.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kakwouxq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dhddwllp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3adcnddhq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uptvlpba.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gmaqzwhz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vpojttcr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3irezekfl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3leoidxus.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yftdodog.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3swsttglf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3eiingfug.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ayccreav.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qvwuyvht.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vmlwvjjk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3pvlqdpce.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3giplybly.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3iurliuul.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wreuztto.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3obejodlz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pgysotck.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3oyngmllv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3nhxzwoud.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3scgowsnb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sfptwwus.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3atxccnxk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vqsgqnwn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rearlizo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kitzcymf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ukciimyg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dqubstxm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xkwyjrat.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihwzqxxu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cikbmlzh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3afxasitd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3keipqgbp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jdmwsour.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vjmdphvw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xcihxfgr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dxjuxyyv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iswxhhpy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lbjloltb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fmwitpfm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cegzhgxp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3reokimvg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezpmoqho.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ireualzr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dxbxxofo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybfnbboy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uuilizyk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ptacpinc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tabwfxms.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mvsjyobe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3owokvbhx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jyecuyvi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bqrgspow.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tcjbdwxk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yjgfxcnm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rzlcwzrs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nsmlgvcw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wjifmpsw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffwldhsa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fmgwmpqv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lkbpokwt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3brdcfeld.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cefniqmn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cksetgap.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmdjgwyb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qyqblrgy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wxjebcit.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ybpktmnt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3apytduzz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxwlmvgp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3purcawif.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ikwuiurf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hieihqcy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pnrlzfep.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nkpolubl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3sabilbwc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3itufayic.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3klnxwjsf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fxkskili.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3epfzxrlw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3utacewea.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3taafkphh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mkpfermd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3knvikdlg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kiypznga.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qxhjneig.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ouajbxol.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xkunmjhq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xrdaoknu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jowicmuq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bcpgxirm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hjgdtwds.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vllqepjl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3udcoeihz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rpzuusot.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tstlcsni.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3upwwmjne.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ltvsaixx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rcukpzmk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wtnjeljl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kehjyrcq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3brxjkxbz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jsvrwfvz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vtkybcaz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pfyzpuib.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dakezkpj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qcwanjgh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cllxprpj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ayctdnvb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hvaceuut.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3sxkjmczt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bfebiyve.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pwfhyosl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wrdkwsdd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ydigazyh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3pfstpixm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dutovsem.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lxintrwq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nlrrhtvd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3neydrxad.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xzpplige.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xbefscqd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wxrueerf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3atocefoa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hoznilah.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nsfgjbmk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uezddboh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuhglnse.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gbjgucca.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewjpcnym.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3akyibrng.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3adpccicv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qfcuuzgm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rutabcji.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3boutqhha.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dfoehvvo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rsruutxc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3splezdgn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ddtnzgln.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zmgdejqi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gxnzmjzb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xcrhzevb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mudopfrc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tjguxpmc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3srbfejai.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lfprblqa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ujpscxrl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qjlpyufp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iewpujye.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3sxcwkdnc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3upjlntxc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3txfibcfh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3okczhqkf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sxefsnbf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3knduwsrw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mvhtcxgb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pyujqcal.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mcunqrdv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rsobtlox.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gayiahhp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3otfjzsly.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nfqduied.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gefyagaj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mdespsjb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bdyrqmno.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3vnscmhct.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ewvjxiia.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dflkiebg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pnbesdjx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3uueturcx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vznuwztf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eskhuogo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3prcmkdcc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dadffdyl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3exqrlgvp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3edsjvcid.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aimslvgj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rcspqdxu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wcoblufe.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kmdopppf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uavlyyox.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3smvabgvg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3isvwtaci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hiuehjwz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mjxudqen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzkksykn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3tcmhprig.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qowqfboo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3omkpxxxp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fuaqdond.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dcsipsqv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ezodygfo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wotzwxpc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pczgqenf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ixwpehst.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wwjtgfes.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3sudrqwir.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jlnfscok.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yqvqkrkn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wipunasa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ywyfkzos.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3odfzfxxa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ypfldoac.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qdkrbrwu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qnjcyjaj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3sruvwgnt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3pfjbhxxk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3slvchfnr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ppygkwvz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lfyqbubv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vvodeang.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3hanftgyw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3htpvlshj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yozukxhq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xqouazeb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnokjibe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vvrbqczc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ixbiitgf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zykdjwdo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3foikympd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fuivpznh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3quhbeebu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vfnbqnyn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xsxguwiz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3crdunqvp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pwzuieez.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xetxadkg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zcivowze.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zblqymcl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nudbvyzn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ustiyuuq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rmeblugd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ziaeqafs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ybyjbthx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3awhkgnwu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qrjzflfy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3znutqnpq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3woteeyuw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3otikesjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvngslpe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3smjqhyds.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3iryzuccm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usucfrnc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rbocydne.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cuwblciw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cepuybak.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dgybgolo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tgibartc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ekbfhkfa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3xleakqad.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yyijrrey.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rqfaupcq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3vergqhfp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qudevack.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vzaekuow.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3bqipjrda.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pdzpmmbe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ngcihqrw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wrcblpfc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3roeaqnhe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ysxdakii.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dugzsjkw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3nqghjjlt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fnozdmqq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3tkgussdk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ymfgjhbt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mqwjszvv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ojpjctgx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jprzoxdl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mtfjygba.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ilbnzrvv.html


<!-- 参考信息 -->