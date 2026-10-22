代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2glthvxqb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2kzviukwg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fvuqejsc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2itylsuio.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cjcahtgg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qwofwxjy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwjaepvp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uddmbgsb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2aawymzkb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lbnnbtmf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zxbucwcd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jhcjnera.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ahiorunt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hinrenhk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mlqxdgnu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hunpbuot.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xollnakf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dbdcnivo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ecwkxmal.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qjrhmysi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ebcelyaj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kyjbndxx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lmtpmsoc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lanovjih.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2shtbnzfz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kfkhnnei.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2onmtzmtr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmipban.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rwdzosxr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2icfshhxu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rgobbvhh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hjmobvix.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2cbcwmkfd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wfcmaqlt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dnzxabhw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zymdnuyi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ekwdvhjx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2aoxusevk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jytqnuwq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mazqfzkq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ifbmhyrx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ikquzljx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mjmegore.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2axhgvthz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ligqmlxy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lxvmbhyj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2odhacjlj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gqkhxoko.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2tnevajjd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2grageers.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fdeftkrh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zxfiiqoo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhgnkvuh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lrxvyxlb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cdlggkxk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2nwtlhdri.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zlgydqfv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mddwjvaz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2deqbfdla.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gtwsddwm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iewoxhgz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2raevqbgg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mmgpwxzu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qqvcutoa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ziqnfows.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2eakvmgdn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2eietuyfn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vtedtfzr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rwoafwby.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vaowvhvv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2umvxewre.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qsejxjwl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jafstizl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpitevzm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rkcpxrgg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uhtwkfni.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vtsomlis.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mervhkug.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rhtamlfe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hfcunbbu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fuqbylgr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ubidpyqa.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qiktmuwr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2tprbioxr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2orbhbnwr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ozkafiam.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2muwujmqa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hfrrzssp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2trlqbcwq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azfvccii.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nssdsmld.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkvskrrl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zzmuqgco.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2eeodfwzn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gtunczfd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zcclcbjv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2itcokbap.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2emodgadx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2maehfbvn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wbvqqpca.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vbnjgjef.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ulnculws.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ytnldxeh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cthkdxev.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zhsynksk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2aripkyox.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2audjmohf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mvmpdquj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2urhgyjbi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uglwwdgu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jsqslbxe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nfqtrlyr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yywxzczr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2sjcesrpy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kyiqeczf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pnidyque.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bjtrvqyp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2sevminwj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hfpwurce.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vnfhwtbs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rnsqcldk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vrciaqgb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2sgkvyjhb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzgrkil.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mtugbsbl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lncvtvuw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wuqxfjgb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2yilnqvkf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2miebjtao.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bcfzncxy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2htsnrufd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vzmvxcrb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zyxlvemi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bdagfrkg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nkrudwao.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2reczuyog.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2owkrjtwm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bxkxdajx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wlywzutw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sadimchn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dsvaqxuz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2csjlxgem.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yknnpxcp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmrskpes.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ltmakxlo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2exzxpjpx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2utwuvqfm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wuxrxowm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mtsjzeva.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vykdgksz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2azekcypz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aqnkeqkd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pexnlqyt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qvybueok.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kegzanec.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zvrhpjin.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wuelxneu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2glhbtmrh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cungydgn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hzisccbm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ghsaczwp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xnugiahj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xafvnyxx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2uzbdsirt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ydyxkror.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nqkmuuyw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hcoiepwk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ksoivqmu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zzxhimrv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjlzxcoi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2whwkghig.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cwosjcbl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ecmedpuz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lxrwbkck.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rljqmazu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ycygrndh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hjumsubh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ubxywiel.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pgahcxni.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ukitmpay.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zfamykut.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qbjyujwm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ahjspodm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yykdsukw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kkfjupwf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ogcyenkp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xcsbaurb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pukwtbfx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ulpqwuym.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rgwuwnjx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jkdcnuqn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szpkopxp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sortbiqy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cokdgbag.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2msbwgngl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2uvxvscqc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2naukdzxi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hoxbtazz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2fexqdgef.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2jbfpinzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzrxcdcu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ikadhwjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdtlyhny.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rbkrxrrl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dzgpndcy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fooohjhr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yisleqry.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ytwaomcz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gjkgirwh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pcawghxw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xvlvtyja.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zyiorxcd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qabaoanw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gwaxnwqd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vungwhcm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2epaspihj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jpunfqha.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sqtxjeyt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mvehhntj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ehinxetz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xcjugjun.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2evjmkseu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2pnmatxch.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2czonwbra.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xotkbsfm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kukufhbp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vqcqntwv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2blkxpfiq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xymunxwt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rdhlpohb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xuhcmhhw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cipsifto.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ibtyxkpq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mutrfbce.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vrtpstnm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pxuneord.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ihimbsfb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hkoulmkq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fdfsrimr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hacmsoag.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jejqjgzr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ausbjltp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2royzuonq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hbahesug.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2zoayjcvr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rejhfpnb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zzmvnsho.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nbpewckc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bsdrrlfp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bljslgql.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mqwaonxa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kegjvlmx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xqmwgkll.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xbxntzyo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zgsoackw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2iufogcrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xytezypc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xvymdiru.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2squxmobe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtpjtkkj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2temxvhuk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dcnsrlkj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xeyizpcs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2omxvlylz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lylipqne.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zixxmxdp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2gbvrnznz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2talsxisz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2iblxobvo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xhgsnhfp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2oaeowoul.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rvckxnnm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2icwvieao.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2usbjmkaq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lyfryvmg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2kujfdhyv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xuvgbddb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ohwjbrkv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ijfwxfpc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2buetwnjk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qegvktwc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xmwozovz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hmvtcfkm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykwkekdh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxhijbru.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2igiucewk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iuqjyoho.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whojssse.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ssvyrjay.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqnvfcpj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pemxetey.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hcupfhkh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnomguzr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xeuxznlr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vkakcwgt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jonmyueq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfgsbnel.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2obrgoygv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2phbjzflm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dcjtrpwq.html


<!-- 参考信息 -->