代发 wailian999

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gyczfugwz.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/garzhlqze.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gdjfuybdf.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehsgjdjq.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtbwehro.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/ggunvwtly.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/goqivgsmp.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gfokfqseo.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidmzriod.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gncqmiqbm.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/ggkafvzem.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gtwogiplr.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gxishudiy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloetgiad.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gekfmiipv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gugyjjbkn.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpcatpqn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/giqjipvoi.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gbubmgxmj.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/grtgdtdfw.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gobknwcbd.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gxngjhjoa.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gmzcrciix.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gtvcffunb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhuoyvpc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbajyxuw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/goddgdxqe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmncwaknz.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/glllyjcdt.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnvxpevl.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnpeubngb.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfytglds.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvznrifrh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaoxsngi.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkkrkue.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/ghnixjfft.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmkvnfjn.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gfgllzbsl.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ghckziebm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkfeyvbht.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/guxwbiumm.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gbluiffkq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpornvhe.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpwugkgro.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmuawyen.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gryrraiww.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnbxmuxi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgvypyng.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gerxdwyzo.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/glmllpotp.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmkvlojs.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gzjxpjynh.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/giuvsnftn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefzczgkz.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/grsisvmff.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsafrpuai.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gprrpfgdd.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdbrrgcp.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbxcmszz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzanjniny.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhwtvymu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbevsbyb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gbhbgbrzl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzdnbjeb.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gyugrhqzz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gteqfiotu.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrzdwrtk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhuemyxx.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gnqboabea.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmtltmtp.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glxwcsmwr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtpsdipz.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhwcurhd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpiihaise.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gmxzgrsbz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glraotdvl.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdpkiumj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gcrczwcoa.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gbxvxaipe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuejwekz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gplrtefdl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbjhlrhr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/glxcnhdmy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkcarpch.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvavdlctk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilllemoq.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtjcxltxx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gctjdiovj.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrcsoeds.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gogodvuic.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtgmslbt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gorvefixd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gducydpyf.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoagelcp.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/ghutehtgx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfeifgcv.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/godcxvigm.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gokzbqcdc.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gtubogzhj.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gbqzarzab.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxfzfcce.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcqvkssr.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gwsjypjgo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqwylalk.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gsijocbpq.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrpiuwco.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/guoamcnet.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdpghazb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsetghpj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gidcvgiby.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytkzzibt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcvfwnxh.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gavpqkjrc.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjconruh.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gappvagoe.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gbokshtrm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhqythx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiixtdqy.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnsxfysd.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkuzlda.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdtaltzo.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gqxoulqrq.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxrgedar.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmrumoja.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbtibzlwo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gwgedxlig.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gphbwgktu.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrxoihga.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnipffvyi.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gyvhlgytr.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhtskaty.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpgghpjk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/getjvhnww.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdajhxajo.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gkxvlrhxf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqysyxrs.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gyywtdrtu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gigpggwko.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwzzfbkrt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gnhrfpgrk.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbnebqb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngifwal.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gejkmismt.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gaayukrnc.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gumukbjuf.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/guehvgzqy.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gbndmsvqp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghanbjqwj.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/grrhsaqmi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gecneqifz.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavgyzjex.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gomkcydmn.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdwqycmj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzylcgnyr.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqcnbwmam.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gkathlybe.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gdwultqos.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhggclmq.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/goosygpxx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxunotiy.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gkywwqlrv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjwusqpe.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gqgznqxfv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/guviipolg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gieutahni.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmktqon.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gfopsdmci.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjlzwte.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzewkcgt.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvtaikev.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicwxuqdp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjysxvpmh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaxrqbfo.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxbrsblk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gguvgwkud.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/greeyrmvl.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqpxepcz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbhkuhvc.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gijzrmmxl.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gtmnqfnsl.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/glqsypwfx.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gekhkscwz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geclrpkub.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpcsmfty.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwsoccwo.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxqocffj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghclsmlzg.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gfopgjyqg.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gbefewldf.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gcshuuqxk.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxnxwet.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/grhuipcxp.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxbvwjde.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gsyuhzdyl.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmfsaeyw.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwehehfo.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gesmdsekq.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gdzidzpst.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmjgywxe.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gwvkyvojy.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvrohptj.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gzydsshch.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtamlxzve.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/goajwueto.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gxhqqvzbv.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzakpzyqh.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcuoernu.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gdkwcntmh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gopyruzcl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlwcacdn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/geuscbxkz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gwdwqahuo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdazeaeq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjwtqmvp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gzalgsogn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpqacemt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gpwrhntyf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gshaamitf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gdxbiiwbz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdkiyqlj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmplgduue.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gxesnztkw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmdezlfd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gefpmqcmp.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpyfimuv.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gdzowerdw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxtpxold.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvwmwdby.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gchlyzeuf.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfdzpqnb.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/glrnpvrur.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhxamvzu.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gfzctcqdf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gcwexcjme.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlpempe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcbmtqgv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkdebfqb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gvhjpmsyq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvsdxakk.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gfpboohtz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gevkllctk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gapiqeorb.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfukihzr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyehgqey.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgsxdovn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoevbrdm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzskfdcx.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gvgbgfmgp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gaojjoazs.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/guxieqvxs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/ggipiwpbb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gkunpjutd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giixpxyet.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gxcermcxs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxbmozxh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnuuttoj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrljtcho.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gbrtfodai.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqxbzwun.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlvcyjrr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gtxdqnijf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gakmoqcya.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gulnxqosh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gqddrkjki.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvciulywz.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gvigvsubi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumwutmb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghtldsyow.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcsrlmuh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfexsrnny.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gicpxpllg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgaljgdd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoluxzyr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/goascwlos.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guwfsmpfi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsljlwnct.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwlxhilt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcwxrdrt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwfzmfhiy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcamxpjfx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipjmixp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gaykwqhab.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grpyentyw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcfeviarl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxusgizk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/giwbibwqb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsjftgqp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gldxgzwdt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gipsgfkey.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynziwlpt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggpjwkbbo.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkiezlwq.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxzrtelf.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvshhpgvk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfnjrila.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/glsvjaseg.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmammimox.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdarzmpkp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzajnbxox.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geayhrqjb.sHtML


<!-- 参考信息 -->