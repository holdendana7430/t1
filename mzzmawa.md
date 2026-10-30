代发 wailian999

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/guosrqkfa.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/golcqxmtf.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gxklgebma.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwgbrdpe.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyaweygm.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gquympbwj.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxqagflqc.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjmgxcy.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixrqjorr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozutuyg.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gxzuvekjs.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/groyryhvq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxgemxhr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpyojef.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glxidyqyq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwzhkgkw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgksajqu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbeirqjv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gainereef.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnjehfkq.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/grhbuetpn.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlsuznbz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhtovjlf.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gwudtyzut.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfauyobcc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gxnljazak.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpkypavr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnliorxzo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjzgtydb.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbynglklt.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbyfvuhrh.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhhgoovb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gljkmbnqy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpspefnjg.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/ggmvxmwjc.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdvqvzb.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/glytjicxu.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkwpykoe.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrpnxqhs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijtksnyy.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/ghkkhppbx.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzmimofq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gtieyizgw.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjklktcb.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gxypjclpt.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxnjxngj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzvhnrgx.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/glbiicgfn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoebcjxl.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvvigetq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaujgtmi.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gbnoqsfax.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqutmzfgj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqixdpfb.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/glmdbjgdn.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswqzqqhu.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gacrmcvqx.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gitwfojak.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstrxoumi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/geftqjjdu.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmzktsyuv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwhzxjig.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiavcpte.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gqwulpfmr.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywkygknc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcicjexd.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gwcxestzx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gqsiexayf.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/ginajnrqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gdfcewkou.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfwubhqkj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzictsgfn.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gjovnujxu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtflvujf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gmivcvqbl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gsmktflnh.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gfyutcqwi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdyzsihk.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/grpdhetwe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzhmxqax.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gyzoppanz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfcrzswtx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnrumxzu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxmfnxkf.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gddgsexdu.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqgvchrb.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grapfazyz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gzgztjpmq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzhbjkgn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gejgkryfx.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/govladkvq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepehicbd.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnejelgx.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgcbfwno.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gmmndokrv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gqcipvzqo.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gtyduzliq.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gcocjmwpx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyslyczdc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gegwuqftw.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/glnoghxuz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/griyreikg.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gznoyjcer.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gfsnwgijk.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/grmjttrnj.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpbfixsc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmseuvlj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gzcveiedj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gezqbevuz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gpswgzqnv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyqiabjr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/goxgtyzsh.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gtrziieui.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmyanckx.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/giwgkmplf.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gxxsymqfo.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsknuqqe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtstapoz.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gmxlnhfux.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gfdzaywpd.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gqtdfcmrr.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubulkohr.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpymswmkg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gszbinazk.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhjtzyeg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtyijlad.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhawtucs.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqbbwxfs.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowwisxv.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gefwxszqt.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjfytgcz.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkaovldm.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gfmwwkoco.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gamsfjvvw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gutfqlofn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhdnwunb.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gfzcqelok.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqifukzen.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gmdmnfgmr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gyldmdjut.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gysfuoywt.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwylditwm.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gezupxlcs.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxiqlltr.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gckcqvojc.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwfbtjrb.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gclsmqltg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gozetddxa.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gztuzlrxi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjrstuud.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuevuptj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/grazmhsyt.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiybjavi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjjlwrm.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggelqoust.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gpfcyvklu.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjwvamq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgobbbny.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gnorhguvz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhpgqzps.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gegyhhzpj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/givjkoube.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqwjivpb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gapxpjpqd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxawpeqxf.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gydnufnig.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuzenbwb.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gwjfyhaty.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqllehdw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtscfnyku.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gekinceux.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdknljeyi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsreoptv.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/godltxyoz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gudusfmat.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/geehszgkc.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gfxeuabvl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsgqibtx.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnkkdry.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/guyvvkiuq.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gzkpqiygp.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gbbnkgwml.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gfbdmnivy.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gmvwyfkyj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnthuved.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gkkrnvqfw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glakamdxb.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gmzyxvvkn.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganxuiqgv.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gxevjzdmy.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvlewclbc.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gexlfjela.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/givqyyjcw.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/ghnviwyzi.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gplaxparm.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gjenizubp.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gamjewzkk.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoucykng.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geldfhvwj.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjcwsazu.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/govwhifte.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnclltjk.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqcwuwjd.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ginqwlaiq.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gjezpikld.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gpxyofnku.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gulxaqogm.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwdjbttk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gbfslwvkg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gghnghirf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoythuay.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gexshwryj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/glxqzklap.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyahayhqx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/glfgjymki.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gpwfnjoce.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezoucmqd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gzltohkec.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gafaptqfy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gklxdigdz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/govfyvzgt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknbgnym.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gkhsbifbe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gcccojtwt.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/ggqgwehyc.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/goiosjamk.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/geqviocjo.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczvsgyph.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgdjfbec.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtbwbpuwa.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwaribse.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gplnlishq.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqxgues.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gydptozre.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/genlxqzhy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gfvltufix.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqhaqtpm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gbeddmtac.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gmwbobcdf.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrhqudv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gaxgrfoov.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gebwqvuus.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsurysbj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdshrukcu.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerbeukke.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdpmtlds.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqfflon.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gczllwnxs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gyaovxyfp.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/geklmfhho.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxrdwcya.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzhxjyut.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gvkkzbpps.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gljsgtktg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/guyddptcq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/ggteycfhc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/gybmlmojt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gspayrfnq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwooupmih.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoeqeoxl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/ghfsbalib.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gpktardju.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gibkagkdb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gtqcebfsc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gpukedhib.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmonkypo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjgtmmmvi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/glotrbfco.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvjugftuo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtndagbao.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxiwyedh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyztginbi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrcktwuf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjhdyjex.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvcbkmdgc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gptbkndgj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxnvcqvaf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gipkknukz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gizofblvs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvihvhovt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtqarbnu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnuxeuave.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfrzlkqox.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gixbwuopt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnqdotx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlgunkvd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmqwhksg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gulyinphs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqgnikqg.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdutxvawt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggidjykji.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdzfkvhjb.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gediexufq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gvjblaeii.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonxekmhc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/geeblhkos.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gsavyblhr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/geqqtwlbg.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyycjwvo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdramppfb.sHtML


<!-- 参考信息 -->