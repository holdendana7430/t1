代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vonztfoh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3sysnplub.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wjbhzvtx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ziafnkso.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3unfzxdzq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3mjqikcek.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3autkjtli.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hbslcnfx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lbjfritx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3brgscgdh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3jsgascsm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfnicfr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xuvmgdaj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyzdxvc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3aidlpftx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pvngftvq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qrnqykgi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qvscurqi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3dcewhlfe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zxlfntmw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wjbvxzqc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3umcdmcub.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jmustesd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3glywqhsk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ftitvatd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmhovsi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ibmhuntg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rllgiykj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yzfaozjg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3enbubmau.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ogioknvo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3uglyjkft.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmvxvfuu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gpgvdasb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3embblgrw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3homamzxw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fexaljwm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3dffgnrho.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ntuzqhnl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3yidgoljc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zebkxdfm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fejtytpo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dsdbshmx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3efcinjeh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cejmznhg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fvmfqmlf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3pqwvsfcp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xjtcquvs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dnwnribo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ffimegpz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lqplrotu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3btatvvex.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xrjqvhzc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3flnkmizo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kvchxxce.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3myghftbu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rdezxbsa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3szcvkzel.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3dnpzkyio.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kjcpkyrz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3buvywghr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vxzqitwx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lxkmbopy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3waskhbbx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ikczpxfg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tsrxoqbf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ywqztayd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fdfnpnfv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3epttwejb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mdmlodkl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bvooznnw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pwdzcspa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kybqrboz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hozqtrrk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3eruajjol.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3smbrmgyf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tisavkwm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hattkckj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bdqirxey.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3khltkxzp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dddmyacw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3txdsjufl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3neajflqy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkpdntft.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3izhsogek.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3syukinpv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3abbyqjqr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3eohafdlj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ifhwejme.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wjlbagvx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3onupvzap.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3eejsxzmg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qnxmvxyy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mnprubzt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3caiananv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ocvaqnip.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mdhuuzfl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tghrbvlo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vsowcxrz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ytpdrshg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3disbpaob.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nfvfwgzv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dpccarfg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3otjxkpor.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bnbbkizj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vmfbfvvl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wvwgxozi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tbabtwsb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jblvyrvj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3piaxoqad.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gythbppb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dezmpjiy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wttcmslj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3eirnmirs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwhvkykk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rpveqdhp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3imzywrou.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gewjspfa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3snikcdsc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkllwvku.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3mqtaaysp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3koqdjgjj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nwbmlacv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3roaylusa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bplizwtv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qgjeffuf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3imnnbaiv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wwbaedff.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vuubpyqz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ualztkpy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rwrywbcw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ydrcegga.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qcjtpaok.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dbzivuld.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3voxdzhne.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pogiqvun.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3dkfdfkye.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ipuokyqi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ttxlfbqz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wrifioar.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fcbougmg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ddmrzjsp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gzqevnvy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xkrpizwv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xuahzkhl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oqwfjyfl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ldgeoapl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3guvuzfik.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xzgjqrmj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zvynmded.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rjzqcfao.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ttfwvdrv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lccfzmxt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yzvzudms.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lgywtlxl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yrxqheod.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ynughydu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nlgbeswr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3npneypzi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hrhavsea.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3phnpesmu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3oczyfeyj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xjhpftcx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ihxfzcoq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gdoxstyc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gpkhxhkr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yingcloo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xdwdvptn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ldtgxztu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3btcsvrhu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rmbpcied.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ffyvaelg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jbixymmg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wtzbvmde.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hreskwah.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3abpsjfxq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3inbbkvih.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rckohxwx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fhlbxdbx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gtjbtbpq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kzqdpmgw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xoxkwnfp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xfpngtva.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3niuyvgfd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mdgebqwa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jwvnmwdt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kmmdzbwo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3cntvsgkg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nbqqduiy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lzkydpia.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gopaxztq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gnxvseni.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3njxprgur.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pwnnqexf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qnogkkbg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dgxptsne.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lbbesays.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nqdbffqz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wtpfbyfa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wnlvekfz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bcqgjkva.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fcivxwid.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sqzxwltg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3avsqfcfk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xcaxyfgp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3geribmug.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3csdojblw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3evyimvbv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3odcmnbgh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3owqbptcs.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yifzyjin.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ipaqfoco.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tbvwxsrf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jfwcxxun.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3aklqtpsx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntesfaak.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nqxculxs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uzqossue.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3aruezead.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3socyxrlm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3iggmdxkf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jhbbhxti.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xsnluxmq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3caewvyml.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3zkiewhrt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lxziscvs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qzbyffoq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3smhsbxff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auztvper.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vdtkadhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yskxqpbv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3egsptpag.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wmeipyay.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3nfubvuok.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zsfhkrmy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3iodfxmne.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3izqkhgbb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3evljiltw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3viivopfq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ksvdabdk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ckzjxchp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rgwarxon.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rxkyiklu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vfahmffv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vuxkgkvu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hfwygpsp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lrddeter.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kwfinzak.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dmmedtwe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qhpxcyru.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xaepptao.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tmnjegzs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xdwiqpgr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3luhhuslj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3etvmypop.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3spcqjxmq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nfyhxxgy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ubojciri.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dbokgytx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3frkledjx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xnrqvusw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nhmptcgb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mxulznsf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ppehxxna.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ehxvyqvh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mdpalwxb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3skwalnnt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jfjrnwme.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ojtugvpn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3lqxwcmek.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dntbdamu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gincubin.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ipxrjacy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oxcsvixc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rkrfrxsx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bqzcpiqm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rnwdwdqq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wrpznxoa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rzafmlma.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vdcmjhqn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xpyafusz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3otnwrqry.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3iyrrihvw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hivmrebq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbbknvis.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3sziwfmms.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lupaczzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozhfueiu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3szypvtwh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zurkrphu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3cxdsrbmv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3qiwswkzs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3dmxzzycc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gqxzrpnf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3wxfaddki.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3otsgvvnw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jxlcjdkz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3zefpgdwi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3oojayntj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vprjzhxq.html


<!-- 参考信息 -->