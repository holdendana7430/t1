代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gpkcrkewz.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gqtgytqqe.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gbkzlrivi.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gabjatdrz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gezfyzktn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gkuwbyyrt.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gelqhumhu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqlvkjq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gucnrvemq.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gjvmhbzdy.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/goenhhknw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gureeszvy.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gxdbcmedk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/ghubtgzzw.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/glcjnrtzj.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gykwkudpv.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gucbscibk.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/ggyzbwzqg.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gboxngtfg.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gfevgmaka.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gmsxyqzuz.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/grclhghds.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gkcomvspg.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gkgmudkcd.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gejgfogbe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gondgbevr.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gapiltaup.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gubvxpund.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gzsajsywu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gvjmueefu.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gvhmsmbzy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gpyoutzfa.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gygoryovu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gnclirdmc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gixqhbodg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gknhfojhy.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gftlwuuhe.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gdtffgrnp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gjjovdzsg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gbnhecowe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gpuvqupsa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/ggkxohbtd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gbicveqhz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gkflhpbgd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gunjeakgh.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/ggvzujhjs.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gcplatbhy.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gychjligd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/glqzgvnxf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gngmkzczg.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gpymmoowb.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/geeptaezp.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtfbqnqun.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/ghxqjnsug.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gazfcifqc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gttnkvkos.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/ghnirmoep.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/giswdbywy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gtollbqlx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gtqzoejus.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gqsaidplc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gcajumacq.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gragxuhjw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gcwreepzh.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gaztokflv.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gkcbzkefm.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/galkmmwzu.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gggtlrlna.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gunzqwjjf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gbgmdsptf.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gjztjbcpw.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gkahwutmh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnhhbmnhw.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gbkfmdeob.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/ghlzaggoa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfsygjofk.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gdrrnfyjn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gqzkxpqvr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gsbekstss.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gzwlychvc.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gwmhbntzz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gpatpipul.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gjbnikzni.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gzkcoivls.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gpgcwmqsl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gntcrpwct.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gwpozivxd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gpsjvkptc.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/givpjijzr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gtklggequ.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gglpfhgkt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmsrtguzy.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gdomattvz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/grcktgler.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gqkytzmmv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gvfrfokix.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gyjyjtrxm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gmmvhjgmi.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gejhtahoq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gbgaswkgk.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gclxnugsk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gqlcayjqe.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gvrqypplc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gcmjeabun.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gsetgqrzj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gasvrxjcs.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gijthdhxf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gfsfojztv.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gkzapytug.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/ggcpqssnj.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gjptfspkm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyfnekon.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gwhjoowrr.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gbsnjebqs.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gyvusgiqz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gyieaqejy.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gismqglyt.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gphxsqvoy.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gxaltordc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/golfpsbfx.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gqehabhhe.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gfgepbsjx.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gdvjouwnn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gifnufeha.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gqijunths.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ggkznjejb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gkksqvrcn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gqcbxruva.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/grfqstdoq.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gsirjunem.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gxutmbfzy.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/ggocgrnex.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gxofvzljr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gzsbrlokt.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gcfcuastu.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gtruwopcc.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gimvmmqeu.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ghhtlraed.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gmxewgtth.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gxluxbuiv.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gbemhvmkw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gdsyvuzyo.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gotgxmbyi.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyceehlmd.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsloalkww.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gatazrubm.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhvsihe.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gzzvspvcy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gkcslgzsw.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gatzizhwy.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/glvxrdadb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gowpxywst.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/guzuijwvc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gjcowirza.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gktodvjyy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gkbaptkcr.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gciqsojdt.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/geaicoeag.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gvhmlmebo.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gvehcskav.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gxdniddjs.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gbbfnrkma.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gugpqhjag.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/grzlnwlhv.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gbphypsos.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gcpbztzvy.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gfmqmgdjb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gvgccrlpo.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gvitycjfo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gulknxdrl.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gznqbfcbc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gewevabzf.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/grtgnvebo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gpvnoukvi.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gljfsjxaq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gvyakwqmw.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gfdgatjxp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gcqstlmkb.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gklinuaro.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gqwgdanzr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gmzsyqlmw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gkmzmervo.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gtyknrdbc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/grktsnquh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gfdgsajew.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmnkbdvqi.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gbivjoaaq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gkmndtnrs.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gupszzuvw.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ghsydttca.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gazagjbxg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/glncicqie.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gnmqdhwsb.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/graweqfuo.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gzijjsdqe.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gfxphargp.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/ggtmarpmm.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/ghusvqniz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gwmfbnauu.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gcrtivdpw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxbiillmn.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gyqxvomht.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gevmmannu.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gmkfodhve.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gswrzwqsx.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gmwfwfqji.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gjhpvhvei.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gdhfvezuo.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gzoittrce.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gcidieske.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gaxdnyvdp.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gughqddyl.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/grjarljte.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/ggqdbvjgw.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gvkvxraji.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gbnsldvdo.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gspujyacm.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gneobspxb.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/guocwogfv.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gwmucydow.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gsokznror.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gjgwexydt.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gxoeadcik.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gajxfdtsl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gjtllfryz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/goxwbdlrb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gitvdbpiu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gpymcnzry.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/glotgriic.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gohkqxgrx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ggsjbyqlq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/ggrtvpnxv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gjvkzmead.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gburxkbuq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwzhkjkrj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gshsaueqr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gmxjmmqbs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gsljtswmk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/giycjcbqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gyfllguan.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gesfzwfss.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gjmxcqgam.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gsyroefcb.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/guahcvnlo.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gocofwahc.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbdcuqhff.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gqpnlgioo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghpaoscgu.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/ggeqpuwuh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gedwzvmlk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gwomejezn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gudlmxuqy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gxspmvkpd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gtcpwpshl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbpvtgiyj.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gebrafvff.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goejwuiys.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gzicomfvm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gldcqdecp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcvvrybkv.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gsghurhbv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gxkezcdut.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gbrovjybs.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gjgthgnim.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gunzjezrc.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gbuoplval.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/glwrvlyaa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gydbbqzhh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gyanwbrth.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/ghhlznapp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/grtvtzpon.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gvqbjfsof.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gweuafztk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gtbznmyhk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gufxepueu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gxhhaoqyv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gfknaegkq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gkwoszrus.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gwuiobmff.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gomybcnqb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvigzbzkw.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gzhxqcttc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gkqpmkkib.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ganqwzxrv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gwxlovihi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gcfgrnplx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gbzxiwtoa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gjvvmztlh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvfceubfj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnpnlamgo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gtlgigdnq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gpznrlbyh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gymcmmivb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjzugnrnq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwpuonoes.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggicmxzel.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gljslejnf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/glcgomcmr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gfhkvqllh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/ggkvnchca.sHtML


<!-- 参考信息 -->