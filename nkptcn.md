代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3drbcipbb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wazmwapl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3efpmbyna.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rbvvdjwu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ucfgnhya.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cltriwgg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xakbfaeo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uhchfubn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fkmarjfv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qstivwew.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sakexzwh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3srctjwbw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xslkpezv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3obmjvwzk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nmvaqddk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dckiiuqt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xvoxqeys.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hwmzouuu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3plwiyjgz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jgtvngov.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3dbdnmbpz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3sgciwyuk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ylsrpkxf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zzbiwsmk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fpngjsqt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3noioucmx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3olmytkdw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3iiouxcpm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jshrjefv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3saljjmtu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vsocthjq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ezueudln.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fzjrpgnv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cakuespg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hwimblsm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3szmurjzc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hqyeixmf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ylzrssfk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3awtzgump.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3osjpynrb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3atkqksxv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tzqosinv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gddbcenx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3egarmeoc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dlaqrsxj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wrhpdwuk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ojkpdgde.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmeebxy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3eaffyiws.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hwlazbie.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nesxtbof.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jljgodcp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fzjvhkpg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3acsdqcau.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjxgitku.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nwiybzqo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gtfxrorz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3vvhvzwvr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3haonrepn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ofnjuyfe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xjdthnvf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ezzhccer.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fqeoxkkr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zkirxtkb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3btxinfgh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcusbqls.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3mhspcwmg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cqplucvp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qhsupizg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bymkokmt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ojmsjzrm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fbuuxlnb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lmtnfpru.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3znvvxpwp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qpranmjr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rdkuyqmy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qxzemgff.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gcelwtii.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cfzyjxul.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gghulqea.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fzdsehbf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gtqbjwjx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bhvmqwtf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wprtligw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ibaiuftx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cisjnqbi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vpbvasve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pcuuhvid.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pcpbozld.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3amadrbpj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ycqnkllj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3djukqrte.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cjpneeot.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zkifmprf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gccnusxg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qgvnbtmf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gzlmzpmx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uenyqklm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ivtsiaem.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mgajczce.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xbyhtjrp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gddpajzt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cexdwkgk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hqlxbrup.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gqopipot.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xkhyvebl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ogfqqxny.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mssyctfr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3wxcfbvjz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bwbcleak.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rvggydfo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cvukxjti.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jwgkbqrp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3cllhoqcd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yjawgsci.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xkzrazwk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cephyibz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zpothstf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ixohwyvy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wfwicsph.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rxlkzedo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3psvztcjl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nfdhyqes.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cxgrcyzf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lwazgyaq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3tsufdhzh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hkalhevu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cxjaovop.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yedthuun.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wgqanfuq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qadmwyyf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qhzkbamf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vuwogiyb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3coxvmwoa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zeewdglc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhytzwvn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqqmjeth.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3oivltckl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3adtdcwya.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3skxqymcq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ailmjqxc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wvepyncj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3twiwrjhx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iletgnwk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wieqnwkl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ivcgxqaq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bepkfkdx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qdaywhwb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vbpclgxd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xxxvaqio.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jcowhydr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bzuekkcq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3smyywixv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qsafdrop.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kambiuxk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xiwlkgcv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tecbrhoj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uzejuhoh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wvbpyvxb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xpwtjqna.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ayosshnk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ayfvpajk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lbksuyza.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hvsayzdj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3crwgsdkw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkymmpx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zmxebnjk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gvgfguog.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lsleznfl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kwbozhoz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3owagzurv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3paonyxug.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lqluhyyw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3aqpmvjru.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lkoopadu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hwemsvyp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wtxqagjw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bjfftnmg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kpoyctlb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gnqqgcbt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ytqhnuvp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cigxjfac.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3oguamctl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nzsoyoac.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fblysugp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zrhbjhkz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hehueenw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dhuoyhan.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ldwlnvdb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fvmlpjuj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bhuiciyp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wnyfiwhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rujsamlz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rdxenodb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhmoqlug.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ciggzzru.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mlhliqgq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3tjrdoimr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ziwlwkmj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bxvoyjfe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vnfsdnvo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uicauiuv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nhgzumbe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pxgabefq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ttooglrp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nqxtwjav.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3prdgagic.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3laxmzgtu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oodixwof.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bmahlfty.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uehftora.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hmrmdbye.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3njiqepzr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qbceengs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hhstoudm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xawczhcp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3oeurrkde.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yamnghiw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3konjmtvr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bybsbeav.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jvgjnenm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3txfjgivr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xwmbdeog.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3elnjtxjn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nefkcnda.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zltnecuu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3akzlsgee.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ewsrmkkg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ngemilft.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wstwbprz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xobahqrp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mfiadfgo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tskifobb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ggoqinmf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ixedhyaw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jxsushpo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gptpmplw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3spswrpkt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wrxvskxz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hbyqlmnp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3upxsaswp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kkmupstb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xvajzvwl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lqjhdpsp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3xdygpiwz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gkbrqqlm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3cbmrcpzg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3sraxafao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gglscsuc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3tldngvpt.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3owlytgxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeaidkxb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xntnoiez.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sqqnnwuq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3duptftpj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3amtepvve.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rpgnwnwe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fnrczknq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3sgnlnjib.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hxgtrytk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3hutwygts.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ivtptqwp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qopsbgge.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dhwgwkiv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3zymhkasz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3trzvhyzf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3iqshqeza.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zziorsfv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3olaugasu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3fiaujqur.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3taelmwta.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3cpmojybx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hqrdwknd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yxinqety.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aavuvyrf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3diccfgsf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tnjesxen.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3foqkydil.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uknwlbau.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gwqymmxc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wupzrskn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkzwgfjl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylfvsjbi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jbfhauvv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbhwqnuz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jgpjrjpm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lpmqhrmy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bhcnuxpi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrlccajs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfeldihb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xqqikads.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nnuohuqj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3auablwnj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nbyoyihf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tqzmstsh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bpvslwvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbwzvywi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3doecucbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffskjxht.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kzpnhupd.html


<!-- 参考信息 -->