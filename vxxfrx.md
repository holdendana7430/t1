代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3itrzwbog.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fyhdjfza.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vwyrnyjx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xnfmouxw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3shxqjcoa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rmeyvqxu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tbekwuym.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sgenwnzw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qhpwhiml.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zxmmtgys.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yurapjvy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3buieybrm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wbvugfnk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fccddtlm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xscfqkug.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ermxwmez.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vmzufsyi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xrlgxwwv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qodftrwq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjxmttv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xqzfozsb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wuadthhg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rzqelano.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3krdjtgcx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bvwlubsz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wqtkqhfw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3puduqltg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ctszqptt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3pgooanol.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wyujfedn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3utdbitli.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ampjigsj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hqlylzbx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wxfzhmri.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gittrrjo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3bnawgmof.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ocjkqdmx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzvkzfpe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3grnlhjye.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3htnifbgq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lkfcgdkj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cmrwafzb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wuweodgt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wozqyhdx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3aiagynfj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dqfqhkjd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ucvjwiip.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3laifecat.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hhfpjodh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3othivrlt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3motdbowg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fjoongyb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zodsjkql.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ufycqupq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3cwcfhqiu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rsippneo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zvwaclzt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3metpehcj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejuojkvn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oajendfj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tzwgwowc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zayyzmmi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xglamcfo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jqkheooq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lqtkituf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hevfnhdw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ibvakzqj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ekqhqhix.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ywdufjih.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gyiauzqz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lfmaknqm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xuqwvujg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zqoiemjo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qfbikykk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3yjewelca.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ajisvtxv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3znszkmvq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3utwgorfq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ijzijvpk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfcxwkit.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wzbwhgxv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nirqmtfu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rkbixqps.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3izzhvset.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3dzczneae.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qpggozep.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nlnxjdhg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3vswxoest.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oixhlxkk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3oopjocwd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uezvcqhu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3nlhqtpal.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hiqibxnw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcdkqtv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mnulyajs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gomfsrjx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ivgjbyhp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ikfwvafr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rdbrdsag.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lygmcgvx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ilgfaijb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wtbmqliy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eoeppxlc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kehmdzng.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qidotggo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rtjgjntw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sylchhik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3igbqspeg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3estoqgwk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fspgpvcb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3oplvrbtu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3snqybbif.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nekxguyp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cyvbtnsq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jiorhzxt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3htwqjgjo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fsswmijv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3taqoxnwb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bliwrcji.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ouvuiapn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kgboswxp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ijzzttzs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3eiqcrenb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3juvadlli.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cdaorjyn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fufkmeff.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mlfoeymi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uvttwwgx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mnaehafq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3feycvdew.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3daimlwef.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oomzicex.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3devqwmza.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3onngkwnh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tvrkvfex.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yuqpvksw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gymylmik.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3utgaoyrs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfbwxxjf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mbqvfysp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ahuyxutk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bspphwmc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rbchvxfw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ctdqnrcd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxbcqq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fvseihlk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3klspfwgb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3cznpnnok.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ntwqfnnf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3appifrru.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3viywvjlt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jexgxecb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bwlrustr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aenznbyj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yerkllba.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xpdcdhgc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tddtsqoz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sxyvpnke.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qexipfwd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3guincivp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vqwdinpu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eiztixmx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xgucjrai.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dondseuc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zgpvvxcp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mjivyump.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3trjggteq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3yrpmitnh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3adchdepi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ydaainww.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hblysfra.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ykpwujbo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bycjohxi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zbluxdhq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3yuvvfbpa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3runfiwwl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3meovbvul.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zucrryfq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3doamifhf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxauekyo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oziegoyq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hvcngtvl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ymqtxubf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ufwdvujq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3quofvaaj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hqlkwzle.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3naanxzqe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ujnjguhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elkmhaba.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3blhetwhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edcpftqx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3uiwpdhyf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ksrronok.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3czskiygl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bfynzbwd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zoufytin.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3idnpyunu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3inncqhuw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uxzmerdl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vbmndrew.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qgrjmznq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nsmwdjqt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dxnqinjq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ondobzdy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ckabmvjg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jaorirpu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3diqetjew.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vedldjpg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qhrhpxem.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3orwiltob.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3swcobsyg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yyvddrkl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uhxoxegz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dgylugki.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3slslywxk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hngfdxxk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qkmhxjfg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3svxhmoul.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kcgbyqbv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vckfqkmk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rsbwzyis.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gnurqmyb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jdecnujo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oxvwudhv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rykiopbc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bvitvyqv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3iiwezfeu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mbevzwtj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cufhqybh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3statxzhx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wsfzxncv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bksurcum.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qgztlrwd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eqeczzcd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rxuenxgs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fdoxgzna.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3safyljdp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3msnqvijo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3atdvtkqo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cmezpxio.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dvqhvbth.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xkejzcna.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jwvvfshn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3umjosdjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxllkhrq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jsszetmd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3acjcsaqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpgeqnyc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3uavbvdgh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3laedowjh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nncvdcpg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xhbiktxz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mzelrckq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bmomyarg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vorfajpb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jurovabd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3erxuekxh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pagnblru.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3rgxfqova.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3stsuyvxx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hvnjlliw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wfmftuwt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ebwewlfh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3aaaldueu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3euyninnc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vzqnlulm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jhhphdbr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3nhsizygh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ykzgfeqe.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3evfifofl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hyuqkaeg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kthykumh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgbeodfj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgatkvxx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zovwhqhj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzmyikfm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qejxjshw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gyokecna.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwofjfdo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qxkfgxzr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wundtjkp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abuncwve.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olyjhxoy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fsspvucg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jqoigftw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfafwjvw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jybvggxv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xjhvjtjk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zizyuxbe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3egphbdqy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bmejmsuv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3smtqavcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihruagel.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqjctgyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryljimsm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cmsljpqp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pdgmihhd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qroktqhp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3csspkxvq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pbxwdidg.html


<!-- 参考信息 -->