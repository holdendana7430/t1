代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kxistqaw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3iwhjcjdw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hasglula.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ingcdpxj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nudytfiq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3blarcuaj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3tywdhwib.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vcozjofj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3erutbkgw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rsjpucfh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xbbplzwy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fnevgooz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vyyiwmwx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqvmojc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ynboyctf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzajryg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fayjudup.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3buwmotdi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mzfiaako.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jcqxyvzt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bdymtegc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tscfsqfg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kxdofrjm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pvnpbyyt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3knctffps.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3navmhxqj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3prwmrciz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ttpddcjd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3bwlskgyj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzbakafc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rnsodsya.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tpavwggt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3shcymwap.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3avvrhuqc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wggvakzn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vgprqoho.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3znwryjhy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3diivkjdb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jzqgonzb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3whfeelge.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3enjzwdmj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3btbhryyj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3yrwaaqvg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3oxhnpjnt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tzxkbvpm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fepqyhzw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kukvlebs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3nydpdizc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bhtogqmg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3duaxsxsu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pareftss.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pozxhrcw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3irwzvdcy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3liebxilj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kqdlccbe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3pdqgfpmr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3feykumgw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3spqaxvdh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ilfrbsfr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3nbofrbqd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3aoosdhze.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qerxltih.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lzefyizd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3naprsdvt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3msatdhqu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lloitjca.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3orcfgxcw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3whptsxpa.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3akuzkgau.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3thhbdtry.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xoasyaho.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3glejadqg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ofiehzqi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gqkeolqm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ipmdcnav.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qhldckvq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dihamsmg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3imkmwihv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3duyjbogu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3gkvpjbbh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nzavlpud.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgcpuyrv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hxevcsmr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3rbvlidlp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zhlpjpph.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dxnjwtgx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nkpcxkku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swzqqhwb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3akbdxzmr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dldiffxw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hkjvlrfg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cvtzotlk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3sevmioaa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zishieus.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lrmfncem.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3caosktyd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vcwodfub.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tgigedxa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ipxhavaz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3etninzla.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rqcxjsen.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vsejobgs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3phnfuort.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klfcutgv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3knxkamzk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvjbafwt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dgtxirek.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lhcsfnpd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rrecfycy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kxgzvzix.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cfaittjp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hpwbfize.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbhxkc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qqfrbzft.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vfctsnnl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nsyjiagx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tlbkbovn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pvcpktaq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xdwkskex.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dhumqoaa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kptjfnlr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3faqwskzc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3anazsnew.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rqksekgs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zfwhnasj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3uhhaslkd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wzpaosmx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ehigioum.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ghcwjtfl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3yssgfmlw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kcxgyley.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ihnpmxyl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qdjfpafc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pwhvffas.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zjossbtu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3soevjfot.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oamacdtc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbksfvc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kfntxiri.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3yicrzzfy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qgofpxbi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gilhcpku.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zjncqipx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jikbfkin.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lcvsfida.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fieewhou.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kvmsotkh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wzentwsc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jedaropk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zasqujsf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hitnwwrr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jvbwmvqr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3revljxmb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pmluymrc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3vjeklyum.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mzawnbkt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pghbahem.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3asjtajme.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wupaunau.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rbukwxwj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ihtwrlxi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ecmrtqmp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3oqphhtph.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3icijhxqh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3csvibnrj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rvvjugev.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cjrusyrx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vqaycjgw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3aqhclsfk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bxtlhnml.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ovkmvmbi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrifeaqm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dbziwcvb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bccxqsgq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xwsafkfa.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwruajpd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3angzwmua.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ernyihwl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eyrmohge.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mjfmhfos.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rtfqdnly.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vdyybetn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wwddpjzy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibsbyuda.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bnzudjiu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qhzyowya.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pmsjmzlf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nrhbtnbt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3doxmjxdt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3duromwzz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3idclpxtp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wodsjhhs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3oyajmoiq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xvrvooxj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3efaonfgo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ihhthlmh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kchgtmrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zunripyy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3haopqhsw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ukyvetpu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ulcplldg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oxrygtij.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kcrxwsqp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vutmstfz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jujldehw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ancfnkiw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pwmlxehb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nvadctbo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fdvcxwvo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iwcnnekh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ivkgaqev.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bjjyxtjp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3haqfkpyu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xooucxou.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zjvkmpao.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zirnyhpe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3phlzbnyt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ojskzlaq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mxegftye.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zunyazxe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zmrqyniu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rkjpcudz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zlwnmzti.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgpidbys.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oysitarw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ruuyitqq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mgkvkypn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fqinxnod.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dflafczr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3oumjcipi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mknmysfb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ugnjuhon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvkqchak.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3imagnlsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmykrcgg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vdcubxfy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3edlhxlnj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wpmimgae.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iwxrlxmr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fyymgxjb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xcddktsk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bfyogdfd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kkjekwuu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bwwdltha.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gnyjhgls.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ctxvreqc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3etslzwud.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mrahorhd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3aspvkryp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nrexapkz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ptmlvslh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tqkoqiqy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fugkvgez.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ynqosgdw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3bzwtcbqc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3fjccchvc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tdwengnc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3siiqnmpa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mtoefojb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tjkwglyi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cmuujqjd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qrmfnogl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ytqzgxds.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oiacwqbg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mktrywkg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3joacemmi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bpuevqek.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3flbteszn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gowltmzg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mahqicru.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vgeijrgi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3trzcdmlz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kvgkjcnv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vlnqalwn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3yejeepmy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ayqketss.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zsmccejf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zcucbjgn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fpnsruyg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xhhmhtgt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xtoeabrv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3boxeopyd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mmveudft.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3girsfkbk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3btxpwksh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gxtljeny.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mpizfbav.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3uoovjxjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuotohhl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ggyjblkr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pvxbthmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isuskomg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ypslcnqz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cmnvicik.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lxphtead.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3eyismqxf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nxmdmfhm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tdmwvgvq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3svtyrzny.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3zfzhdlmf.html


<!-- 参考信息 -->