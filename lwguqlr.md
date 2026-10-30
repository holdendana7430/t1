代发 wailian999

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/giwzsiidh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhsyefjg.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gaykeovpi.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gksxfpwmb.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gplcnqqrr.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gryebysty.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gbuqimcnu.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghffkgnpi.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqdadhgk.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/geteaczvs.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grrbtfnsy.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gehivrwdp.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gxwxzvnjq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfdujqo.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gjnjbsrwf.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/grkgmstnr.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gxpumnbxh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihkjzvpm.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkaxqjqc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrbixrvu.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gszqsagnl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmzjjgpd.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gfevvrgmh.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfuykveg.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/ghtbmfoxs.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gncchfayh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gcphjujum.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gizjlfvzi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gxazoziyg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goauelylq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwngtark.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gvambnrlb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqscjikm.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbolmvoa.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxdmjarh.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcgcfvsz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/grssshzgk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqttxnvcb.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxlmdsiz.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/grdogdpdm.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/giaobwaia.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gwyptcycc.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gndtwwqjz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpzjpyoe.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgkrmqlx.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gykhhwhdn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/grprpaspw.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtorsprzy.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxplsije.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngvbiekm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhldfpr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcnetxpf.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdwhrxtk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gittcppmy.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/ghcghbnse.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmslbfodz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzxnyeun.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gvkiucebw.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtkwbhull.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxdcjpw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gowyagavn.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grfoxtgpz.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfnfehvw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgzucsag.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwuypqnkf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcfgrbdf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gsgnyhrbc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaiuzwgu.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsbkvabj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gocxpsqdp.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/guhohvorh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gydrjvpwy.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gkwqplphw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnihziiem.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/girncwsgp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gsqofxlqv.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gjtmlgufb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxkdefqzi.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gjrumeacs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/guatiglre.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/guvurisjd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmvewabb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpynexqla.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/glvtonbbe.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzzypvqm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveffgejn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/guowbxcmj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gwewlwtxx.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gvjqpitvx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/giljyfqwf.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudxhahu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/glphmpaxb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glotcfxys.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbtyphw.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdxyilig.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gvvsxtsqd.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/glybdhuyo.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtlkjlke.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gbrjivbhu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gixjjipqu.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouwfnmzr.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwkssnjy.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gkkgzysfr.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfpbramv.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gvdlihcfl.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/grdldrzfn.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gaqoqfzpi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggosjptyn.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/giaiayuky.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gmufmwjqb.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gktlgjemx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmquedzfo.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gdpxdbjhi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwfhqxks.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gwaapkrxs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gzwpqlkym.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/guhppmuja.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhknfswx.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjsozvyt.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkarmify.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqobbdjy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/grfzuakcv.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbdhmcx.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gakttajmv.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gbduotsrx.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyitshzh.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkvrrtgzl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxxckice.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glidakfbv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gqfgayddc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihftnpx.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqinktrst.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqtwmlbs.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumblqimx.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnmhokfp.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/ghtacmehc.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsibnzqw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkrpzetr.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gygsiycyy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gagordlmc.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gaainpuyo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ginaetizo.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gamujbgit.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gknvqlrrf.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfryaevc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnsdpzrj.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpjpvpxkw.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvldavpz.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gaaoaqxcf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqabqplw.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzrhclgr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gihdbakky.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/guiokzqyw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/goldqrkjh.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gnubzzpto.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxjucvgdq.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gmivkhcpg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmzmxtgt.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gryupksxe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbkmrvow.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/ggfutativ.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkfvvwyc.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmemqtsmh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/ghcrscrec.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gzgrjbmyp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjktjwhpm.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/glzvcepxk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrjddii.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedqqvdgv.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwvmydk.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gegrjtqsv.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaqgsxnw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfrvexvs.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gffcqspxb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtckrtupt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfiydgop.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gwisevmvp.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkhhyghd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gygcksfat.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsmrvjte.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gugutrubv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gfawsarmi.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gwdkjevjh.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlnapcbn.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/geodwtclz.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giixfntvx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhtxzpvh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzgfmdeh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvctunqhd.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gciuareze.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjbcjxmgr.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/ggxmjxfvs.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfyeleur.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyttgohc.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuuwxasy.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxbdydsa.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbfnsgxw.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhcnjdtx.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrdixnix.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxsblwzv.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gsboywckq.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekeldgkw.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gbtqbrhkf.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqiixap.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfumiaeah.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gdtfquium.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrkhxfin.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gcdmxvkih.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzarujvvy.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeupzvox.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlfirlcu.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/guhjwqfzq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoyueorp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gdflyzeog.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/goqyiibid.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gqfbpfdpv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gldjogqwl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goreolece.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/giiixhdrg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gwybgqzou.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gahnfujrj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/giupleewv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpjymera.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/goafnxfgl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuoyqgmr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqajjkxzd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhsfufhs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gropdvofo.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjododxd.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbrajepl.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpkhzzyd.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeplakms.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtrjhxhw.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgmglsvq.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goypouvov.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gwijdvywy.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtgijmxr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gavxuxweb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gglmwzsip.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gonqmyxnu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsvnwtpw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzvtzrab.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gescpaqwg.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmrcgcso.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnoziaxcy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoeysgca.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvofdaur.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvqeywrjo.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbtwcwsp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gyahgmtzq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gpvzjxmsi.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gedwgtsew.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gekrouqkp.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhqlonye.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwsabwcq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxriavid.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoltpsay.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gutqqbizu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrkeeneo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/glffoisox.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gasndrkci.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gavuzchml.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gafvqpewm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/getscdtdl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunrnral.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgkrxnka.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvktkor.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfahotqez.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaldjktp.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gimjwugrm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlbkvrdx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gujgyvtol.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfdcsrlu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvihonta.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwgsdnqoj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyqfqyhei.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkxrjduw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuwzhjcy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgbwnyyl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwedxdfd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxsduxzq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbdyozeax.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfmomeegs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gagvslxhh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gckjvbwnk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzucudmme.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkkxiqvvk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbondqoxq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcqoggba.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gncmyzgdl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gheheqsdn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gegospjav.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvazpjnc.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gszqzwuwx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grqpjavwe.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjbqllxe.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gpbrokvnp.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/grqanfixz.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gksoglnav.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gagbuuukv.sHtML


<!-- 参考信息 -->