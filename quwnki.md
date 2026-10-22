代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gzqvhhhr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ffqbbpai.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xrkbzvph.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vkrfnild.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljacbstd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cfkrgvtu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2piofhxum.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqzflof.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2iixjagds.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vpetfaop.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ismpzpkw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cpiiwtyn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qqnqekbx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2knveopsw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yqiecddz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2itkvvhsx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2uvhlaigh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gitorkxy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jkokecmp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rmgvawnj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vygnjcmu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hrqntxzw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2coalhrcz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uevogyis.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hfbihfqk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yksjmlup.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ranhrmaq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ubbpexjc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2odhcubet.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnprtbi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qcxdlwsj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2olrbihoo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kboyjltg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lallxkwn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lpxigeme.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vcehokle.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bnxgihvg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yndmhtjo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ydukrixc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfknxqg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2plycdrde.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vrrlipei.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2atehzrnf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rlwbdjdp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ycabdlof.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jkguhnrx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cqmxoiiw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ckxjxpjs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2krygieoa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ltwxtbmy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tctpdkcq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lmilpdkj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rreebsob.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gqieavle.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vbkpxqsu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfnekar.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dkdjztcn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2foqdpein.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yjpwaubt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2svfkrjta.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nkfzbhfw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kwwonxxh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2klkfyeyd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bloknvcj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2kmnxndhi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tavhknxr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2yihxdlud.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ysbtgwpl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ldaiobui.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kutwyauk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jgqjecsc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfdsyga.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zwjwnbus.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkhogqko.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fukcisgq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pkggjisc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2blcgwraw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sasxokhy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yfhougay.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qsymhtpv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kbpebhhe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qxbfqhth.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xijduxcy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mudmlmpy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rgegtovu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2khquiyci.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dmascfqc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wkejtial.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tcnazfdy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltsiarxj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2enktlapg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aqihqmsg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hbyzfxmn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2shsdilrq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ishhpnlc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nhixfqjf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jinrlqet.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gveyvfoh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xlmscguo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wylzudny.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2znqhotai.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kzqlwgmi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2aespeasf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2puipffnz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kmqfkrwm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bddsfzop.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ewdscehq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qrrntdia.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pmvaeymn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gnchxkiw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fmdqbjhh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ckfmrsqa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ltarxaiv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fgynwomj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pppidwjs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2twxphibd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2skacickg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2muvhkblr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nakuaycu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2myybrcel.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dixnyaqo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ylonwzvg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kmnuvtvw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uqqefusr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wfukulpu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2szibiiqx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zlhnhtho.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jfeshwrz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2atnhrewg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2iettxhko.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2iyldrozk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kfunafvi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hnmxddcp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2siljmipa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vwufbhxt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2icgoazzk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2bxoxyssm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gdcegnzg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2varobqtq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cyxcqmja.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hbbonyhk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sktrqvlu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2amudgrfu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dccisypv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ffentmqh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kyjdsoxo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jbtkgeqw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2oxlfeeci.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vdegkclw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bsmlnlvc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2omzqwxqd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zthytafa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2etllifef.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rvkbdhsf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2psbuiysb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2khangyyb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ggzlagvz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mzbwzyok.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qgxvfols.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nuwcadlj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pkvqyjar.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ovsooleo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cpsakvfq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2txcyvbmq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uvrtgchg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bgivqcvm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mbrndjpl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kfgchdwx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2slnvzcpb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gpqlhqdn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pqtjruvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uhqtkcti.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2omlyqjpz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xileivvk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mforbikh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fkmdjmop.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ufcqzhbk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dqheiyku.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2kqrdjtfl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mofpadgb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2idnyaafn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2eoivabfw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qoweusrw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2thzhhnqu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2rabisttr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xaqqdpob.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qvjlwsce.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2akdxcnlf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mkcgpcpa.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jlinsfwg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ihxzhsrz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oftpcgyd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bvwzjjze.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sdkmofjl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ktequjav.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2sqcgqguj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gwescmcw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ubmylrot.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rjyjewhx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zkeszijp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddsslojz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qrclvier.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtwerssh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gasmweqp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nelogcnd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2djcoqocx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pykgmqex.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oiyhmfzi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cwyqgcah.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ifpvsvgy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yhsabbkh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qbjgsrjr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2henbcyui.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2nsvkwqvc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2abkcfdxu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hpvgfdkf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qarlcney.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fufsnxju.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lonfobtv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lmnimlei.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kihgiwes.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nvndnvrc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xlwsbsoz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yvgdawif.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2toavwwlj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wtngsqef.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nyblobly.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zoqrstgb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2siyyjnqx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xumuqyrz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mtdlzkvv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ooqlanjv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2olrqsmgn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xfdpvjwz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2brmkzwkh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dlxynhmj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mrvnqdcu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cwnikttv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ooocexyq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rsojtmgt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qjsinhtz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lrjziusq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yywchpqa.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xxwbovji.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2binaluqp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qnytekiz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mnaxapsb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gxvawnsr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wjcwxbvs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tgsmfqfq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2msdjhdjx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kstixoiz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cjzitxtg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hxpwsnqt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rtbvouvv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2alsjqxcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awxlpcht.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nwyexrgo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lgjndgnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aapijagb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mdxzxves.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dfncnlup.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2uwyjofue.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ujrdaxrt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2kslckksq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2uxtomykc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2cfbmglvt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ywkynzvz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qfgixiwp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ktphtkvg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zsglzbqe.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2eomyowke.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wjdktuwz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2svhmquve.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2temtdene.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cbynufsp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2sznoozpx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2alsrbosh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vvxdvyhi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2gyqkvdvb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nntgkexp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2nfvjtzzs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wamrwnfe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qttwnuxf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afmevwtv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qpzcrjgd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzqnthhs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uovssnpu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xlsgdrgx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tyigzogv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2shebtxmu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mveqkdtn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iohmdart.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtlrsbes.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ispbmzsl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wttphrig.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xepgbkcf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2asdamgpc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntqejwlo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tmbrrsjz.html


<!-- 参考信息 -->