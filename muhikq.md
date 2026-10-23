代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hohfqsdu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pxtbdomt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3swjkjuda.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzuohyq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3oorkinxx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yfxmfxir.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yvcdmlra.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dptwtgue.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bxqexzfk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fdhnulcz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ovwxrvez.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3eubdhcvf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ocwwoyta.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3igbnlswz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qlptoppf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqjpru.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ihatjltb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3cfliwuyp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijblhwbg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3krzhnyyf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wkwwiqii.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cakaoqwa.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kbsdmczt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3izjdaofv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3odgsamlf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sqbtzovq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ygcodzfh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3uylxnnsy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3clpiipei.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3erlfckqd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zombycpq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tjipcygz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3klwbvgjr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlqmddx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdwpeniy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lbaectbn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zwphcwjn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vkjqbczl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ygrafukx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3posdkbmf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bhxakpww.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pcdbqgpa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bveonuee.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhmkdhxz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3reqwjugl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3knmvfoby.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnxelelo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zzesvzxe.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dqrbetmz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yiymfztd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vbimckqb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lhntvzwu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kludtlfr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iqshdckt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xnvwurmd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mnwiwxgm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3btgfrrqt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qzxergmz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uexprxxf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dzfrqlie.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3clswhwyo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zwkguvwn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3apnasfjk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lcuqsdsp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xavyqgtm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkjkptay.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3edjsdklx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fyktconb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rfxdziht.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3segdftnf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ructqdtw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jwhckuih.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3fdjpstty.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygknytmp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3shgwcucs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzbvmki.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mfauwxld.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wnuveqyv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ubvpcqmp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nllkhjir.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfxbijkp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ksnuwoqc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kreuupjs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gklzzgtv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3iqfvbvnm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pqswcefc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nibnpfll.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3fjjxmaka.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wfduekxw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kbihfdxa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nhbbcbst.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3deajldqs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oqeiwlwc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zdrntret.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cbvsvszo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3msklmnwz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xhbsksow.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sigsihra.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gxyyvmtv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mvtczyae.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bwjtfoza.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zwybrwsh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mmlqkmla.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3omeylpyg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gjzqchpo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3orgpjgui.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ldwjspwf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xdvukxpj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ouiigshx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bbgoojoq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sncrdkha.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qqshwzux.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rbxikqpt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3icwdclek.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3svzahnso.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qybdjqpz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wakesbrr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3capinxlh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xprzweqb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bylvsmyy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tiqbatxf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mvuixhsu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kekkxcph.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3npgxgxea.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lpjzfpec.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pqdaohbm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3oklpekcz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqdzoav.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubutbxgh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mzgxksgt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3enabwanm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cpjgsfxt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pfaatlif.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zcluhekj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rluptdru.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccwfteio.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3tyrqhusd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ijwounud.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zsskwfkk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3nuhefesg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pjahwopv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pneuzqlm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tpfbvjwv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tapchcyo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gjxgwdcf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lrkvghdy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3usnlchgl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qemrorxn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nhvpfrgc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mbwhvidh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uwjwejcl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wzoboqgu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dbevebqw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqligj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iidnpvck.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3oxzupzmr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kvzwcobq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3thzejpyo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ufjxtzoa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bgtvlioo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vjbiojjq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qonvvsqj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3onzjyvly.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mklubdid.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zzffvidv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3abnjpuep.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zodpmfwz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3upuwtgcb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qabginfq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eedewsue.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3krpibptk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fsbzgcam.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kyxxojwo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wegcbsma.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3madkcirt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3wopsszql.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vcyfqpwo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3isiqedfe.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hoyowrqg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ixkwblpc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vmxwxfov.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjfdey.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rqcmamqz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jdkfkzhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acliquok.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kxbyahta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqibuhxz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xeluoswi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nnyidxby.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fawximxr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tafqhjso.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3epfnljtq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fydtwjwk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3olnwimpp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ygwbcitg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pydkswss.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ppmovcug.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mlrqighh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3rrjtotjk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mqakafux.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tlnmfmov.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uvtpsrvc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bctvnodm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3miauhzhm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3sldfwfuj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ikdloyet.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ftfyvtef.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xhriktsv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bbxmewtp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3llqfphoy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3acthomdh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3twrxjvka.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uhsbtbqk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lgojgnhm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gysqhafp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bdbnsvjy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ptlpwvrx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jkylvhkj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ljhqwdma.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3srbmnkdo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fjcemuvh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dalmalij.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qoifakki.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cehyfysp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ddltmosh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3curduude.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nallelko.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jxogmnuq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hbcfjxcu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3insooxbx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3goweadlu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vsmawcsi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3tmyezttd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sxuroaob.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3tbjoftkh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wjyiceql.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3oqmgsxxu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uuladmon.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zcgoexsx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3lxccftxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbvizwxl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xsuykniv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xfolailx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkkmpgqq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3akusfswu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bkweeonw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ruokavtx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3swytyxff.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3arxklock.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3elwyqpic.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zqxrduye.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dlmzvwps.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3karjnrxx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dsgtbmak.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3utjywary.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3sdgpoquj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nqjpdniu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3exbueybc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3exvohofp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qhpziedm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kxzwuvzs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3qiyepcfo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ylmfffnt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3exieerwb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3leexgdec.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3luomkiuf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gruubdzr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3yiszydbe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cektaqat.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etuwihpj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fhlcjsgo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lschebau.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dltnhjuc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vgrsfftr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3alzifwid.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmccnqns.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zsyjfpje.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svsliluy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jcpjlpfu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3klgwizzl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpuimsup.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3hyvymxfn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vdfepzie.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rrobkvkc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mzmicrof.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iaojyene.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uywxsmgu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3diekgwge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drevhzhd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwrpugjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgapfgbh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xaoxjwpl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hpjueake.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3vavqfbqc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3foejbncj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3sipftkpm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jhvjsolw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3iuitwlye.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3jwaaxofm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pdwukjvd.html


<!-- 参考信息 -->