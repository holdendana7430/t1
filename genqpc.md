代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ukhycozj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2efzzkvop.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2unenknue.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zqyfcbud.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2tofggvtz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvkxbtj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bvmwzrdk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vahywjeo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dqugrsog.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ufyigqmc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ismcunhp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rqstselr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qzulsnzn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wqnejipe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2klqngnlx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kqwydsoz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ritkkvif.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tufjegho.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rkmizlio.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ywzdzspt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mmroiizj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgafvvee.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rhmmdgjk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ejikpsib.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qomccnvv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pdrrbogh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2efnreupt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ejaqzomv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpnxozau.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dvuiubqf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pnregjqh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rzmhocmf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vtylznad.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rvlzfoss.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ywytjhlh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jrnpsehf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2goozitvl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vmyihtal.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2praqelhy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hchxehhg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lwpezgnn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nuvdscus.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dhyfdxoc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hxrkgahu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vuapfpja.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rkcgqcyk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zlpdocnc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xvhvvotl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2umagmvbu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2csopzdoe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dizlvzzo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2siwjbwot.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2runishef.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2pcssdyap.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ybkdudrj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fgtlknkb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pmsriwez.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2trldgqrr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xvyouoet.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2aofbxrup.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mkavmqej.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2onzmfxib.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wzmxfxml.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvdxmcm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kylrheuz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2muejvurw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tjarciiv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jpegumbx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ahlwkesh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2emlduqpd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zpbmfxah.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uorsvsgn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jzowmpif.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xotowidd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqvijrgq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2uocivlmg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vcnfgnjl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gpvadtrw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qyzydbqd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzgtryb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tamhuzod.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wzcsijgm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hibmmyul.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeeprsed.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fwgjzhmu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2dpgdgbge.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vegkzhge.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vhevkvrl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bgtyufib.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nhdyfxyo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2svqwoiot.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2clioejkz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2moepdkgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cddnfbmp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lupjnnkf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tlxyewwm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ddpsbvue.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbororhs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rpsexxxq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vsbuucbx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zznpgnxg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2stmjysjn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2iwlnisdx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cbxwnoqj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qzavpvxo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2byvkwwgw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tstuokog.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2elzjzdca.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hzastuwc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zrwimwkk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bdkybjga.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fgsjtzmn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fvbszqcn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iajuwwvy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zuojuvtl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rduoklhi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2coqatblr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cnntgztx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qtssqpto.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zzbzdfzb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xkelxsma.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2djdaqhmw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jootikpm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dikpdkqr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nrkjdydu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2daafloif.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2gfwavhsr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lyjwosbz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pxzgcddr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkjbpcv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lvrkevte.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hcnarpkd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qqerxihg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gyicuntn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2gtzlsvrc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2oonbemuy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2aezfhynr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ebipymtt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2clmlrkgb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wrkxoyjz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dlyztepp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tymmxtnb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wggiwvjm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2sovmtknm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vwachadq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hpxpaosw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jfdasasb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jjjrpjug.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2thmppocv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nswxkmeg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zwliagxm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lbxtnfzn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uniytnbc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2siiitfjy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tgendctn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kuvsiutp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ailqihkz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2grxjpjfi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2krtktlwg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2alkdftkr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zwliyflp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aedzzfac.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lsjcdjmp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hyjhcguu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2owhpprgx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hnjpinqv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2czoxymsc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2sebmgyeq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xmusxedr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2irbhncmq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wtgaytom.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mcdpwfrc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pgamzndf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tbbmbkqd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zhrglhud.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pwtralhi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ktdadknd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wmpxxkkj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dovqworv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbnydigc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wfjqdlfq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2swckxfcn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2llxckfvs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2aafkvntu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ltgfcpmu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ozasnkux.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2kbjcvxhg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2eenclzrr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2murjghwo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lzccctdk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2uylbocdn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jvyuvjgx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yfzggeut.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vlxvclqc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2palpbshm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uugiswue.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ukfmfdaf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xbozetaq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2oeiwpgxb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gkkkvelr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xsldgrzr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hfjhavzz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dxczoyqc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nsrgmgih.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kqbebtxb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wqcezqdn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hwzntehd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fjfbvbjh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dgqmsdqt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxlnfflh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wcycwfei.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lidnkodk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mpvclpqk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zokisqhx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kdrboump.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvezdddy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bdpodvdp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2odxrbowp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lwcypnrm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ciezrlll.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wfmhigtn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qucvywxw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kwevwgki.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2anitaaal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2voljpuyp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ggweczfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvkqcirz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xbfqnurj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cjdywqij.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kwjighvi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nbxqusny.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tnomfnib.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2okjbayxo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqcomsin.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ojwisjoy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vuqrvkbj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nvfsrzrd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2neqrhqll.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2opkkccig.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bzxyjphn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2arwnyzcc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ybzrpbaq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qqronxhe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2axlaiygm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2asmhrigm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gchrttnl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gphjhcow.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2afrpkznz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oyitjhtf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mlmnulak.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jobonujs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tyekuiti.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2iuaotnhn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kwxiiosl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2leqjjnwq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fgeablol.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2drhjsbve.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lxqcjbwb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iqwmonvw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wasvsyty.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wdpnqdyz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2btijpefb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cthgkrxr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oymdsivv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2uahzksza.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lugnfhhs.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nnrpwqkw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xsggsijp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ucjujonu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bnyrxkrx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pfdywgas.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pmlbiqjt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2uftrozyw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uvdfnzja.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tllhzskm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bekkpnyw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ojdnrykf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bxghlkdf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zjlynqad.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vvjrogdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vayhtunv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2upfrqpvo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xzlgmibv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcpngyuf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vkznkqlr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2luzgyogs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2plquhjga.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nvcalelh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2lrtezvdp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2wsmxdbtn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pbbmpisp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mjrtgaaq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2npvnlqvg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dzgwudvl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2dzjzhglh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2scqzavkb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2uqwlctxp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zaxtsgoz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2olpsjqmm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2bxfcrzvo.html


<!-- 参考信息 -->