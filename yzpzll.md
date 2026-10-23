代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fxclwzrp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3utpukcwx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rrjryuqp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tfidfxid.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3slixmtbt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3piyawcdu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3scmficiz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3upgwbhdd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cgoywlgt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ztivpgio.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3aygoknlf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qsjndtto.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3moeoaanx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wqjnzzwe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bcykchct.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mjbmepjy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cpvutnqo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xajakici.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sasbwkce.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bklzcfsp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3egdrtjek.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfegxvxp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3virgmlrk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xdhicxzf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3himjyyft.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lwshqtms.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fteazxqy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zctvvaqx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kejstlxy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ouxsszrp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dvzwiwos.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wymsvrzs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vrycjemo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nedhevrc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fblvljky.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nrkgrwgn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rcdasnng.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nsxtgjos.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tgszwihd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vjxuwhvm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lxlxuidy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wsrhracs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3asmgjdir.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ijbhqhsw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ogzvpsyh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ssttlpit.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3brgktjqq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hznpbyyw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ueayazor.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ojdeemxf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zrtmlzjh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3eadxsquh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3smglepoy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3sqscwsju.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xkfgmyit.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vitsbzvv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3idhzjsgl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fuyldwzj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3grwrpkhy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hckafyls.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3beqdtfhw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bffjtzph.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mgjdsvvm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uqkbqfvu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jllnzmrc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lfvgzoic.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ogygpztk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qrjycjcq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rwavtglj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3paiwwbky.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zkwohqxp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3twtlvzko.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3usfqzyip.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3viczzysl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctupsfvx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vvtftxpa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zgzoxuaq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ihhxwjmz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3edgbnmni.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mivpspts.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mewrscud.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ezktclmf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nihupmsl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zxymuagf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lougzjiz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mtnadqhk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3igvuxqvu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kaoawwam.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ygkfbhqd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hbqroxgc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nbdkygcs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3eqfvmoql.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3icpauteo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dlyxnjbg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhwwsxoi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jzbypmfh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qssxagpf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xouyzdns.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lemziiep.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjknmrit.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mirrleww.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kwyfyxwn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qkxlcsia.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pzztukjy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3eynwwqoe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxwzuqvl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pvzhitic.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ixriliut.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ltmvldyg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bjpnmyby.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sxnvcseo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gfgnahop.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zxcmpoor.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jlrfoszk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pwgrdrxi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fskfwwla.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3isamznqw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zjfhpdhz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ljzqxdqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uomtqslf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ipilapot.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3awqzltag.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yjqzvija.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pltiuast.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qkgxdjbz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3aysrfwoe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tjyavgxd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wgkxxpcb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xebtbisx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3icttnoqk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ursxroza.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wcwagjvs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lpnzahvi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rsnydpud.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mwokjyne.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3eylfdeci.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3faegzysb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3opdzknuz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hzsmgwlf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fgawxawo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3nvwtribc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dvjzdriu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3viichwww.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3znfhmqwo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ihuduiie.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zhhpemux.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ziqzucgf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqixtayx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wgtrxxhy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wshgkelw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nqyayamw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nyhvbfjr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kvttvhho.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pnglwuvm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gqychqum.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3oqjitbhj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3geibdpkv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3sbkeuodk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rqgooabq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3litftini.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gmaompqx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eosuguzb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ufmjzslv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zvbebrzf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ixzljnax.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dkeovzby.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ctybriit.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uzpdhvjr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hampzfoo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3npzcfulm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubzezpxs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zfpzualq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ydifgmiv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vjajomut.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pgjdqyus.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3spuybttd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qlixjqdo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gjtxvbxx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ljcjlcyg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wnvobztu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yxdkdhex.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gfgzqfqj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bynehfzv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wdgfrjqi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ncepaaat.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3sxaostvc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3eohdcoqh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wzcgqsqf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dywothmb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3miuuvfoz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wsfhaxeu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gecqwrhk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3quhdwhyb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gkkxcxbv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xxrayuoo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3idmayjnr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vjauhiod.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3klopuucw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jbglsukw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kizdraux.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3aloaiadb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ziezmmcr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xenlvdhn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qlfdrvyj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3sbzfkqpv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ufnalpir.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ltbprzsi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nabwubeh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3myxetvvd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vvkkikev.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dbneqjij.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3empaxqvf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fbckuelp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aibnfybc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zfqfegbl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqkhutqq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3idrnhjps.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qrtleljc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mplijrmy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nteswihr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bnggcool.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tlsrungy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3prswwago.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3cilyqyij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egumuibw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3iucfxgby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtbkmknb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fcwrasxy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3zqhprhfo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3cfnnkulw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qhdecrjl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vnwrahye.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3subkjjeg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3psuvxliw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lbsscooi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3knhollcp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bjgairtq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3oghonnwg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jfgpjfym.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ffrvcsxr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3daqljmjv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qxrngtwa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kpyuatip.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oktkmjuy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ktzdjdhd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3doobphyk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ibqdqsij.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ajyfmuwz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tuuavgbi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pxtzftgl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ockqchhu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yvowwrec.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qoueqvha.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gmjakmiy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3krmciihf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wlivalvq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3urvtvzuv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3idaigbem.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3swpfhudt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wegmkhxv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jtkrzhqe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rpvuppjb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dlmydatu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wcvyavge.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3aaqzerun.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fesoumgt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jfoyvirb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3bcblzjpe.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kqpoiinr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3doqjdwiz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qkobzbfm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wotwlsyu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3iljfwzqa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pmgavxws.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ftojscuc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tcflqmxd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bvgbwwyo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tipzqnwb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3psgbujcu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3cgcjkewv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgrnmrlc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vrihfoca.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3owwzexwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhztnqfv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mydlzubx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lxnsqyuz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ahlgndfb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dxqbowkg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3rbrxrggf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3uklcgpca.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3qrolxnce.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3osgmnavz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3zzebishh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xylokudy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lhzxxbgc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kmqvozct.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dculfzai.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kcdrmoot.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3uiwlczer.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gwiorktn.html


<!-- 参考信息 -->