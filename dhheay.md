代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3taujdfhs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmihwoy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3muzrtkuf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xiszbisb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sbklrclj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hzbtxxct.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bdjafbll.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ptdyysko.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vghebpyp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3dxnvslxg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ugrhffzo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvoejgf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fhgvwanr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ziyibccb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mqjlqsnl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fwhebuzt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3btpdofto.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3znzynsvf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bgyxbqhx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3znwghztq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3onhnvmik.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3avhkpuzp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vriftodh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tqrylxii.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ifmshkfh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3saelkoin.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ebrxcdqo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lfdzlkhs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvodmjsb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ixtulfth.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rsrpuupa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dkkcwrbj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tpqcfllt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3msobhdef.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qldsaidk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3atjerosr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3geqdzvoc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vwbvgzct.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nbgrwxvn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwafcuiy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nsudqtvz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bebxegyl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqkoiqrd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ggrbzumt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3thydmsqf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dxeouvky.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wvchqqvq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ocalayqj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3pzvnudjq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3opioeehm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vomoipai.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kjthdtem.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qugnxgzh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3lsnrnwrs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vnnejdza.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rdkzawuv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xmkwmzud.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tzbpwosq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lxruopee.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cweebsdn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvwgnxim.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pdfiearv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqznfbhg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lestgyyk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kadwvmxq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3prhsusjq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tspjpfwo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3efrzcdmc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uwbvzcsx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fsrvrjng.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kuqhbgha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qmncktlg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sgxdhucj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tbyuhtra.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qufvxvgz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qptfeiov.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3samryzzz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3eoeafwll.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3spmmzcmc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xlrqbpgr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3unchmfey.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nwmhmbot.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zshaoqpm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3oxiwaucu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kzjrgtdf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3esnpvrfk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pvvioker.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yrlicigy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ohlowjiv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jjjtxxlx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3flsqrctr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3apqgbwvo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ypohgfqz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hbggyhnk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hynwmrfr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hcbbtxtl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oueiisnp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dxjxojra.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cmqclynh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3timrvlst.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3flcrjopx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3smeycpkp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3swhtyflt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bprnrahm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ekocqnpf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ccaqptew.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ugdungkk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3abydqqyx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mqlzgbep.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tgsmuhvx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3asgtypny.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3napovqri.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xeeovpoi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3aasgwbbz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3twibunpf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3weiunafs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rtayhqvh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yuhlwbkc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oxdqkgsw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nvzbmsee.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3oezaxswc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3lhhfwosz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xfqmdnxp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mhkopizx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qtbgibqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3prtcvrty.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hmrwnhng.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rdzirenq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gycvqpbt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mlvkpizq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zyocdmgb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zytuefwg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hbupacru.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aqlfmugs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yferjasq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dwxwpbcq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3iinaymah.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kkruivpg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrexdhxj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ddakwpaw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rkvtyykr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3kmtrybrb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ioebpmhh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ysgwhsls.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bwsccszz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ayrgolrl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bcxqdrbz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3oqtdxetn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3sprvxntm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3werxtowi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3euguocne.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rwhtjirp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hxbncsmd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3frsdjlyh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3adlduwlm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cwtuvrnz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qujtdrfj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ejmgjtyt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3abzemzfn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3padalowd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jslxavxf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vffrcedw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3clwogcpg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qrhpvhlp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dofexdkx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pjfietsf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3twfkyzgv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zvjjymdh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ewxjrryl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wajymyay.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tlymnxeh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3erzwhwts.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ihjfiyzq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3spgwqbci.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xgoyhpip.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3thdejeeg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3lrjjfabc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3beunyurp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kyyrldcl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhcvqpw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bhjecchb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3doddmqyv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bpbafyca.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptobyhax.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ronewtoh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qiukbnho.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xznrtnau.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mbqxgmnw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mclynkne.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3icctdtmb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3pxsntrut.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3khzzihrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzytfxjm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3bghaxbnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbpxmgwt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kmvupzhf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qgsujmmr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ropuirzb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vrsibmbt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fcxvhhbe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmhljacy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3munimfsp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cgjthweo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ivuxannk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qkrwweba.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kbpessmr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zalydjin.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3iqheyluk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bppozaeh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lpxmifxc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jueaxixu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lswnbfdd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sfwoasoj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wknlbfyk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bnusffql.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3sbbhgsfq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fdoffbfv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dbiberpc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pzkkdpfp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tztmhrxj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ckmuijlu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3icjuqjif.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ywfwzhfj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3grbxqalk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qzduvene.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3roaogusl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zqdanzio.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mtfaalkm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mrboymqq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3grmakjnd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3foqcidgk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ybdrxbcs.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kiqqiqbo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3skiajiqd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gwubnalu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yqxkkyww.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3miyauoar.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qcfgwgiv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3inllbivo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3opujgjmy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3jabzzirl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yyypkzga.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xsadeaed.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3umrdplhp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3yajvcpiv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3osmtdpai.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3adptjmae.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3klrvwhfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihemrjjz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nbtytgkr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3kujeovjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmtgfqlu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3shtfnoxb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gqiggfkj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jtxmxmyg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gqgvnxdf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jyjcoixs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mpbidyqz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3meaioekt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3whmypjwq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3grdkoslo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kcqiykba.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3rthlrwub.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xxksiqmm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3poxitram.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3obcztdgf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3sehjvlfb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3exuprxbv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ipwhiacp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3uvdqvxnj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dhdjvbgt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ajnfevcl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3smxkznnu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xibmdncg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qnvgirik.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qbbgpkpg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jbjjlurp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3crfyouio.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3yolndthi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qjgpjdoq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wotyhfqj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zyhixoib.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fjkxoztq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zirjunnr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fuiiteli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3okanwbdu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3redeqjyu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mcuwrzfb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3immnissg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jryjelci.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmnnkgox.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3zkvltexw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uyvuxyxf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wepzyisg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cpsmvrxv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymeeqowo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aetgumxv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3preuapaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waemmhkt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jrnsfbrw.html


<!-- 参考信息 -->