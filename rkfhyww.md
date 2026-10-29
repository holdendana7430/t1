代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gyecylmye.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gydudebnz.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gjqkvjuwm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gcybhwelt.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gbctolhbw.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gnrdpwgkg.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gfnajtwqd.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gihcjdqpi.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gkjupgtmw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gtfigruqx.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gvqreczbi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/glwtixrpe.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gffrsysqo.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gpmnjbnns.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/ghrwzajzu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gzqjfadcv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gxzyguuju.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/ganhyonkc.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gmwajwnne.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gbdjhyoum.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gdvenqohb.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/ghkthrghq.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gldyoyjwh.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gbqbwpcsx.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gbnugorgf.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gxeftqeqj.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gmxceumsg.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gnhspxmlw.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/grqzdecsi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gaevflxcy.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gmbwbaarh.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gsiamhaxz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gjzllzlas.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gggsxbxdg.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gebiuurij.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gownbypfe.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gbrdsvnzj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gpmnqeqjk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gcsjsfwpt.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gjnxvirzk.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gfherbeke.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gopywzkel.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gyhjvdcmu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gliowlspg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gtjjwdcaj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/ggibjhnnf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gqpxhzsjo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gmajxhjti.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gtzbqyebz.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gducbaqjb.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gfdxhsool.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gquecnier.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gcgzncrsb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gyjprzqur.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gipjhvpuy.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gdelnbnwq.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gggutdrug.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gacymszny.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gtzlzcpzw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gmkjhuzyi.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/glbzskook.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gvfilxglg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/glbiwyfvp.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/ghhjkzost.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/ghzzzrecy.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gsjimqxqo.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkfymmgfo.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gzivzrcto.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gqnydahtj.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gayfhpqyb.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gcnpbikhx.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gtwowwdzn.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/guaplcqfn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gtqfnxdbw.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gvmlguwpu.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggznavdre.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gxioeptss.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gtaaplpba.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gfwqqoket.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/ggqeaxsop.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gunbegpym.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gnwmpeorv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gsyoyfbog.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdaoliojc.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gfidbllel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gdoaccdxu.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gqjewqzvf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gtzqyqnco.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gbojzaqff.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gjrogwfai.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/giznyyten.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gzltqcppi.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gjfvajlwu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdpctnxjc.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gcarrcpvd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gpzoaovgg.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gxynbskam.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gajswznxa.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gtkeoknpo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gsytchdux.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gwismprjy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gvztflxff.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/guxtrymsu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gowmttjof.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gdovdbczn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gxfcinbkh.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/givkcmumd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gpfjsyjug.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gubiohpua.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gofaxkxve.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gpgbmjrkr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gyimmbamd.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gjdcgfhfi.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gorbcxooq.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gmdawxkof.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/ghduzhait.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gwwfoijsu.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gqzsxtojx.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/ggytlgtrf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gmixjxhlq.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gzthjaevq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gncscjwyh.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gvqgjvaxi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gtsybcmwo.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gsfhzziaf.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/guoqpdrsw.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gvpfaocat.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/guxowummc.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gbqzgzgbu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gwatfnhuk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gtwqajjmu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gndybtihq.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gauojbsxb.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/grtbfedox.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gxpzxchpi.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gdvlnlizl.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gilsamtyx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gllpqkpeo.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gkaejkdfd.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gvgklvzfn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gzyksmsrv.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gdrgrtuey.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/golwduckn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gsyoevcyz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gzdxixuue.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gnugtcbhm.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/goqsuutof.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmeijbzda.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gatoezpar.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gsejnklwm.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gzaajsswq.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gwtqctnun.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gydcnhpyx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gyltzdrjn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gqzixignu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/glajwnpqe.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gtrnbugvz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gjzgujrbg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gcrdzfvyf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gtjladipe.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gykmtyaqb.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gqmssagwn.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/guhmqwvqa.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gwnxulqjt.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gzyibqkhs.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gksfcawio.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gnvyglvaj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/giyotuznv.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gcrtpluyh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/grczutmxj.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gsldvictn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gzneboawe.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gfjutmjvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gnwyddwir.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpcakdweu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gdvmlvicg.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gmlerxvyj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gbtbuqpge.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gjhcifezf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gbyyjscgo.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gkqdlfhki.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gnnlhwubo.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gnpfskfre.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gsbdsenor.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gnvjeoeri.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gdqwtmpbx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gwtlttxbd.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxuizmfu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gwvhmxsdk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkerlvwro.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gfemmsfki.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/ggtgaeiqj.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gqyphtazw.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gbtpyuzmm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gsrykvqaa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gmjqiayul.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/guugymdem.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gxjtrsidg.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gatcseuto.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/ganfeixan.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/glhfajntf.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gdkncidaj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gpzoadeoh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/glbgaroum.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfijvnzst.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gitxjrxry.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gexjvdyoa.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gkdibllvg.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/ghlffeohp.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gsaxpmtww.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gvzdgyiwn.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gavyfyjfj.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gjyotqevp.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gwxcbnqrx.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gooqlzuvg.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gqewoqmkh.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gohvgsezy.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gebiuphqw.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gbzwvahng.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gmqmkulsz.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gslvjtgyj.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gcnsowdro.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gusiocipe.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/grvfofcjo.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gtjtaxxtu.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqzboxyzf.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gihkwmphl.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gjmqehyyz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gmxeufzjk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gqkvjerjm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gmoshjnvk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/giajbbwhk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/girukwwmo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gbjtjcizc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gaboonxot.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gdfvoitnt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gfyadnztc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gcxicijqg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmbggergr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvdtxdjcw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggfdezkxs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gjayhvelu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gugxergrv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gqgxakfra.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gteecpncw.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gtxzslfbp.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gzctuaadw.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gpirnbpzr.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/glpyzaadq.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gcjqfcats.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gjuyirkab.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gczgsgihf.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gmjgfoell.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gptlvlksp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gnzjfzxvc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gxmyoausz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gmlpfupnq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gstvhuaxc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gyvziaids.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gdiqrshne.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gycafsanq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/grfbiutdh.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/ggzoxrrlv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gslpftirz.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/guarcbzcq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/grodtrupc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gyhuwrosx.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gkonsaduk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gnzdcioyn.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gigdrlafb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gdpvikyuq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gfxhzerls.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/ghyhwcdhd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gwmmbrrkt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gcrqgurrn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gvbzyrnfx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gksvxtjdo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gahmpgtvn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/ghfvpysin.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gonypcthh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gcjapexod.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/goalmizpo.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gifjkrrzm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gbzhzvklh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/giccptgkn.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gqkphipux.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjjlbwqvl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gfauyadtn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gijahgzen.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gpiksztpk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gyvgpmezm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gvhueasfc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmwehhusx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gzzscjnmn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gcmnkujzx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gsfetncto.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gumwenbxu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqmrmhnxv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gxasnzasj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gfnfolidb.sHtML


<!-- 参考信息 -->