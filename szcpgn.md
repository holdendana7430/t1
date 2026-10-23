代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqaguiju.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lpoamnwe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uitxykra.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3svplrddm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fsfwusxj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dhqbzheb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3bjbstvfv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3paenruqh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rgsgsyun.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3sjemnhik.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fhhelobk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dvazpvtd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3musulmzw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vpnecleb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3iptyrbdz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3spytwljn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ealhbnkj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3efpzceeg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xyblwzod.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hosebhrx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3idbirqvg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mohhncrt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mecnwpoq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gxlragtk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3niowkkuh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dweyzems.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uhhcgash.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3erpdoxli.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bwjrjlvh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3frzlqieo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pkvcjfcx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wvogmrnb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vgxbpbyd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3nkyxowox.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gfpvpahy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jnuffuhj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mkdrxsab.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jddhlpid.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3niutrsrt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3drbgsndk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lrddchgu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3csootitc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wkwemmom.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fygscglm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3akjrkgwt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xkwuuzzy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uropjonp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jqxfbmuu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxxmetoh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ppzrunjg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3clqzxjje.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqhouwco.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3orouhizp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gktaaonw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cpgfbxux.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltrlytyt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ntmcakwy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xemqicmr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3foieodwr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ucecuila.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ffvwjqqv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tilpkhxl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3biidonkq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3frzqtwmr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3bvftajhv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3klmjyqkp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fiqclhai.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hxqytbeq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lputbbcw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikcjfbbp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lcxrmyzf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbgssajb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dtjksdlq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3intsocmp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xfzutpqh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jwhtpbnx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zdngooub.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dimfaejc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3guzqbfkf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ngtsufmt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bdbdxkek.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hscwkkht.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qkhmzwvs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xwtjcqmx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hnnmnxyi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3looyumcs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3doeppghj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ohqzomst.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kzbkadme.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mcrwtneb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bwnsnvmq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ijdrofdt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3etzmltrb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fipkkgdw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ufvxwihh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3efgtykea.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hrqhgkyf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dzimausc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wfymzlun.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3veplyogz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cwjyrytn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3yzeqjvrg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fehqtiak.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ifiinuuf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mfsiwgbo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3efomxtyz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3npbrxsax.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zjarlhla.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bqytavur.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wvuqmsbe.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qawmklyk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yvtnymse.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cnafdcan.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ezkqqntr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wzvkzkwe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3oixzesxs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cgqhhnqc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3sbuqbryw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3knxlaeld.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ivbqzcxj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gsnptaen.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zrjymohb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3srlmftmz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3iamiqlky.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wzvcanse.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nedrmser.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3uktlkwde.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3luafrgkh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zhsnoslg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jaellfqr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xctqjvki.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zavavmik.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rrdwrhvm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kizbxxdh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3tllxsyda.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvcponk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xrnbnrmt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3yuxhmidt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gkxcomwd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwyuroeb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rphuitgw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pgcfnzrf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zuoniblp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jvvfqzsj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qyemsejr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rfctdihi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3frvllrwk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fphskwmc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ahodwpze.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vktncnjq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bqwkymru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3iplfwwje.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pmnbdgbz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uhemyqch.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mwvuwxfs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3obgdqjqr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3eulnulmu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxjjpk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3yllipiam.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nghcpkvc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dfyqtvov.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3webqyvva.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3iuyslsjz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3azrqvuqf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lojtukvh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3agfjlatj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xigmbwna.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tqaxvwuu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iqoumfzw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pddstaxl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ztcxxsws.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xnvyujxj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ndyyxxzx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ulvkdznh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jbqfatjs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wgsgjbvo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fowdlcdr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ejmugvsc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3atuydhsw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tyqjjlya.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3oprfgzlp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ykokkzpt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3znweyaka.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lladuisy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zjolczyb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uyyuryxa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3aioedxct.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzxfannc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zmdtbuhi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dkeqbqyn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nivnoayz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3brwxttfv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kixhjldd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kfggexiv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3spqhamlw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gsadibtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmspwoef.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pqoregyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urzzyofd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3byxurjve.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dwdcbxsl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mechienu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ejuwpdpe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3koicdowz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ptxygxwl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lwfcfdfx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3brupndxs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3eebmqazb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3iwyjzgws.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ymdvtqed.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kgrclfcv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kaznzgjl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ansjctwq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ztpoemyl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3yujrimak.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gczeyjtv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xahqjtog.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gifrhwfy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mrhjzwee.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3gnprwsgr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3edfgmbrn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gfxnihue.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3btgbplwi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sgavryqo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gkghjhni.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3embzavfi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zphswqda.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mejfvzgc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ttmrgimq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3itiivoam.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xxmxbkem.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3utnhvkmp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ldsrvqbt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3aebjlecb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3srpxrggm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wlsmfeoa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3iiwzxklt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3sirqzwbh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dwmcfyau.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3brxmvzdv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3bdswrdvt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qzibqghv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vbrgfueo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3adytnecd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vksymfnc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nmyjxhgv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3evuxtzow.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3cenmmgai.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pdjacaym.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3zkbftabt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mvodmypq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ifdxnlfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgnondro.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3qqufoqbw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3iyiclrkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xofzdlnv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ssxwguqi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3irikzrsy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vqjmrbro.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dhdmqlnm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vcrndkdi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mpsymrfu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3msyhzjmp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ehyxhcxg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fxkpcbrw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qtcjyppn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3krpgdhlg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3pmxmznnr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xziatqja.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3llbpzkbi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3eyvzisnu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jnhzlsog.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3wnnhgwbm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ooaarnza.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3oihcskgm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3efxbfrov.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fmnbnfin.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3egdwtzwb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lsblqtla.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rirbroxs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ibmnctdk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vthcbbcs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hkclbxaw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wfpwepid.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqrkdwgb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ajgjnkpb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3spaafjbn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mxnlfcxl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3apmiccnb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fkhugvyl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gqgblnjm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3snbasfdj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slylnocp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ojnisacx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jbwjbnyd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdtofbyd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvbqicka.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hsaigzbr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xlmnkxrk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqphxrjt.html


<!-- 参考信息 -->