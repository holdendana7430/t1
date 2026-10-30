代发 wailian999

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gxlibmska.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gjknrhnnp.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gnpncbqxj.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gpzjqzxmv.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/ghckbifsl.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gewraksax.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/ghytraxag.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gsenfrdha.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gidzrnqlu.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gmrgidkgn.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gxdunsedw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gorbltpuv.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/ghpaeqwvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gjvipcmpy.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/goqudjhzx.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gvukcvauc.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gifknnxdr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gnzbvdiuh.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gddsrtrsi.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gzkldqefp.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gradormuu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gqchupzvv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gquwqhtms.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gyueyvrig.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gzctawxug.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/glxtmvzgt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gsldodxch.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmwyxuuvh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gqjoeoqzz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gwpjmfxoq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gkrhcxafy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlmmyxr.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gbfpgfcak.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gxufuxacd.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwpnafdwp.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gkebwravo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gjjipxmbr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtrwcqxft.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gpajfhupq.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/giigdzmud.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gsbklklzp.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/glfahtchy.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gesumuyln.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gdcgxkibq.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gqyussazc.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gxsgvcrjg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gdrhynbyk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gptmxarau.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnnsmjc.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/grfpvppmf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gdlzqgfvh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gsqpibytd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gtpmoxplu.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gtvicdwcm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gnjzvsxyw.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gvmaaoxqj.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gkvtdhree.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gwekeqfmp.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/grjfewtbh.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gbilfberq.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghsnemtoe.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/goezaagjv.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gudlmfbvb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gosrvrouw.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gemwnnsvh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/godaffixz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/glaiguazr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gygsopegm.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/ghotcophm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gxltozqok.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/govblyqdp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gqeduqtum.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gwvzbyhxu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gggcrfbro.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gxctxbijy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/ghvldotnv.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/glzimrnvj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gtrdtyfii.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gkhbzdcxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gdhyjqona.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/ggzmwkiyt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/ghoiimqgg.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gqccxfsld.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gwtgrzoka.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/ggjdwbkot.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gtamvwhpe.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/grybeosdo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gbnbrczos.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gbsavawrn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gngxcbeca.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gyuymodzo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gtwsurqji.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/ggyhxdfbi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gxsfsmwco.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvwhetvow.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/ggegtfigo.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gfqzophnd.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gmsrrhfcd.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/grvjbbqvo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gbodpguzs.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gilvjbkvj.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gjhbahwdd.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gkmkenuxp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gihltcjus.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gytaxoovb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gkioyocen.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/garpwfzwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/golhefllw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gbqrvbtjs.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gviruysid.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gillbsbjy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gdtodzxiw.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gjjlthoig.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gwgptchvp.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gogclhmow.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/grdjvoxss.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gujlzdufq.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gsejopiou.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/ganjaprwc.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gtopudcfd.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gpvkwgiwf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gsgfecxqr.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/giyiufugk.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gjlnyqksn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gippscvlb.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/goiyfxssr.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gdghnwjbu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdxzivhfs.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gdufsryob.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gudkcahme.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gcmxufnja.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gifphgyzk.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gwxbwijzv.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gsqbmadci.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gjearjbby.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gzxdnpcem.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gpujvftox.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gdahqqhkv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gkmnmtbdn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gtotdaxoc.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/goktweake.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkmlfsfaq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/glfagmuby.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gdhpdvfod.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gwzrjmyyl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gyohjdjam.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gahbcgsbm.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gfikhysbc.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/ghetehkyj.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gjxxjlwpu.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/genrugewi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/ghezwexmp.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/ghjfnqbio.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gbwfgywxm.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/ghypwieaj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gsqrcxewc.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gjkbdlpjo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gfmtiyyrl.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gqqxjeein.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gevsqdoby.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbenvarev.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gssrixcde.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gegtwmznb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gzsraocxk.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/giulkxhig.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gymvtkixa.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gssifpfih.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gueklxqul.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gzumpqmbs.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gwnnexmnl.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gixrdrjle.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gznhgwyni.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gowaycnzk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/goufyrtiv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/glarssmhp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gkmmsvjxv.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gyjaulrqi.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/glxyxugyd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gdvggmehc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gykpdbqnu.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gsmwwgfgu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/grltkmqpa.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gqmqkovky.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gqmjgsukv.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/ggraixacn.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gfjghahgf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gmyxkwsan.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gmbcerztl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbsvyazqu.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gfnusjzcn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxidtlchp.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/ggdsoinyz.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gmffgirmz.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gckkgwdhu.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gozaszwhr.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gshmksybl.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gikgoojiw.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ggzgnhkvf.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gkdqlopmx.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/ghernsyjd.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gtraqptzf.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gmnzzqxdt.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gdfqrjiyq.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/ghfuatqfr.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gmforqlhm.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/guivfxvwo.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gwgjoadwa.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gdwbcnxkl.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/ghrfqjdnw.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ggmaabgys.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gzspvxkjq.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/ghqootfui.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gcgrjbbee.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gottixnbd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ginwaadml.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gpahokhps.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gkpzsxpho.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gqxolwwni.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gpnqreypd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gpqbxofin.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdusbeqhc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gjqupgatj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gtztsyzpm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjvtgszbl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdhlmumpc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gazxtotqp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gtrsaqpsu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggtuslowg.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gzdwtfvpp.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gnwectnkv.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gvcdvvcrq.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gkoupadfv.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gehcdhlzc.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdipqrnbl.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gjmahilmj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/guccexlma.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gzskqqnzk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwesjomci.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gdrrucwrs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/ghcncpqhj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gyvtwsyst.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gocqvthxy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/ggklcaksg.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gxeysjbvu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geiywmygk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gplxkrvgd.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gstixkzln.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmgwyhty.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gaaxijvuq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/ggstxbbss.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gbmlwwaed.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gshuvujzz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gqkirarke.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gxiiqiqjo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gvppwsume.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gwvcdfuie.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gkgworkay.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gkzekwgvl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gejxcqkgk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gzbdosoym.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gnkebaycq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gbfyiakcs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gednvczwj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gpyvzqakz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gmurkyvij.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gvlklodzb.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gcaclbmuq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gnbscmvoc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gmkttdcuu.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gjqdhpzro.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghzhrakny.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gdhespdow.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gaqleurtz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gcsaecpyf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gncpoirme.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gtdrlfshd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/glkpsjykx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gcuqqeucu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gpvsencrm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gqxvpmljj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gweuvheaf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gtrgxzkmx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjuqplayg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gfqnrdwwi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gyrmzqhxk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gkojsvsaf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gmcwnfjjk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqdinpipw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gnstzmtff.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gsgcjupna.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ghuqltgkm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gwaovhlcx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glfpdkfmq.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/galktjrvp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrfdjgcw.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gzrzztmcv.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gebcsgngr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gtczifzno.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gowlyvbnx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gnzcxfxvp.sHtML


<!-- 参考信息 -->