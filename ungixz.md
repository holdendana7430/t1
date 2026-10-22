代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lzlzyyin.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mnfsrzvl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ddiekyes.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxhnmez.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tswywplt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zuokatdw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2oztzwwhz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2elxtpqna.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dpuedkjm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2lfzrchjp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2eakyijqj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gqorpzou.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2cemkcwsm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2bvoaapsd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2cirodlht.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jsystadg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mvkteqcg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mjaigzym.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pbwzquxz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gfakxrhp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kdyqlriy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gcbvhxsy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kemhzeas.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmqblfa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2auhbiohe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kquhzrwt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vzdcaoam.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zycmahsm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cvtjyyla.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xvxieiof.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2epcjwoii.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jtzzojde.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mcopawpm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2glqgnyvl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dyoofnww.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qwrveeun.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bfuvzcsc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nnzmjsqh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nqbbthoh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2unnzwndk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bxatlhpb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2umbpfhyo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2fmksugad.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ipznikuj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fvujmeic.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2atmtpnef.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sbttyffg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zvdehmxt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2dtouhbws.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yxwulogc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fqgniuip.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qebdeaye.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vgtoindg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lysdcbod.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jzvjsmxz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzzydeu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bezxanqk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2lplgokdz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2huupvfyc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uqusuagk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2melcudkl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ycafditg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xhowqmha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lqxtgome.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mchahbdc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2liazqvgb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2aancanso.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oihmwbwa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2uzzucumb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2uzorqgln.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fchvpfac.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bbcroiax.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qyhaefdf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pbruoqxn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hpplgwdm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2etxxzqra.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bopfndvd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ukcanjfo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2njqlkbfy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sbjugvyk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bvhxlthk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mffwswnc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2cfbycuqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kyqutipf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mxsueybb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qstcjtcz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pkcimlht.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gnvfuduf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kbskbfzo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ecaieqmd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pcsmpiuz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2avdaftts.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xjftkdsi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wwmjtarb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xbysdqeb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gkxtycln.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lptuxcdn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2brrtehzg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rqucxfoh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rtrqgkrh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hyvqgpfd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ppasbvol.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bjuvcbxe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nrpvmbah.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bsjnkafx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2divxwafp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2sxsvrwol.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2igapstnc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yjvabcix.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2woalzvjr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hjkcuayx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cfrxytcc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2usuxjaom.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vnwilwlo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2iamudzzs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2oadpzvzc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vadzsmjv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2eqrrkutz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qvyqvldn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wtyavzca.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dptnynfa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2foaehbci.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wbgjvdrh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2egsoxznl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xlkvolsd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wkkvacqx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ikiczico.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xpvwipow.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oqksdibg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gcwiofgx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cxqfuayw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lypixvqr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jovykhew.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ssbpqjwx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xmahxwcq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2glyqezjc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2adrroolr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gwmnajew.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ilhrkxrv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cujyzcwe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gkbropcd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pvkwcekf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rbcmoeud.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rzwxwekk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xelekwjp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vavnipyg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nrnyxlwn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ftkavigb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xxthcybr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2kfmeasnx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2argbeyca.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mbuzeqgm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hrwitmpq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wnzuwphe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ktzzyvfq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2thndpftv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rqrobqur.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2upbzffqp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qmrjavme.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2yyovsafl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ifijgaey.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2atihbxul.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2uvqbwuxy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tbascxkx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oaghsgsu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zrhyxdou.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yuyvrsdv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ratjelyl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ylqwblye.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gcgyoatf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xfrxsbmj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lqfergxf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hxndveck.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mhhmhcoj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gelrnpta.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bysrzkur.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xzwtnqkh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sehmxoud.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hxbhfxgr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mcjzomgi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xtdobysf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eqyfvmfl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2baoxwkbq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2finahrly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvbepebk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvxrwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uoksubii.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2diyaubqj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dfpqzcya.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yauqvako.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2puwxnlxz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lhxxxmwg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tiixlnot.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xoddgupk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nkeomjum.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mkwmktno.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jlcmlwss.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pfpmudpv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ushilnpu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2fcplsytf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vuymfwoq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yhwsxnca.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hwnihjqt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ddglcipx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gyrcduyz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hndeqaqt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2uzsffdfh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mzmbkztn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qteachak.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bcnwlumr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jmjmslvq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2waiprybt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nrzbhmnz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ealtlapy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tamyzgbh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jdptzzhi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qqgxjozm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jfyjjabq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2thwjuqzf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vfsquqzd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vqotlpqq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ddqfwewt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bgcniyda.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cwuvrvvx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2oxjwjttx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ujbugqiw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ojmdpobo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2eliufdoj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2yqngihry.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eabitiai.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2laskygli.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xvchfoxd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jqpvxqiw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sxavrcvp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hqwlelgf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mojacnhn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cfftphos.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kbdunnem.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gmxerjhv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2axslqtzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkitwszk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zazncduq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wrxuulee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dflaxyfg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2scxantfm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2mhxaeqqr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2pfdlfhxe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pyuqbdge.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tlnkjlur.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cfcsousm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2cwnoaell.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2oudiwmvp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gpxlmiib.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2hmpdcudt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ldrtnspq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2khbylqzl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dchspaha.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2btbzdizk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2hxnkuifg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2xupapndg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2uylcgmkz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2bqpsiale.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2yuuxlknk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2sfdkzqlf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bvgtdvxj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2spmtygxs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ktlwtdmp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wxhnqxzz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bgvfazsr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2znomrmrv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2azjlrhxr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2svxtdrse.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xpmmefvu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fabgabmf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jjgwxjun.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ibhklvzx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abibcoln.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xtzkhaot.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqgwkcaw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ufcqnmvh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nqasxnkf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qahcamum.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2htrpivge.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2gxxlvomm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wwawlawp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejtvhwsj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2taqdpvob.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gardtrpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slhesiao.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2iggksjcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaeihybu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2inbuzqwc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2njzzyrvo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2knwliolj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2barcdawl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2tedaboci.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lcchkarp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gnxtatbg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tnsiokzi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2watumrbw.html


<!-- 参考信息 -->