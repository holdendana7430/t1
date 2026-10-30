代发 wailian999

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbkfwcso.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbjqakou.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkihxwgu.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwknmykj.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbloilpah.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhuhickc.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gqycuvnno.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghihfmkuc.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/goifyqeyc.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gbohydlsi.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgbndlwx.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgeapuwe.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/goioznjog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwgezpes.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/glbvokwpq.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/giszwasff.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvgmtdcs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukztckxn.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gorbuwqdz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxdpqysl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysvmzqcl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gwlmlnltl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjilmmxgb.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyunfpqt.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvsqlueb.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gjlsteenq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymkegyca.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gyjqmcmlm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gzwuwxghq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdvdkuwy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhpsvmmr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeowjysx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gnjbwhnzs.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvsrzqry.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gskkikgqy.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/goromdesc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmmphcww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwqlldng.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkagcwixh.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmnovmpg.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfumxemkz.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gqsgtcytr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkuveucp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnjepyct.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gkloncjlz.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/goofpkviv.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsaotxvz.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeibdqes.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griycdksm.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrcoycgc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrwcfvem.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gctdlqcae.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdqowikz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/grocxwxuw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gytgdgqml.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gffxenawn.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntktyza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gzbvmchge.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtflmqudt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijdekseg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gupiqamlk.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdzreuvr.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gibobdqjz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gvflkirng.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyaxsxtx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gozxnvntr.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gyfedqbry.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gybceqadh.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/giajtaohh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbdcjbcz.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/glebjinvz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlzmiveg.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzfzqjzo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkrjqeap.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtnojpsi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gopzomzhn.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/ganneszqu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyjtucwlc.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgqwtlgs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gckdiyefq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gzgkecklf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gmuwqsxud.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/giiusacxv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gkgxccldk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfsgrvcd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glziorhez.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gldeuxeby.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gtarotujx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdvjsaou.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkbnuphe.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gdmzgqruh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxucitgo.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmmhfsrn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gdwswwgxe.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcqsezfy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmtkmvw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygklnsqw.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gddcrqykg.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gzpacbwbg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbrpfdgi.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gknhvbpes.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/ggxzmpxiz.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhusuhev.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gthnzxorj.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gqdbjewrw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbsuwikm.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gumueylpi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gliojxzux.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/geqdhkcsf.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gvfowsznz.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/glttpzuzz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ginaffotd.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gruwsptsc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gjbtvcmrk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjgikrzo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gselqacuj.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gpmxwgcjh.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/ghhysfwpt.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gmofseelh.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/geivmdaez.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqdtjtna.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gzylzoijx.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdmqaaip.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlvvqykc.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gygybyykf.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gplqkfena.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfyxjisgy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkdrblgx.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gzawhxqjy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gpanuugqf.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gunxhfddl.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grghlahyb.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmgqyypma.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gljulflim.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvqbnyy.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdqyqbhx.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/ggacaqvcj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/grnqsrhem.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzvoqqla.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdeupwsm.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/grgtoofxz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyvalbyr.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gzcujwowm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/goylyrpra.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrlpumfd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/grbpoqcxq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwuhmbzv.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpogswuk.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuhyktip.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gslmqwdiw.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gamvkbidf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/ggqgwvadl.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gfzmivorn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhefrzol.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/ggaznsalc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfmmzdt.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzbvhqzn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gtomllbmw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbukcvsb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxowikye.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltermhlf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gznqizmpj.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuzffwqi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gmuxdfcba.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghltnklub.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurfnfmyw.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gdunzeons.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gtnsshlpy.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdssqgxgz.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpulziesd.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gtjhwcopj.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gkarojjfl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwounhxgb.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gauuseiei.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeagouvm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwpyfkkz.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gkyyxprzf.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzegvmnf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdsyunvt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gadmshgey.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkbqhnth.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gfrlzokcj.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gysdnablg.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gxljdhnxo.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gmvtoztzb.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwtlmomn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gkopsfvde.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganyekrme.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqnturd.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguaienln.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkarbrviv.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuiiqrsl.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbufsxcw.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gteyitjxc.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ghyqhqdyg.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzofjozr.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gnmbnfnpz.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gqvjqcnxb.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gubktpacg.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmguesy.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbegugdkz.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gycwjwvki.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqqhicgc.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gywrljjnw.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/guzgdkrfx.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gmqghgfnh.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbnjvdwj.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/glxebyujs.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/ggrmaiclj.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahnzwrjo.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/grnzcdqxf.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gmdotjqpi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrokqzrq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/geoearhrr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevhpiofk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gryyxspfe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxjpxoii.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gkumncazc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gimmtaqsp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpukpeui.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaefqmjm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjpjwspr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gipdllhlc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gxzubhzlb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gvdimsaxc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbpupkkk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxwogjzt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gpxrrfhhc.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gdybpwxry.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gdkymevrr.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvmerjtz.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gcfauuqjr.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/guytxmjcz.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckwjcxfs.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gftrefawq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfprumlfx.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopfllbmw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gezcthnfj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glicslyda.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhkibisk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gdlorwvfl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/glbcrncro.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gkzowhllu.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnuohlba.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzstorgmv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gxwvqcljk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmsxbcvf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfgjzafk.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/grpmnmzef.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptgdogps.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gadfeilkt.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxroqbyc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gziehjyja.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/givnrwtxw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gmdorisel.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlcieith.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gzaxicsdf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhmlrxwc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gwpftpsoj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkzkvysn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepfvkfwy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guocuract.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxhyqjnm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gainnjbkk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gmjguizfg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/glbdnsfip.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlwrkjqe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzhqagzv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqopbslo.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gwpmuexyz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gvlzpskgd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gtewljrrf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnsgosfpv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdilaqenc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghomegtjc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gfrwhfduh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpikvjwz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gekzlsoih.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giggfoxvl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghsncmavp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqdncbyy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfbadojpw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjblnyxp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwuwbxll.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvfecwk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvnzfajth.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktwhtehs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggctfxred.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guywqjaru.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gusisecuk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gwhwoaaki.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gftuyjdvt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grwqsiokp.sHtML

A. 基础语法与类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwwbnmvz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzoqrjdm.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/girufmclb.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjpiqmmt.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjftzltb.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gaxasjelv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzdutvsp.sHtML


<!-- 参考信息 -->