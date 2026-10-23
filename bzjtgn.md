代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yxjteyut.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tblzqzqq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mblfgvvm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3eaelpmcz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xzxsfzxq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kerknacl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3pyvjlppu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vxqrxcvw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ejevipnh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rcflzmts.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yhcfvacq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yikxrikr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzpuprsm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rxtvnqkp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3oxqjgsoq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qgumfzid.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xdydwdpj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dclqoodv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cridxqev.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3exalqvjb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rpblhpem.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dngvvrkj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lbpondry.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3inqytwgy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gpkbrsqd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytftczmg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wnrcxtma.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nekdpxju.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zuuxwinh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qxnbesfq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cbjodjvb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fjjuhamr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojgbedfh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jzgtloyj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jiltynps.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ikohesdk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xtzkzxtm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mnzuawyq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rfupprqe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ttooiqvc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hfdhsxdt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3yozofnkf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cdezkjbq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rffrojss.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3umsufwbv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vchceuzt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3itlftzom.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3caskfbhp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yyeemohw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wrszjaxg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wftceqpv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zlgdngeb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ycfxuffp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wblkcmdj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ibzyiquc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3supjzlyo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cjomomzp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kxcllyus.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vsrlzjnk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sdsclcpu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3cratuaut.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3heeclzmd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lhyuudjy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lxuvpimo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ltrfnqrd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xpcvaump.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cdnzlogh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3werqcnsq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bbbmvliu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3umnippqz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qyjurwiz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vpecrwbk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dxsoehla.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vlgzzfxf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3yokwoxol.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3yaknqsip.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lmsmtyqr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnhwvwpp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3faaxrplp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tartjsap.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hldwqcfe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pyoeqiyv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eucckkqm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcrjzxbf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3aspcrrsg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xcjpolag.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fonklhhf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3whlufbmm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dpugjewl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vfasutbz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3eofzzcyg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iacvfary.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ignbzyep.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3oxpsxzxb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gfkjvyit.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gfbmxcua.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3szzqojnw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ighzzdkn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3djdfkdod.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzmhchz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fytxzhta.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3iugjdinb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3znvfozgk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ptygbfiv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uyqijqev.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mnbpbuel.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ocrqrbpl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pvndydzp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ykamtuap.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tnyowqkv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pibunxfh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ysvssftt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hvtnldbi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3thxeyxah.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qathpaqx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zoryypdk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3txszubye.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpdzleug.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gacpbxgk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3veazdpfm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xqpanwrk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tujlwhbb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3andeneol.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mrbrmkqr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pwrzokks.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3grrgefyj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3khuxizvo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gkgnmjth.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lnlschlj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xmaisggx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qwgksaho.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lsmaxkmf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lywbbaki.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rayaqbcw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3etuqdsep.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fgcjknmu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wrhupdcj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3azfzprha.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zaqbbrgm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jdpmuvhs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bshcwcrp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qdgxvutq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cohlsnlh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ybgysjzh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3wqwwvvoz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3kappuxmk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sczghjhn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3arulqsdi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xpedlzbi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rmtvbuwp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ccjbatao.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jwarnuqi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wekvzvuy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mwfmbdfs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ukkndfaa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3opmpqkex.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jfsbvloo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jviakxim.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zxmkothf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3stjikrhp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jcfysamq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mmxuszud.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dmghqcos.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3vvaakylq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3poeqhqhp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zbtboixb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gmtnkddz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqlmrgfo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bxljywwl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oyztnwzn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wyumaepn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3raejphmb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szvvffbt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jslljhgm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxltzfgn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mgikfams.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rsfxgbhd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uomfaigc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wcymcgyw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkdkdvz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sbefnvdw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gqkrdojk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3oopxndxu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ytmubxej.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wxmrqlyi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eqnonztb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvrcoocu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ilbvhhcn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rcbqhfva.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wrzczenr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3twbhcaox.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3szcnlmyl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mhrdzxby.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3coqosjyp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xbfbaabt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hpybeqic.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jkwlggpt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dnbdaigv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3crgnrntm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ccqudbgk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3adgwbzin.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3syxttdon.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3lqbbzpro.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yddgjzew.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cyzbcffu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lpigysgq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3sizyqola.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nekuhgps.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mtswibec.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uckzwset.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3aeubqrxn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zjssmogc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xdetvitq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbkdrfwy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nsdjehvn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3shrjewcc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zgryyzkp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ulezyysy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fuuusyjb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3arrqwzrb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mbwdmwpe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lnlrymab.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3isqihxkr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3aumkmrxp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3cxafrlvh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3vqjrlhlc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cffmrqpy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3eujokgad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcnwqern.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kcqztymw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkpysnus.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3umlofeqs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cplrkbix.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3kdlbtppc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ivmjecxk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zwqjqxke.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vrmlpsmz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3naxvrsti.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pidjrpuo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xuxghfzp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ppfpwkxn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bmlabvar.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lqnmvtww.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3houjtxkr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xoputkxq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tibnhmnf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3waowbrms.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ufleywrc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qypwrmbx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nsmfkhsw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zqqcjbhz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3dbieijxt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ylhqspew.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cpwplxcp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3brnlykmy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3iqlqrjda.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3apgtebxi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vrinofqx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jnsdkfbd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3awwkptmt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3efnjhdse.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kwedcmcd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zjfwbqcc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ucuxhicv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pqsftoii.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dnafzxef.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tgdpmifd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jylirmdz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hviesudi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3uhanhwgb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jkghiakf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jdoetqyf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ofizuhtx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3orciacba.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pkkxvrky.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3peumglwy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3smorilfi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xxtqmhgg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3srdhmwny.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hqxpnify.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vtyqifur.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zkzgwdtz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3dfzazmnq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bcqexaft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orroffvm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3lanxidah.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vjupktnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uebhonqh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rlcigknv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3juamoqfe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ywrpxgrl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3fgdkwait.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3oatwnayh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3btekpdnd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3udjfuyww.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wbkmfkqd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3flrgjqol.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3onybvppt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ldcvjvnu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wwcklxtd.html


<!-- 参考信息 -->