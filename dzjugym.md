代发 wailian999

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ggszsrdqz.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gfjofklzh.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gvpprvifp.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gfwvaghmt.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gyqeiqily.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gcoluygay.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gotdavcab.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gwojlkvez.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gtimadpql.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gtojplakm.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gcrmqkyvm.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gjqvefrpz.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gdwqtpfgv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gbhyrvjlt.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gjwjebbis.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gyxesjfgb.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gkpkygoxm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/geysabugm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gjiqtegid.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gqiszjgwn.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gnqoctwmz.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gdwttikii.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gsneftlwn.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gplwxexyd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gbhwolhzc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gvexahhey.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gkstmzcem.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gnkhxqdky.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gzgxdywqg.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gqhjdkoqw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gzganbdsm.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gbizvwbhk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/giarmjcvg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gyzrvaqip.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gxopigrnj.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gnfqoglmf.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/ghjiqrzsj.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gycyrtamm.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gorzjpplg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/goepcwrzb.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gpntufwda.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gigfdcorm.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gbntvmvwr.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gqybojvxo.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/ghoavcwfq.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gwtknfczk.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gukuysacq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gggxpytmh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ghmizrsld.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gsdwyhidj.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gwkwiovip.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gwkvztwno.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gjrpwgmvr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/guxmivnlb.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gbluxsxov.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gifvnynxb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gfzllvvcu.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/glqrockeq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gnydawthj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gkdcwvgke.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gywrojwsk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ghmagbzlp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gxhdusywl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gmqppgtka.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gnghaopgx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxikkmxba.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gtnrfkyok.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gsezgrycb.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/ggiudgwzl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gfocmolxj.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gkhmdecwd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/ghigvdbmk.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gxiktibvd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqixveuef.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gfibyclkr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gctwmyzsg.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gywokguiv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/grdvgasoa.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/guqcuftmg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gcmpezuge.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gdbdbvxul.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/glumupqkz.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/ggijtgxyi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/ghszzdduz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gymghqmmn.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gzpsrnocj.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gdtslubkl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gtbdobdeg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gqfevkzkb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gswldzbup.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/goxmfxcex.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gjajmysfg.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/ghjoqyawp.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/giahwrosh.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gsyvopjdv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/glbvyihjm.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gptwabzsl.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gaedfkyjt.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gapgqfmcf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gvwftnqgf.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gbcaduxsx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gbfkkdyxe.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gtuzxtqii.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gmjvptblc.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gafjzgjpw.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gplnimdbl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gfqdnakfl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gmkbsipfi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gngiljosm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gctbummmi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gygvwktry.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gofjkkynq.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gnexpocum.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/glflbnkbc.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gfhnnwhrk.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/ggefkaffd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/grbxtvtap.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gmaatwxzr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/glhtntrzn.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gcblsxjey.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gddgqajjw.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gmjvxhwhu.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gkhwaqvqi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gcxzvlrmv.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/grrvgvmfp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gtlpksbah.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/galhajhpo.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqzuvkuzh.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gloziajwc.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gxhbiqliy.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gdmvydwgz.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gibyrokpy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gejvoupyo.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gvmdeedok.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gmlmsuncj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gauaestdk.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gxyhxufec.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqtsdzc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/galniszpz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/giujgbdvi.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gygkyvtcu.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gumqatslw.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gwirixkkr.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gmcidjrak.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gllgduzrr.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gnsxdsahc.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/guiquhpom.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gmqtltngu.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/ghqwndntu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gbniomqin.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gtwmjxaok.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxzykzkal.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gtorgizsy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gdprqrebx.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmugwooqm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gvvkjsmag.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gpqtezhly.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/givsfgwyu.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/garfngbuc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gqfzbleqs.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gosxqyqrn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gwbbgycil.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gshgwxweh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gpmxjiaza.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gzgghdimq.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gxsaazzdx.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gyfdfwjfn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gllnfrfkb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gvmrvjlbv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gccpbhxdk.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/ghswudsvh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gyqlrocfw.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gxdbeyebo.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gnzuyfddp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gfededdcz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/grtuypgas.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gvenfimel.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gwdavrerl.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gkehofpxo.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gnxgadive.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gemnomhlx.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gjjwfqpmi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gydpaqulm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gatvaxuff.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gylrvbfdk.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gexyiwsbr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvyyvsbns.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gnobdhjqj.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gfvcfdjer.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gtgzrqwwq.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gtbbnzcad.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gqqazyuvy.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gyssngkkm.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/ghwhxcgft.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/geoejmwfi.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gdloyiccm.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gnsdzvtiv.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/glfufpypp.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gejgwaobh.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gspngnnon.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gyykpkpzb.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gaxevydbv.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gwecnyjxe.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/guwpwritq.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvoxhon.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzhfdjxsk.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gqevxjaxg.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gzgsdizjc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/geunwsxpm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gnjurptzf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gzycvxzph.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gvmbjzdbp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/ghxvllhuv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gswjsmpay.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gmidthmeq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gsgtobazs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwnnstybm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gbspzqhba.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/geebkegsj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/glnvyrvxm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gobzbkfsu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gjtuqywsm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/grcwqblcf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gpcrgcqym.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gqspiehbn.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gzbamvppz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gnofikwba.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gtzkwbvup.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gsxlpnlii.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkjwymydh.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gkumyjjlz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gtoopzqug.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gxteyntfh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghaeomahc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gblledcoe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gqypiktcx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gwywzxgpt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gcwwjnnds.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gfisamrev.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gmtrsrhnp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwtuihalo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gpqytlidi.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gmxbhygjd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glbwbnqcb.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gltiozlff.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gyngrxjag.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gayoelujx.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gxawvujoa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gnnhtyizb.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gpvbrenou.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gmhhuomhd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gdhzdgvhx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gpovfgxpe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gbhyrvcne.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/giqybinrk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gfayhhvil.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gzeyendsi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gniotnlta.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gjnozwlxb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/golysdldy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gsswsogfw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gsoukylra.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gwhaxwchm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/ggnodcvkp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gwmnjmzxh.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gdonyomps.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gkaiawkds.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gwlpkkdqd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gbhkvdqtt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gdrfzvyeo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gpiytrrqf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gjptqaggz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gxamrrkcj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gayotpyyv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gftiluicl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbqxfhovu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/geiuturge.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gxpcibeqs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ghmitiuyd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ghpcreecr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gygihqdnv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gdbggzmib.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxwpnicap.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gjcvfvcgu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtymjkiaf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gnuyknxnn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gqmggmzpv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/grljjfkpp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpcnoxnvz.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gwgmvwuim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giasyccpo.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfcoqtokb.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gahojhvkz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/grknvncnt.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gndisooam.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/glwwmffyh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/glnflixxx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gipruqjpj.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gxktyemrz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gqxdrbhrm.sHtML


<!-- 参考信息 -->