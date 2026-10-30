代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gpofzocft.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gxudsbfzc.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gbmwzpwjz.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gjmpwagoc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gmcosopvu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gthcinzat.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gxuarbmpv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gdvpwllif.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gntmqbhjd.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gikrnfewj.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gkcoypcya.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/goimajgts.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gsrlfqwcq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gvlcrtwns.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gmzaxuxiy.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gcczzuufs.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gplszildb.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gwcanxyfm.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gdfhqrcik.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/goyjcrrog.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gvbtjtkut.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/getpocxpy.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/goqewnmcl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gltpogxoi.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gjkgybmgk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gcewcliby.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gdhxxmgbz.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gfpxxdvcp.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gwyftvxnu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gmmrbfgeu.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/ggrutexqr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gttdcbjhx.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gjoixkyjk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gvapibjlk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gtdmiakgi.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gohngunzv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gypryztku.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gebfgoohm.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gkibjwvbc.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gyrefdkjx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gnivlgwna.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gqxdytfdt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gjfixicsb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/geyatnzzj.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gjmtzggry.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gegatgvxx.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gfcbyuisg.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gvlhjojwu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gqgxnspxo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gwrctewrb.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/grqkedpdd.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gokdzmiqr.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gpvphupsh.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/grheuttas.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gaftmmhhv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gogynruvu.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gjlhrkljp.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/geeeaqyfd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gyxbuququ.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gcfzucerw.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gutqvvrwx.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gktjmbpwx.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gyxrsczwx.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gixmcbbdz.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gumwbgyfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gsbikcuqg.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gxisbwbge.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gmcgwfftf.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/ggnwosily.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gixmdmnto.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gnsikmhko.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gfjjuhadx.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gosiqwiko.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gardsekyp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gsyphkomo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gasfxsqqw.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gdabjqhvk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gboqsgabk.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gdqiukhkd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gvbifgfnw.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gnitfyqzx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gixotlmdn.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gvppafdbb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gxveximns.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gvzlopdyv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gkndflezh.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqbinqluj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gwbhbhtxw.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gnsvdjgff.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvxxdytok.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gsdxmaesm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gpuhblfwp.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gmnwnqfmm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtzjfig.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gmycammvt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gpokomelm.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gdxrzovsy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/ghdfwwirw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/glknrvxrs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gyzfljqix.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gmihnkrpq.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gomtxndny.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gaheanuic.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gafssvnts.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/grzunvlsv.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/giaruhwqp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gbgkppgim.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gfruofasd.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gsjwwjmuc.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gbkjjvnqi.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gxubvfrzd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gwujgwvci.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gbnymjcie.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gpaxwhiui.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/ggzxbecbu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gqczoecfc.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gaodlcvch.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gyigdwtpl.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gkwgdpvnw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gbjunbvwo.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gahvfbhin.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gedfrzgyd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/greultzmk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gohrqhdlg.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/ghustpbch.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/ginfzzqez.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/guiozwhka.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gkuyrremv.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gkqdbsgvy.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/ggpmcyykz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/grfmbhine.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gqpjovsxl.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gjjsnhavd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gziefdomp.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gkuqzvapt.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gmmxbfbql.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/grgfhneqi.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gopjvpbsj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/giluqaqkh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcomzlpey.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gaapwqmfs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/grqomefbq.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gojgvlvyg.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsiqslbap.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gkmuknwuu.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gqnhekspb.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gjrwnrrmm.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gsfckprll.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gbgdsdbit.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gzyztigzz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gbxkxslzl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gaxyymubj.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gpzptopwe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gjzszwhka.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gmrwlzgsf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/ggdvjkasu.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gcycnprns.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/glkbstiay.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/grqwwriyh.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/ghopvlaze.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/grpazefzl.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gbbzuaaew.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gjdbrdoja.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gwvmzzdvr.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/grrdztyxt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gnvwlntqb.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/guojrakqt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grnujgwob.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gkcidrxis.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gddokcvsw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzloeqcnd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gkdokevup.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gobazywyh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gyhlfqkfl.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gycbqqzns.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gsbklrbxf.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gehrvtnpt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gkqirkpev.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gbowyjdby.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gftcijrkq.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gplwfihru.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gbhffgcnd.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gklolcfmb.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gzmougmdz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gpfmwjjau.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glzqxamam.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gtalwkcyv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gdhplpehr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gvqmxpssi.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gdnvrvrww.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gvffkosct.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/ggfsrzlcn.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/goxihlefb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gcqcqziol.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gfkbqmyyj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/goiopuiai.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gqkziszug.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gavdwjdkm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/ggvlbawyo.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gqwagobav.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtdimjceg.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gohilyhjr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggaeuqwqe.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gnstfnspe.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gtkucxtkq.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gyfpnjelq.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gflbgppuv.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/ghbkzfcrh.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gfvlzoeuy.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gdnpumdlq.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gmifmylix.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gyerqxhhq.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/grodfyhbg.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/ghnywsexf.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gvtyggilj.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gsqzenniz.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gvuscqdky.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gmlgtvegx.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gctoyanjr.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gmelevkky.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gmejzxyxp.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnhhkjdaq.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gdlxdsmzr.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gmnuvwadz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gwknureck.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gljuwmpcx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gyvbdvqnq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gmhpbinmh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gackxyrcl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/goagvcyre.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/glpbnaqel.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gfqktdgxd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpcocxlyy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtcgzec.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghxkyfvdf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gxyxvpfay.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/guukthdqq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gjtaizdhm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gzyvevfsb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gflmlniva.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gcmnsmgwi.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gxdfwhkac.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gjvtgdeft.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gdcupaapk.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/grubmoari.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzqnuafgh.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/guwxrlgzs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdzwibtsj.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gdhuxxoev.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gxifsgegu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gmemhiyma.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gdzqofcxb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gischjtyl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gpzdjnyvh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbipsoy.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gmedvxykp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjhswnwqp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gasbhnlcr.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gknehrxcb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjldxzovn.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gproopugn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gaxqiymro.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gxayswxqi.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gswysvtuw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/glyplbupy.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gsqtegbbr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gpbcyshxu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gtxohnfqj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gzzbhmccb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gjnyjteyd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gqditajjl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gebgkvdoy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gyvsmzspy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gozrmgoqu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsedhxo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gptfqahrk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/grbhvcquq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gwejggvwh.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/ggwftsiqo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gbvfwskle.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gryepbzwb.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gidapygxr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gbaoeolig.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gexuiodkn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gshrpftqw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfudawsof.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gnfqzwkhv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gwchxdkko.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gjobtxvre.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gijtynurx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gwlaypzav.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gejkhgiuc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gzcexrshd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/goigltpqk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzmyohosx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gstubxydh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gjcljubnx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/glrbjfcpj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gaofvcsqj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwewabkdp.sHtML


<!-- 参考信息 -->