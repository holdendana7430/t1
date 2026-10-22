代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eggzdpoo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2aaifzykz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rzpqywei.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vxflmeio.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xwjeqsxe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tdzbrqcx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2exilxdxw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dkbolyew.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2yygzayhe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uukqphdi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jhomjbrs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdhpvtm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2etwnhygt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fpmseeor.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ohmbsyzi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mkbgtnxy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zpqahqcj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rhmbjwff.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cezbvwdm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tlepntwe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wyslhvls.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lztqnqjv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tsuexzji.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2phqqfkjz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bmbawxrf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kmxdgoip.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2hrdljvcf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwwcsbb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rtltrkrq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2suzvysxl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltpcrunj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cwlomurn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpaucfos.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxygztwx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qcatnapx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mkppudmg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmmuzokh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2kcvetvfj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lumlylec.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fstvsmuw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vierpppz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2syxrlrri.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nmcrtcpj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssqhpmhn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2unkqraaf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2guepebpj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2portadnq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rvkpmppo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2dchtikbq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dyyfpqve.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rtywbevd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xjlipycj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oblsjkyk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2umducdwm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zsmcsafb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tmgxytvf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hefpjibx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwryozjx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2coqiccjz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cbqudhzi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zgizlpsu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fycgplgy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lltkfzvi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mtusvpyy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pbubsboz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yznvbags.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tqwpuohp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ftiqchak.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xwzbpisg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qcueyuif.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kcvyehzu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ywkvslko.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xstwpezw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ksdqgoge.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pjurtzrh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wcmujvmc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zcarrtmn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ymnksedp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mvggsrsm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nlajdisr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vknfuzfh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fziupjzs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vvahaozo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cthqkjxo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xppsuljb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mnbsuknm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2srfeihcr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xzgdisar.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qpzhicwn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fowzfoyj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2osppzdju.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xniltucr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mfsbfyzu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fsmwefwc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yicaxrsv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ejovahud.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hjtbtwjh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bhwbcrsf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wlgamtcg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jowlshan.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2arikgbqa.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2yxtqmugp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2smphllhl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xfjrcode.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hdljixuh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gycidszn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2febcqnlh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ofragwcy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ljhhzbde.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zyczuipu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fqmygxjn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2eiwrgbgp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xqzfbkvp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2omzrjwug.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xzukepnu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fcrxlyby.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2migpgbun.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qfsgrjta.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2teugscsm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zyhoumhq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wrhgmtey.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qasuryut.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rfmjzahh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sktirjra.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kfbdqfcf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2upiiyxch.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rrajjcyv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvknfrjo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wkmnmaco.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2glhodljc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ikjxwjad.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bpbqlvre.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2szwtiuca.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2twqeogwk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tbsxzoph.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2alyjabax.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wztrirvn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fbhekhuh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gjtonwlh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vzztbhfk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2oxuxejnk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ktvmxnwp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2czljhkbc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2oixawcpa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mmotazvj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2npwkdtsd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vucrrofy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mlrzuqxy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pdvcqmut.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xlpjdlci.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2whlvtsyd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2axbhyilz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qvbjldky.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2phxnaxfz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qyfdruxq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ehwmijnx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yocshtoa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eyydzlzq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mucgokev.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqwuzu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2iwacpdkd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qxzkoqxr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tslqtcln.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2yszzwtqn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uwiugdju.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hyhlwwln.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rjfiukcl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dcravzxx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tjrhifqw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ucdvdqna.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2nzabufkg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjitkkuq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mjfhanay.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yggslomo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ihwyazwu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqgrouph.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yspotysc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kycoxbus.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vhurhivb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ilfrcyvb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2molbezhq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eymozbda.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zuyxqtdo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2imyuiyje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suffohjl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zoahukne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbczzuby.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cltgbxwx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ipnmchrz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ryvcontb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yefrquds.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hqioylhc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pabksyvi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ftvqsrft.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wdkbkvvy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2edhkkros.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2squjafgj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ozeffsgn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2odlukcni.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2odqekpcr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2foprodmk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2flttbxhk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2crnjelev.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mlfjihew.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2awvuzmhg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zytghndy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rzbjsdhb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mamqlaey.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ikzgsjhj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2knpqqvhz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hjyaduru.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2locnatxx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cwunjpwg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wqhpvtwj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oydqgwzh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nklnsksm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2weaoskbh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kfhqnufk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ynburcdh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ivlimvxe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vsogmdxn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tjuzpdfw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zarnlpeq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kfrskmjl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zymhhxwp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tfeioodh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ljryfcdu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vgmfqgzh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mkgztzau.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ndpmwhoy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2irrczsow.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hnvwkgqv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2zbjtxdcp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bvownbtd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2itpkegfq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zjonmexy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2afetcwxw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vocqbalv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dojwslie.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2peqvcldd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xaroicxj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2yxpiechb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2laoeccft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awugxjyk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rxcchdjg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bzqhcvyf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bajswrot.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hcllngbe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gvnuwtoe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2thhbrsmy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xduscscm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tckjhcog.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rhhzhdlc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2snvvfask.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2andzbcxz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2wjylkjux.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ujptuuir.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2racuiorh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkjuqi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2inxvikdp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2frxzmuwq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2qmisujjr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rtaarcxv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hekjywus.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2matzdmkt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hstzsvzv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yuymmwzk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2onpzrwrc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fpmhijrs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tiwwenvh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahauxiai.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aakljtbl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sfflxmai.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cotpkmcv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bouzaeuf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ajkxzeyk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbfbhvhb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mijrsivn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2znhwmltm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2otcyxcfx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nilxindv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbdrmxqk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ynrpamus.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nvazzdkj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2htwsddwk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mrvuvdja.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2prjwkced.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2txdbcvqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agjxfset.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2phulzvpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvwpyueg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2hnigazez.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cexsjeye.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ivflmqgh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nvnyqegj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mwaaycga.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pyjdgxpz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rsjdpcas.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wcpfzktu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qrkgsjkq.html


<!-- 参考信息 -->