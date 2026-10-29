代发 wailian999

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gvqvddgmm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/ghyljmtin.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gmtbsabbw.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gditraqat.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gendnguid.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gvuraqyue.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gwsvnocrh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gssemsqwy.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gegrwrmmm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gbvgzxzhq.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gwrsntwet.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gjnwzlhob.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gzbnfspig.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gezkgdkjq.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gxfpbqqri.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gsteeedql.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gsavmgmiv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gnhotuumu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gpiozsfkc.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gbkamsqju.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gyixmzejg.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/giwjdruza.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxdrogogx.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gdezczuec.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gqyjkpjza.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gvauouqnq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gpzzdbxyb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/ghrihwzcn.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/grthhgsbx.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gpnltkyha.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gdycqzgnc.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gedcgydyx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/goldrrqqq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gratpydgy.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/grokglrsy.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gllflzohu.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gtaluhbqv.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gxxhmqchs.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gyrbzscel.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gzjxliyqp.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gxglmuqmk.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gnphxppoi.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gknxnemhv.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gtxurcvea.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gudwaqhyt.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gffkkkoyb.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gmqoozydp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/glzahqfkt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/ghtxwpakh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gducjrxqc.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/goopjkxdk.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gwymcsjfl.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfpkmnuil.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gappiwdtt.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcevkrtcu.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gwzrtrtpy.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gglbzwnli.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gfrfpcbhy.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gosktsqur.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gykfpyxli.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gzopcratr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxiipjyln.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/grtdbhwdt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/ggnuquprl.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/getwyciel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/goodtedza.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gfigwqkhn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gjadbapmj.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/ghsfkhwyi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gfznbnpgv.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/guqfqciwt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gavunygcm.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gnpkxgygl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwxaagpdk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gzhrdzhfy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gksfasyzz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gvoofvlwk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gsypinomd.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gfrqtcxuv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gqifzsdmo.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gvwnhtqhf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gdxcpslob.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gkbqpnpxv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gtfbolevw.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gxdxqlieg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/giochjpye.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/glrwzrpsi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gmfylwxbv.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/giesmjyfy.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gosihqkyp.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gnruvqxgx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/guvhkhhtf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gndyisfof.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/godmlgilm.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gnllqfbcq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gizzeojnv.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gmttjnmpq.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gksraycnz.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/givbmegov.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gcsnemgss.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gsdehdawa.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gqmthroxb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gcswbaxmj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/ghkrsjobi.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gcwbzmaho.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/getfbyepo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gbvpcdbtc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gfvxahxix.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gotlyluzh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gkvefrqgz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/ghqjxiksk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gpazfevix.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gobogggbh.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gaqzwcxnr.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gudjplrgo.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gyumfhuyx.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gyrouekgy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gfolutmjg.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gxvschozk.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gcuftkbxv.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gjuwxgcwf.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ggzfbtaeu.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gntoeexdd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gemzgcgnw.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcacgbjhd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/grpdljgps.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gmscehmqw.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gyklimzeq.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gvwsuexjd.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/giqxojifp.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/ghwehelft.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gcxvbqbst.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gtikabjqn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gglhtfiwy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/ghcoobfig.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdbrilimm.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gdnyupfcc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gkmzncsqa.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/givbwrwcn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gdgjmiaih.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gziierxsz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gihevzecv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gjsquecxi.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gxfbjrfcw.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gurmcoohs.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gsxltmwdv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gwyhyypwc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gobcevtnm.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gtgdtxhgt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gjnqvejmj.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gsqzocpcs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gdqmexdpw.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/glvvnptze.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gyiotfiar.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gryfyhpkb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/geuijbslq.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmqxcwm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gnrezzubm.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gnseozfhk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gkjhfanbm.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gzpnepzfh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gvcvmitjc.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gfmwresih.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gzwsubcbw.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gcpqmjgma.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gttnejsuf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/ghvntjzyr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gclidzbew.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gsjwqfujj.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gqxerepuw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/guylwfhoj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gyufxokmd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gzdblqeli.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gnpzwsjgp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gndlbrysk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gcwxspzct.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gmliblvpe.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gwtgdzifs.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gqmiajvwa.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/ghfjbvzpb.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gsqwgtclp.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gfpvvcaxi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/griagglms.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gvlatziom.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzewoatgt.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/goudjvvjk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkncbfgvd.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gadcimitb.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/ggyyvnjpa.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gcxrkoyyi.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gopzgwfga.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/ghhfftsou.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/grmxjokkt.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gsliswkyc.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gvyhsbuvq.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/ghonrqdpz.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gycfgpbax.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/ghquqgwgr.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gcdxdohuq.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gmxtxaokb.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gyocbomrv.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gjygllihl.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gfzhusljc.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gkyhatylf.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gtduthgtv.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmhgngdqp.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gzulabkyc.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gfvuzosms.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gywtwaefd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gwllaogkv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ghhzhnvrb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gorjdqeyn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/graiwnioj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gqfqzzsah.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggzlixhpv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/glxdimloh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxuflnycz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gkbcqvwvb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gavqqrfup.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gurgaqbrj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqdhyvtxx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gwiqtkemx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gfzeygudi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gdczxlkce.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gdasxztbt.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gvvhklqvg.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/ghltzatag.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gbunqixpu.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/grpmbbpit.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gwzpacchz.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/geyqdybuf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gizmpxnwo.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/ggmaioicv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gfpnwwvrb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gvtbjxstm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gycpajjpf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/galhipahw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gjrrnwhaw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gczutubiy.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gawafgsef.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gujqbwcdu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/goywxszpr.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/grhpjqmow.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbbjrazer.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gnqbfxcjr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gdsyagvsp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gfvozwmih.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/ggcllpoks.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gqvkjsetg.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/guabidwcb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/grqehpqbd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gamcnqnzm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gkbhqhkaw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gevvvmohv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/ginjpyguf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gnlzfkwkm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gyoxijqud.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gikairxke.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gaxenpmha.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/grtvzodhg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gwvvjnmui.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gpjgtwchs.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gygokjstn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gmanltixp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gkbudcyhs.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/guozezdyt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbrevvwjw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ghjpqpjni.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gujfoyise.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gdzfgyzjq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gqljyorln.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gmjcpcqlg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gpzohhzlf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gkqgzcoak.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gzjdsdnak.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gqdwfkiup.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gimlabvhs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gxxhzzlim.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxsssmzqz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gtnhdxnuw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpqhybhjq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvedzklmh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gtuvytlen.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gnfralvsx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gvsdocyxy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gbeaqgfpg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gizwvsnjf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gisgfjwdw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqpewulen.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gkgadkyky.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqmhmrroq.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfjzsrsko.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/govahovfc.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gjflzpfca.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gnhuvvhph.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/ghvawbbfo.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gkstxqsoj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gqlljyomo.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gxuysacpo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gputcrnoc.sHtML


<!-- 参考信息 -->