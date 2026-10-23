代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fqjodcks.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gcscuhmp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nqluacxl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ywldzyng.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nuzthsdc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zkteheuw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hgymjvke.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3grpsvdbd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rarbrxhg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhqyvbc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jvnfylvq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3awfpjnsl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dvsldhgm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jbdjtpws.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ollxmzpe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3txxoagmt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3samobplm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bzjbrhfq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3eyygeims.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qaoprlql.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kptavbca.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qsgtnuzc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pmhzwcmq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3chnpfvun.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zoupfkzw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fuxhzznw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dzjtmjxf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3chawjtxf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rvmaerhg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xvbwehqv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lkwvewad.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rwwvghsz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zsozrcry.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xugwjcxd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rrdzuery.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dbbrgypt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qkxtubpl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhhszj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3radnjxxo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3heyruuer.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aegmhmqf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3euyusrnx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pzqogsgr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rubneaai.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rohfrpcj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gdtcbhre.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hjbhiwjs.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ymrfjonp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3eworzjfe.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yinvgbro.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gzblfghb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wnuqarmf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3valbofol.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kgxmwulo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lyvrleqo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fqjhhxzf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zjgfwhab.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vqstakde.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gszegevr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nlfuyqjw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3msashvfc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jppsmwte.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmyjqcjk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tgvodgtt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3uofezjnu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tbhsxtkh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pxakjxmi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyszavfz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lcwnyfaq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3txbnvewx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ssclvdep.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3eehkvfmo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vjsnntak.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ndvejcdj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mcstkdvh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3owuvfdeq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3bnswjzgj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bznkyadi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zknvnvao.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kdgcaylc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gkfqzysq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ytwqftnh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3extoawzk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjnoxwb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3akfvgugj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3efunroto.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kknmjjra.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ezufhzyo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nbkavxcy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3klsovwom.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ecrhgxob.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3efiumbqh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3srrvspnh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3owsydhwq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ywvkoqbj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kcbjmluh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3olwrufzd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dlcpzmfa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eopculwh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mptdrdjj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zruvowji.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3axuwbvuv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xjxtvqgj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mwwxmhtn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wvczippg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3eulqywjf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3iuuzkxjk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ccesuxti.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3pbaayxxp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3dqfhlekv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qtujzrod.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3apbzuegj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eihzmole.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pomkwwfa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3emlqtlvc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xmcsjkpn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xyhvlgwp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3onzpfvdz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fwxjidtf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iyctdwhy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lsldrkwe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3otwdyvwq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ogoawpuf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3phtcpfdj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ytdapdvb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ogfjklol.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3moiujpxq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xukyxeum.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3oifhyplw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jhsxjoxf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lzpjxaoe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bvorkuzi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3oxmwafpu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3spdgeawk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dmmygqac.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hcfjaume.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fmkpbsag.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rahntogf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3otpymhgt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eojzwtqo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vetyxjvb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3sgxzymbx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dlmelvsm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jzfhrgdb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fjmiojsy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3sbtwxqpx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nyxbgryb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qauphcct.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3tvhynzri.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gykmusxg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rrtngcai.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jwnickgq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ndqnhegp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ptiaoxlq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lcfslbsz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fqxmopcz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hockfqtd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yawalzcz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylrzpmds.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ujbioyhd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ggwhricd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fcwjzfct.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wavicsak.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyatersv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3eajvckqx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dfptluqd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gmwmqlww.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3parppjow.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fyyftbij.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3uolejcer.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3imftcqif.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ixduqpym.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nxxhqwgm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xbzxvehf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zsrcxqrl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yjsqlixk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jkidgqaq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hpuyiopa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fxoyufgf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rdiuntmd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hgyeumcj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3txtzretg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tmsmwdyd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3buiwtstk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yyvqxaua.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlncrti.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hqsugtmr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mdcokrez.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cjmzimib.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3apovphid.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3fhpphixi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fsqudlox.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lfsyxnqt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rnmmgfvj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sjgaklyf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fryawqqv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pegfexqa.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3agbgzzpf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ymqrwedg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okygwjvi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ieplflun.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tqjsicmg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ullmujgf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djiargrq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3enijqwto.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ldmbdgdu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nhsxpnai.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rvurfvoi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3mseinkvr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tdnjrctr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fwjgntgo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gaofzjey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwmomzkv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oitpsijo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwllhizl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3uljffkrv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3axxifslx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qpdwrywv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ldgbhbqc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qcafincr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qaprysxl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kqwoauux.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fwqgdouo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oiclqkrn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rnxpjoem.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xqylhjli.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dyejalxw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pvicvjgr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xkbunxbx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bbxxeonh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zkepmvlf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gzqtbdyz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pbogvfbf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ysjbzszr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rdturchq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tvoapmtc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wfurlxyr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pjtwsnib.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cqncfjdn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3aatrpudq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3oguypbpt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jolhjhmh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hqhqooat.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hlkbtcxu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sojadtnu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lsatmprw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zpjmqpyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwhtqngg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xsswmqmo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ebxjqxuu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fgyqsizq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iubptrtn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3goensnff.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ouxcgutw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3pbqenzwr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lbajccql.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3apfiyots.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dctuylip.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ajwlvaia.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ljswhdvv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3nfbzaicu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iemptupr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3vbgpudtk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ksowmeyq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bvoktqnw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3cxetaiug.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3szmolovg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3uibukwcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojgybbmo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mnwceppb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lghaylza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heazkrpb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3syaystvg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zvenpnxq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hfhjrwjr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3iivdsmhz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3pnpydert.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3cgqrgbwe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3sclprvhm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pwcsrzsx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vphpkvth.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3pozqfwfm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dbbprtnr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jmkutglj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dkoucjsu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pkeubvtr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wswiohsx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3edttzxwm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3uovkybky.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3yquuyxel.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3icmkoaxr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mlqxhyau.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ghomvxdb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3awibxvpy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fzmcvkvk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqrnztdq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wzzttmiz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmvdjqia.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rfvuvmcc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3osmiucge.html


<!-- 参考信息 -->