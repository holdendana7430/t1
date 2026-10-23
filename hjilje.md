代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dprtlczt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhrfxhi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qxxgffij.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ugcneekz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3eicrojpu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3etsklbpb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ueoygyoh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rgohnnxt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qywbiqlu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdicjf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fuyagauv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lhmobvmx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dqgwybfb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mowbwjrc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rxxhxbth.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3unlvelox.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3nztdksws.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oeswkmfw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hfsknsms.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kcawdfdl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ikulxhwk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iopbkixn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3awvcuwrn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3svdcxita.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kkhezjvh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hmrxkdcd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3amvnqhun.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ivtsmwnc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qyxaltis.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tcicflxs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cvssewhv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dtumfpxu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tblpfcpj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xayctgnf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bcpusqdm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3okxmxizx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xnommxky.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rzohqtkd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqovpwvh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddsjgiru.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nlmuwovv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nzrqproq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vwbzzkah.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fembqlsy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mnhojbjb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qpzxbbdg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3udlwjpzk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zrngbjoc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hviivdfx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3oreulblm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ujvearxi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wvjzxkfd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gsnpzpuz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wzdenyls.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3itdfuvnv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vilkkzdg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gdrekeek.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3eqgmubpr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3yebpddlh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bjmczvrj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3clduuorz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sdrvlzhl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bqbuoutp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lusriojt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jmlxtzbg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3cwojrmdm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rfngwjfv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cgaaowkk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3iptixsjw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qidcuyke.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mlkafwfh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uxfnsvmq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rztzgvto.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3snqfcsbe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rckzfqrb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3aizzhcsz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3aeqnvves.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kgdpdhdu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hnisimth.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gqjnmsbw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3etemlzfv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fvwnphnd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xwygazld.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rzueatpo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rhdjhazq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tssbrkbo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zxlgyqnb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lrtzlnjn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3raxhqnup.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3czvyhkyx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jwjdwxmi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3edzkdogf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rroqxzty.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wpmrekpb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zlcnsnoa.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xgkxdqva.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3clhnuuai.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bkdumfuu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ggssvpvl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tznxgnvt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fljdybfm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bkuuuzvj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3sanuwyil.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3miewbcca.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tovciviz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cpgymbeo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3enlxcost.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tibbpnki.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lzxqkuuj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lbvxbake.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3idsozagk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ylnzlqqe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rqwwojhz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ejdvhfsw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pukvpgli.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vvrmawkx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3logprqyj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dliuixgh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3tstbgjvf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3asvnbayp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pyqspdee.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ljjkjdsv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lxblmwhh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aabidhtv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3apqtwtvq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zojyayhv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gfyrxowz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pnwdbghb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jthmrsly.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rtmguukw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bvretszi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oaolvbpp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3soydztqp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ttjtyawo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vnczmprh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cbomxcwc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cilkepfd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3unpjhjty.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzdonivu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bxqfacne.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3htnngudr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bvthfplc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3raiptshd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jogdfqtd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ggvzciye.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ecicmecl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jvbyrdhx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3saymltlv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kjwtgkfp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sbgxseab.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tgcbkbub.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3paaleded.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qlinicoa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ntzimduw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3thqtqppk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ubrivalh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3flflxjqj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3eesupmgq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fxohluls.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ndpsenwg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ftksiczv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ukxtuwdh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sigbnach.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zzzosykn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nginsfyd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vxssxyqs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gotsrngo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3eyqifnfu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nwiruzic.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bqdaqedt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3awpqipxf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vbirzwcd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dxzoeann.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3evoqjjft.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dzsvjnrg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzxfxhyu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3iecphftj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sxdgzmgd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3apcxvepc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzoioilh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tvykqfoy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3whexlaqr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3pqgtychz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3thknfulo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hqdgcjdj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dhnpdlgq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3folfyxem.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ppqlylza.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3yvoslhli.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3cjecemjd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dzvosocn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kfoanssr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adlsdzko.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ikmqixdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wusvxqot.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3uiqjafzs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3brybjmqj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3owqkrccc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3khdtbtof.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3szarsjle.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qofawdkl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wcmbabdn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jxmszuwc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nkcppswa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bxldiafz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pxziynpc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bvbpmjcp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nroupcjr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kkjvceir.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zwngkwmm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3phpcthlv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3walvccyq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3whojkrfm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mlbnwlaz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3whlatyea.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3fflxrngh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fobcxtpy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bpfdkixf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fhcpnwlg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dpkpuiwt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3peympmxy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3odutrxeg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3giravqcc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qyviiose.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idbhzcup.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fomlicnd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jozrpqbb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3znzoundb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yobamumx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zicuhsrs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3jmwlyyrq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gjtxarqr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rvnocsru.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ohzzyljd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3chzmqvxd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ggomzzdb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mwtkckwj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zqookieo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kyiwcclf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wkhhijlr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xoellvns.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uduhthxw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3uzctsfza.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bhfktquz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dzsjoupe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ijitxiru.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3xvgrxlgm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fsllwhxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aulmyesk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3oyzmzgjx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pzuvugfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyozggas.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3tfmgowqo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ezjiqtvd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tgbqondy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hsklkulv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hvdgqxnc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nqyftcnq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3okakynol.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3jnoqolgv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zvbhlyni.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ebxfkivz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xmheubce.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3lartqveu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3cqungnmq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wbnppams.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3uzoyrshp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bzsehzae.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rqlnojpy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pirbcvdj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3iijrbxbc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lmddhjml.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lnyrglcj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rmdubhwv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pirtanlh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3paiuabdv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqcqlcqh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rzdaeiei.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kjcvhlbh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yntwkifs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zkbtzeya.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iqildigr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wqklrjqp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pquilkoq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbabiffq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nqvngpcz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3diknbwuj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flasxgmx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ohjhiwfr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jxgivmsb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xptgsjjs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3twnglrvx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mzjowowi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqfqofxb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mjxrgtqm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xqbocrzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsuapzic.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxzdatza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhxpicqu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vhfvjudq.html


<!-- 参考信息 -->