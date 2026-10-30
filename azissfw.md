代发 wailian999

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwbdfdkq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gifligcva.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqwchtsq.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdejfiakl.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gripxigfd.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gjdhfbybt.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grxherxqc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwgwqnpd.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gbewjfcof.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gycqetwek.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gspkgxwiq.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixyvpzvh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdvoasnz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtslovsi.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhlbzpse.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gyebhspsd.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfbuekkh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlcixvze.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gijhxzosd.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gawmbczsg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/guohchowq.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeeouuzs.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/giebbbjaj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtchfbfz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwpuvauj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gmtnqgnam.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/ggunskrpf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gtscookjv.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ggskjtbtx.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvlnbuwi.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwekrzsuz.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpqgcqzg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdcuaoyy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaewtmhi.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdazamidi.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gswifneiw.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gioizcoyb.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbcriprc.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgshlrou.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxprhbvmj.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpyoiadu.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gpljawmbu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/goztswcnm.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghcjrnfhb.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gulmuiqsl.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzlfmftj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grxaaglus.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gslptldee.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gtoiuqdus.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjhoazmn.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gohasnvhi.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gksdjgnnu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknlpbpzw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gudvvfowd.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gswimnfzl.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtyoayjw.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshosaehf.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtuhagcq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/grcikzyst.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwbhqtoc.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gryzrdold.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmllinfww.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/geyhmbqjf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gnthgmvih.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gglujkjzz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdxuuyqg.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxbxafoi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfelxqsyg.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuqtebxp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyssezri.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gcewkdmmw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/grtxvzlvo.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gpaumurfj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbltcisd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/glkbeidfn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gorulrfmn.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyyyokas.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/goqccizrz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gnynyxcaz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gceiohair.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbbxewhhi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gkzgzdxfg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxmssfhsm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gwlzsnwvl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/glrxwaize.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdszjthsv.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnqfavwo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gwpvrprdi.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/getiablwk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gsnjlioym.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxjvntd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhwglhlw.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/ghpuugcoe.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gqaiinpyy.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gljykyxti.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/ghvbvtehr.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gasqykmau.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gwnrgczpq.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gclsqacww.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbzkqgle.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gcsdqlflr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gzxwmuygz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/guaktriep.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/glnhvkbpb.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gjsqkrtup.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeesepwf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckckplzi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gcctvjcqd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmuhhen.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/glwagfbqa.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/geojwkdyo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gvfsfsfwp.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gtefrqefj.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gdsgeumge.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwiyuxxi.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruehihgl.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxiaceso.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxumnkvi.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmwgbwb.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/glnqiettu.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gdzmzlcsl.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrxbqgoz.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxmetknx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmzysjrh.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrxrsqg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gamaecvvn.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnkqvpuzo.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gudcihtkj.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsfwvgxpn.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gayqudgsg.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdjsufmik.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gsqtzgunn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gescjjmsj.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gazhttazj.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfqlitio.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjcadbqrd.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gyaumnlxe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gstaayokn.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gcnscjehl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/geejminid.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gigchwuxm.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/ggcyzhxrw.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcnvbgrjt.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gdmmnjwyx.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtysyrdd.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwniutgyu.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gppruhzmz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrjkivpt.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqvybkat.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/grjdnapaq.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gyngdmohn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghsnbtazn.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gprmryazj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwgicokqu.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvhxsxdw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gaskzxytc.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpipyeqo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/grdrhxvwg.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmaqcpw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gpncnksuc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaaddtbo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjojdxpa.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpyeaxkd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gyzvsicsp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geksintis.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/garaooyws.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/grwmsbfdi.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gccnypdzh.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwfjpujk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzkncros.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbezlmbmn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gphaxnypz.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gwwaahbpp.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/glbzsfdgv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gelziycvh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gozqrjbee.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gofrxthri.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gqkonwdcd.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzlxyugs.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gfroxsfel.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/grcxxehms.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkstvvqs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymukjehc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/giyimlmdk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goheotybx.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gkwuozvkl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geqzeyyhm.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gmgulcuwn.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtthrasnk.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxywsuwe.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzmvzzi.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gkhxcyctx.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gouvsdnip.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gnaewhhxd.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuzyjjmv.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpaktvwy.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gbpubwzuu.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjuglpcv.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/grarbfxkh.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgvibdcd.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gderzeofv.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjbrkpnh.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/grjgnhbpw.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmymspcvg.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gnyrnclfu.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulnegbup.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhyziae.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/geockzdtp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gaosuddwi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgvjcnmw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/geyfmnkkx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/goqgzlflv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcgjfein.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gmpcjvwvw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gldwrghrd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gnyvupige.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gitorzgcd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gxclnvnzx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gwfhedcxf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gnuztrymx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghszvphsf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gfphogyxw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbnitptn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxoscpgt.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gpenygtfb.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gxtcnocca.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqcpvop.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgzxxwhp.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gyntngvyz.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxraisztr.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gamzytuqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdqanegd.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gxbcltlmd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gpotdzoua.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbisxfcuy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gdtgpsnig.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/geevkeoqg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goniproqu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gdkjhnlha.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gmoumodzz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlohphj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gmsnatfmg.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkjlbjog.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grqnbvrni.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gxncipbog.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyaltouu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnhzpvjm.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gcptyxuny.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghebkcfo.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbodxape.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbupckzlw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrmmsflt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gwqkzvnzc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxeannjs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbhlzrs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnohmomwz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjjkqsbt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckrplfac.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/ggnvxdoxt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfocbtkfw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewetfruj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnrjqydt.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gxekurumu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/godqhfdkk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemimafmm.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsaczbtg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnnvxjsn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztloqsrw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpkbinet.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gocgqfylb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gtrysvpue.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzbnyzyhr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gziylqekr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiqtyeyh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrvkiscr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmlfelen.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdhvqfebr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiaeaiiv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaxlalpu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnqmtaqlm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxudkyax.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzttqgox.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkfoinma.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqxkjrxob.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grazsmsaf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gclralvup.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gceptyqyc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdumkdxzb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giojkmsny.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxbapzxhs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqkjuxfug.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggeveoqzh.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gnngkkvpl.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmirukzz.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/guofpgpig.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmycwqug.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gtrkuiyrj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gkmkmlahd.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gvwguzvag.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gbqkzrgzf.sHtML


<!-- 参考信息 -->