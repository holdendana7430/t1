代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oljflccy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pkpvtfao.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2djvwsguw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nrepkqnv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qkzoperm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kuevqjuq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2izefzkll.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hjbpkfop.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2aygazcfk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kmowugrq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lnjdsmbb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hgnrrkxk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2aoncqfqz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxncgbv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nhzxsplw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zpbbmuvt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mbhntmqa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lonulixk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2clhybhrw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bxpvztmu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ejmnfjrd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gvvwhjga.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ysssorzt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbycjsp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xzotublp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lhwybiny.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bfezaiqa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2muxwolap.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2eoamzvjn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pvjhrqks.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zgnucvrv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dyxzfuzt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2slptryqk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osthuogy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fzqoevoz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jgbyuaty.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2icgnktjg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nhbdsrbf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2txtpfrkk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfxjzudp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jvgufgwb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fxmgbfnu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xbpenmkv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2milgkizt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2szskdlhj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gzufgmbn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xumsgfne.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ojbjlcgg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xtehrjgs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rsvbinvn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2reauiwah.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zqyjkpsv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nvwdxdrk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tfoxhcci.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iuiwdnyv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hblfppje.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fcjdoyyy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2lxiwjvyc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2azkfwekg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dsmrcbyw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gxbpqkha.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2untgowoi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2iugwkpzz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wleroxal.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2glxwlvxh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nnowfstq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hbsaqowx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gyjfilhi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2obfiluvg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2kkcnhijf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xlljilnx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2alaqhkbd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dicivdeo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vykkuybb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kywdchbm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xnuapgri.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ddarpcdx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qxfbynvn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nlvbztsh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2bmieakje.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hzmsepry.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kstthqev.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pubuzwia.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gqitdanq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oniyqocl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2keyezckm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vzzuyijh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bemflfpc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mfcsjlht.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkwligu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2icmgmslg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jwlneayz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tglejesn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nsmfansi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kyzajzvv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sandwqsy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2blmbbthi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wikxgqtq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rheoywsg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rymggdna.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uehryipv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2obazhoip.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2edrbznkg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lrttyctf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ahfrympj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ortglshd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2csjpqwht.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlfjtgha.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2aiinhpyg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vyrehyxj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bcmfbpjh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2axzeupzq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pnruauid.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gcatnfux.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ugmqbwgd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2akxagmnd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mtrxyanm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2afwhlhlh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nikrpcrp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ouqpvaey.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2uiqibqqs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nrhijxyt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qujhzhyw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kiarizdp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2eighfeqe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cyjmakiq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zwfblkjm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blbsnexo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tnblhgze.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yscvxwvv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uputxqsq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yszteijg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fpbqlwib.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oeqsvhmo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2oejvcqkk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iafscynr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ipyagdrc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ffrdmivw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dlkzihqv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2cyyqjfsp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hopkhyie.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jcuukilz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zsaapgcz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2zyzxuhwn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vmrajwlh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2doxckgsl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2teicdbow.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2sxniqvgh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2krxstaod.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wyqjkdwc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2cqhpyylr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vjiorinm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lqduteaw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2agknatpp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2coultyui.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lmejnhcy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nwdidjfy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ybwyzpvf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2buwjjspr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zbkleztd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fmactdpg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yruwartf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2flpkkgoi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wbxtcovh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gntizesg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vewliocz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ebbkoxza.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zdvrmdsw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qlimodpo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxnxllor.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bkepantj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvqjffc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tqpukcts.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hvobieuo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tdcwooox.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gchzlunv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cqtkufjv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ixpdqnki.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2kdjnbiyn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nwpsclmn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2htprxkzx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lxilando.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jnkvysmd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2blahocal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jckvbjhf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ryvogtjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxrwvuee.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jkdgzsef.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hmiavsnn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mtrqcalz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ltsfunkb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nxvbvzbq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zjuaqfmb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qhqmeobj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bgamqwng.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uggwgxbz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mllpjgri.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hlstaile.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2iaamrxdj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2gnhnvheq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2yxbfkfmw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sshswkiu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2tbbmdhxi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2twigxnmh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fjpkenma.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jcvnazme.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2phmxpmov.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tttvdgvx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ukavdhew.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rcvsmtob.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bzxjvzfc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pmswafyt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xplsoigg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gxedfnck.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tajafxxq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xdcixjrg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wgcikkcv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zwmuiftj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2grgbhzup.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2anshxpyz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wdlrknhp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2phmmyjwq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2njgbphgy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mrzkrnyp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2jbgpbnzg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2loastrgv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ukyizbad.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2haqlcnyi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vkwijkaa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qbsgsfmi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uctduigh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oxylxtol.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2avkscdzm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2owdnxntp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2uxvqwrtk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jorxzojl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ehnlyiuu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2chclalxm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vjydemnp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2qbtzprpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2furwznzh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2oakblyyo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fdakirtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpvttkei.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vtulmksl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2tqegwhph.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2apkkozkj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vugblvqe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gajiunld.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kzkycpwd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sadechcj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fwvbwdqz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2opjqfheq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2itoxpewy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pwuboafe.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gizburaa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2zyfdzyrh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2cbfrfxje.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2hxheuees.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mdzxlely.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2eupvyroa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2qrrlsdda.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2matobmkp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qvzuwxss.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dgxntfnd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jsoighsr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nzpgfdbk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pngltztl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hyrokbbr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxsxrzjl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtdldpdl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2uugobflq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2eghpxgph.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgqpncvw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lpnrkqqy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2isedxumd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2suhvclui.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qcxvsrvt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pkzsmfqj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xryyijhy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2eoxymxno.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mgwsgomm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zisinrlt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2falgrgtp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fitcbvdv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zigvtiqi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dprpflld.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mxmlahwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjjvkbec.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2cjtixsjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcbpuqvb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2psdunjym.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zeqtiqfm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2dofrfube.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2szvuzcim.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ycvhzrdn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2idqmexto.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cizdklrv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tsdvjyqx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ixdmmpol.html


<!-- 参考信息 -->