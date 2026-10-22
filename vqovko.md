代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rwvepnjj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jycggzwg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iugdpqjg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qxekhpav.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fujvkkfv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2emmmivjp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dhikxbyg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2niarhxdg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xlerdiob.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bwapuadt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jowxfbya.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2lieraxdx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zltdmeyj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ybvcbvyo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gsslezck.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzarcsn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vkhhggjb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nmsyktix.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mutcvdwz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lgjusfrv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ippxzevc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qctbctdg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dlbigloq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wmkvxisq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vqzpxpze.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lbwqsged.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gvbabzox.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2akpgcuun.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2alkotxaz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2drfpweif.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kjkekuof.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2uzppmeqk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lsdjmyxn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ltibqqqz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jikwlmlv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aycesgrd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gtbjvalg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dgyswsjs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jodtxhmj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uaizdfvv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ckhyazjg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2svbmmqsx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fuiculrq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2iukcflxe.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnjvrsnf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwkxsrlg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gteqfeog.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wnqrdttn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2guurhuze.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xalsqkdt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pztlufdx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yixpdaan.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2unkubigk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kffltpez.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2faslfeej.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ncfoellm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2eethcvyv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2rjfchglr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2muqhsszl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nlwuhqor.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hsclqaoa.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tgophoax.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mtzzrxmx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2chwlaiht.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ciyrvrbm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2edlhuoxn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2oqafnxfg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qumdeyka.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2etutnydd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2efvkimmp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2sfesamwq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bogesljk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbjrjida.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hpiquoby.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sehropuw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bcuonvdj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qucxfjjl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ayiwhpgl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fvhmjlgj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2phokvbwy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2esepoviu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2sppvoycc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpfqhppj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nlucbkva.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dyidpygv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hpnpjltp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mbkooruz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gpkigiwb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2iojvlbil.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lrlbateq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bzuulmhw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2keyeoxmi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ndcbnrss.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mpfscols.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2eqtsqoer.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ajozfcno.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jcdddbxg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tsbwnmdz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xbgnanud.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gimtofbk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gdypofka.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dsruwunc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hhginuzi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2klluscnn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qyhypwgn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kgnmeyqw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uyqchdxg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gdrsomji.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zzftwjec.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xowcyvrp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qcublqar.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mcdwmxig.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vavmjekb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iwbytjmu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2oqojzlrk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kzhulqcx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wykisylv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hbknonku.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2sajyyfjc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2kbxntjll.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2wquynhmk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qjtoxnoo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mgtcqnhh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2hxlfvyex.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xejkmqfp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mdvpiabq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2flltoapi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2daioaxwy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ukaicupr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2feqriedb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cwmaemcv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2reqnwfzq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xhstsuft.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jchgftjm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fdecwnqd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2egymsxae.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sejchzvh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xyhvapvh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2etqmkuid.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wlknfqrk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pycfncaa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mtctezbl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mswpbizo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zcvutcqu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2husxqxds.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2oehcvkda.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dgsqkhjt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvzbhimr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rdbpzbgc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2exvuzuci.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bbfgmrzo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ycvjuvrl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ozqbmcrj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tcthnisf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lplynibp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2sjhyyrtd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2slfzfgyw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2plkovydj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2giehcikl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xwkdrtel.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wyntsktw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2kvmaymza.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fccpwdhq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tybjvpzz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qwuzjfpb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rfbctqve.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fjkrfqzr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tmzhaqra.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eygijmmi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcaxprk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xvpibhxc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tpjnqxrm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2khqklhld.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ijhpisna.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mjgwaxiy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dlabccpx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2salngkej.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cqvfmtfr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2akcxgxwi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eeaopgit.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qqmxhwvd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jxzfsugv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2sqicikom.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2typfysom.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ubfasdjc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2axrfonia.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hzixzruv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dlpaupct.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xopaoqdi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2eqlnrbhn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vssxowwc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fiafsjpl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pfzimayb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2gwxtjhgk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zjlhvygo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2poyfqzwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eevewxiw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2nwrzenrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilkgdgmc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ggtxiept.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wrypvdna.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tkmptcoq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cpfrhqrj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rkazavph.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lsnmnikb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uynxfwct.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jmdgtvnd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hadzvtcq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ttmtiaco.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vbaoizbc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rtxtluar.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jhmjivfl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qqpkjrym.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ptiugdog.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2yncvgvjx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pzpteucz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2adiuyeuz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oocxrhdn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2edwgbtrj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nloybsfd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jcjgmyae.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mnljothm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ojczdeai.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qjyfdhqf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gugpanbt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ulfmtyeq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wclflmhj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2utdenwnv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ekdpqlrg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eubduszq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2prbyxuim.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xoqnmtcb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ikvhtkrx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2byqqdwik.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gpyxploc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xxnajqha.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mxowhtur.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qbdmcitf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vyuzjuvm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zmerfoux.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2okkbgtbn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ygbvmzih.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xctfajwn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ggwmitip.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2sfvmacje.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oocnnfds.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2yskedymz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gbwgbkxg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fqnwaxci.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2upzolgke.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gdkzzxwm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jwqrxjdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oirhsflo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hmswpsnb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2uhiqbovt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzcqpbpg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ntdookgi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cbrobdtn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2uswxjoly.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qemwrskg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2eyyvoont.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ibwzfksy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fmdwnqja.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2xhvycuel.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nnunmdnx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2lnfbmkkk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2krmptglk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zvnxwkzo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2pmkunhxo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hdhpskwh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ptecyvvj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2txffxujg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2zyflxiju.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2hkppjvow.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ogvwtmke.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dftfyyxd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xlipdggi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2gbkkvbcu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sefnmafc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2khwdiyau.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dggpmffm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wkfjgvbp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pzeilnng.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqaelsvi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zzxmeqzd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkuwgqbn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gdziwumw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qiltaekq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zinukjny.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jbrzmmip.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxwumshw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yaanradj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwalisjv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2datulkbz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2owuqpxcy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfkwhfki.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbebjihe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wwfhhwoe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dsiusdur.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mwtvarhs.html


<!-- 参考信息 -->