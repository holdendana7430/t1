代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qpfhgdvj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2cwdvfhhc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2faousrcp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqcblit.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2awremqfn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jzzfozcf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2abezqpld.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2majylocl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rnaqciyo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2oycvcvnv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ycditczw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2chlgaybq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qrnemjig.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bfsjhbec.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fbqkwtnc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrmkiep.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zlkfriis.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kfiijfqi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2klkcnbdo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hkdtscru.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gaqjvvss.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yvcuzhoa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nwgpfofd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpsvegi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2glwxyqgr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pnwwcuto.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bzamkpbi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2svqgdebd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2arxxjmft.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mixohret.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yytfdptx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2opbzstfj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ilojbamb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zwfrkhqf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kjyaberq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vgnncmig.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2famzrgop.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rriqwtec.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yasvbjsp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jbwojold.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ivggdyzi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bezerowt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rrupoafk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gklrvxdv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lblfgmzu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jdlmkbsl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nydmacmj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkqasxfn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2klovbtvd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zdqblhpy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpmlxwvz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2texdovqp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zppqjzlo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2plmaafou.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2myabgpvd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dhkmtxsq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlwnbnvv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fsosvrxv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rhadxoag.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bynxwkfr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dpfwasgo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jucybzwz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gyekgdis.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afrcfdgi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xrbejuet.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lllyxzgi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2spfoggqk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2srkmcamt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2egsptifd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qkhhhyvc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vzilnfnr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jmrbnqbx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vhoytvpe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gmbjxsss.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xfpxkbql.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2reznliqu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bykfageq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xidmgrpu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qfzafknp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tgfuwlpt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yqvvvwdv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rnjqfdsz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ytrhptfp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jebqurly.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nxqrpyqm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wjwgfwbr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2laopjceg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2nwiyvoyh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fcxhpjmy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2javptiuh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2auapmrhm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gjsyxnpf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qmeblbcy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvvpmtmt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rhygwpyn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ofgeoiiy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fzksiyqv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jeizxxei.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cltlvtiv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wkxfvias.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zulnrnyn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2krkdfknw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vlzkuvmv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2odrgtsch.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lwqqvmqs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nnacjayi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fizxusyo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uufygzjv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bwnarjfw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2knzpuzdb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjbydrlf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2oggkjogg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lmuedfsh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tzdfgqyi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mwmtbtdr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hckxxmzf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2maswspob.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kkkfnadl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fujrsbgf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lgvzupoo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kzelhtip.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wlsekgnd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hlqtqlrk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2unhyagai.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xnbijrki.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tlnjovjc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2igkpvotr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2czjofapo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wmmhdwqj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ymikuyry.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mrmqvcde.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2sfhgmshi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ibapgcix.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hpgnqnsq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jyezlxbv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ybktwrrx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gjirazue.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2laxsojlx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2eonfpxgk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ikbhcwzb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kuxsvqsr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zvbtzcif.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vflqisbj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xadqdesq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yrivxzwo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2yynppzfz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uiuiavpe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qkmboztg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ubkqutyq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lcfwayhi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hxzqbyxm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kjdodtwe.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rphwpjuy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2axnmjtea.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ohkqcymm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yidhdyzm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2shimjhyz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qjumeskl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2abwzmudd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bonbreic.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pswsfifm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jaglhlpf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lpoqlvgi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yrntagww.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hohvnagp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fkqblzoq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kxbkvabx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2iscqaudu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ovstgpdy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xgxehreo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cqfukwau.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tmwfjjgq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2putuaaep.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lulepoka.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fkuwomqe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hbdpvisy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nmjxzwup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eqlfwnjk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gwpliuue.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xopritph.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rioxjnst.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xhtubpjb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2cdohrbzv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xyddmmwk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dbwjnaej.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2amztfitm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2obnomuow.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wasfocjp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2svrdywix.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hhcejhes.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2uuiwxikj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qhnaravt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vmmavupk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ncbcvvlv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cbupkdoy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcvazcmj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2foqwimsj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ojgqnomn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2useyyhpa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wmoftrlk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ykbljtxq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ueqljbmw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nyrmyokz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2exnssafo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rokmznll.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ptvjjcmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbwglmba.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fsqgrjag.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fxeqtocc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cdwrjyjs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jzqadync.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jnzkvxjl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nysfrxlo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kzqxbrmp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zjccfhmi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ihxwsjxv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tnkqudno.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tprbuxzz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2oyshszxb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2iyaozryk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2clfqupru.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bidzscao.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gsgoilcm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jjkqsluo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dpsqaknf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qpwudsfz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zxnxhyui.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nxqdusub.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fsmhbiwk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dwwlkigd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ytvftuau.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ymoeqntw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pecndqhe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kvyndobu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bywwnjte.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2smebzyte.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wvioqvrb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2avbdznmk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gzxxobqe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lgzdqboi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gghjrlen.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rqykkwns.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2nwyclxva.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2snyikwyb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nyriioia.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2smxgghwr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rlryxidc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yeopyake.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2itgwbgut.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fnentxdi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2trorxvvb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dftfzwzb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2otpczdvj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ckyleyze.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2vgyiutbf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ydjpmicf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrvqos.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mltdojcy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fzlzvlvu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2dnylteeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uatjsuwj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ccybkyxk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2veqzijsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peovukwt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2arkeyokn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2muknuwzk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kpcunstd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2nbgwxwzy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2xshfrcgi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qxnwirda.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2inbmxefo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2jacxaado.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2uphomnxa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gjyupugi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ocvhkomf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fjgweeng.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2erofpngg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2lyeeufds.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2dxsydfhu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wfeaprbp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rzdsjtxq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zpihmydk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qqcicqhl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2wageqetn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2efsvzxuo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ciqkrnle.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wfkriewl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qrmqwplk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gwcdwval.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2prrfaynl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jwyusucu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkcxhzha.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rktimltr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2penxggzl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ckmwhjtm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ztnomccx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yslahxcw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zvglcnwt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ssaiazzc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xjqodaoj.html


<!-- 参考信息 -->