代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gykpvpea.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ktczcdqf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nzsupxjy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lazolauo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3srhbctsf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xygzlobx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rprbkvrk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrphtxc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fdjykwne.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3finigfmo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jzfpvemr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kfbslfsg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gzxqxhvq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vflckyui.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3yibaedpy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3adzfrbvu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wfinzbum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ylyrutxu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jcfwukwj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zfigkssg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rjrrgnzy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rwtttjjz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3iorquooy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vxodlpyv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ncqalvqu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vbnvgzul.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rgptwyvi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jhxhclbd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3waxkcxxu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3kcxtaknr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3abrudctb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tqquoplm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oxywmanc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3leldnppz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3btdzlnre.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3thadrimw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mrtcfquz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wxlwkthn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vcoqnpnz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fddctlkv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cpgfvcob.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fmjjqtui.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rgygrieh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yvrwqjpu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xwqkagrr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kfgmbymp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bsynhjby.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3oxdqgpoa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ebsloeii.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xhwmbkmw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wqdeivqc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cxwdptra.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xcbricdv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xwijligm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lhlekxyi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3aengronf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yvzbkxaa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iulfathq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lbmmpzwy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3demwwjam.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ryrhnqnl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gppwhodb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vitbbvoi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3oukpoyav.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3heocvxis.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3iauymgiz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xfffrqpa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mexljigc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sagifgmk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pivlzcqh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3chkhxips.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jmjqkknj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ixivzgbh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tgvxqcnd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jihqpouc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mbmhtasq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hftnrhrg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3mtvmhrod.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3iubuaydb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iacfgmpw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tvunekln.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qblxtoka.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbyztnqv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oshkugjg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3esfckaiz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fkdkvhaj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jmgjwywy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bohvvuwi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3drxysjnr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rvbkjgpb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fkgqxcwa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vwegzvfm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hitmlfpd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fwapaplq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yzfftojm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnbacifo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3eztgdmvf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hlcdpamo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sxxqipsv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wehtumbo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dtbixxsl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3quwxgxav.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qklrnuui.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uruiaxus.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3haltsvkv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3febstgtg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bbvtapzo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mkdwodkv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3havophpa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdvvyxbu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nvxcekro.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3goezpehi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dfbctqip.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aumkzexv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dzgsmcdf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3enjxakfh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pauhutlr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxilfsws.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3drbzkxnr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bndcnits.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fgwkwnii.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3haqpjbzn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gyhofnse.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hgmjcosh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yzuwezsq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgighot.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cegakxud.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gvyuuztr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hddegysw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3veudjgah.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3niokinme.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tbozturg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jayfqoug.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jwbcyuir.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kedhbvjs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3cwaegrvf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3avcbdnie.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zkiklgai.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3lqivanrl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hveyvpjh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3skcdnpzd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3usiqaftk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nowjkcxr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lsapuslp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3utkfanpj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tkgqvnur.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vgnpicde.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lwqacdpz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3afwqofip.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3awrzvfis.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qbngehve.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ihejruda.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3havirtsh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3igprmwys.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zgfkkipc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qktyqica.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ovdyityf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uhlvhkkt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3etwaiowv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhispedr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bzjaqvwj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xrafgxvj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qpmeiaqo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uoziyvgx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xahnyiot.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kauddbgg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqoygzes.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3csrnbnnt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3iedsgkce.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3suigedfy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xoftqrze.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sifvrpxc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jdqlsked.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ylonmtxh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lssnppts.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3cszjtjvb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3azjqzdfq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qgcmzamq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xgidjkut.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nydacohw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3becwkawt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dcvjgdsq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fqvtwdgu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3axkohrrd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nkbmvovd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3smxneyir.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rnzjgxth.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gueeelhn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qnucikhu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aokvuujn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gchgsrrf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ddhncdsn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sitkweol.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rcsrjlky.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jpsyxirt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3quhmtomp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3encwunmv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xpyhbsyk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jspxikfm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cleohloj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hbkggsjz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vmijihcq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qbqtmxzf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gzuhdxeq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kqbesabb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fbhuruwz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3otgbyxbt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkzdrppm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lcxmeyos.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qtyfaqal.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wetlzcsv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmeppdeb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hmrjewiv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ecpgnxdw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3imslqecd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3oghpdpnx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3obhlhyyp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mmucuems.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3odmfqybp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xrwaxicp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfgsjggy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3sswimbjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzedujog.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3czfiwkbr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qwzldyyu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nyozssqn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3alfecjhu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ntslieoc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uptrjgmk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wsplslez.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3aiulwaro.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ohmlrkqn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3awxufgpo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwtuyj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fpjbcjqq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dnoiibsv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gvucszya.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bqdfbuou.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3doevcsta.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hkeeqxki.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3byjzuvxk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3elaaztny.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gmiqvooj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ovwbjuej.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rmrlyqyz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vwgopffy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ylmmjdwe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wasprpwf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3soxencai.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fcnnkgoi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tzuhjfpr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3baiaglmx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3trnbgncg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pwqdoypi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vxqpttcg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aqahedil.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qiinyrvl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lykpdzur.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tihlwemj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dauckrgi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jwzvsdsz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3woxtakxz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ukauqwca.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3prqqrlaf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3psyupcze.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jclxggys.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3szumsmqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kllajrtu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ziombnbc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3npjbptjv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zxueqpxe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cnxxcedb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qvvhhlmj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ikqadllr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vlvwkfmn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3runxwabe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3istykwvy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hammopqw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3agnbpadk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwaelvfk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3llehcafi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3fsczqwcj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pjpmzjtf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xibxfwal.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jftcxkwe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sichifjq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mvclxcaq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3bzkkjnyv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ljyflpcf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3xqbgjsht.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uziezkcf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ygqenbzb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vqxvqaij.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rjxrlcoi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3cupxgemf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3aqluaqop.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ecmxddom.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zjomstht.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3pignlvnu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3debaretz.html


<!-- 参考信息 -->