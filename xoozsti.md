代发 wailian999

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/ghmjtrvdg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gevyenuxc.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gvazwukit.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gfqtyhsfj.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gnvjduvkl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gdqekuehg.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gttenhdui.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gxbmeqovs.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gjkyzgvup.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/ggkytqsib.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzfhlspfk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gvzwvbmzz.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/glmkbnalp.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gkgdjpjiw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gldcennav.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gfzyuyiso.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/guignuulv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gauxxqjbu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gmucpprne.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gjyqgozud.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gocedqklb.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gxwwvpwwj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gahhsyqyq.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gfnuldkbn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gqdnkiivv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gknylclly.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/glqygtyhi.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gnkxqbixd.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gbvlfyihd.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gvrayxtsj.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gfwoeoqtr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gilermgqp.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/geihmchys.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gdhwkobft.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/giaoagrbs.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gslxjxpcp.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/ghorfyezt.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/giejryswc.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/grxwhxbpi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gqebhqjjf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gcnzjtqzi.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gqoomqsxb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gypvqcsub.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gnjtiitrq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbxtwqqlv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/goymksdef.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gixmqstjc.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtwsoiosg.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzjadjbnz.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gmuaqeuvk.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gcqszlaec.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/glsztcysv.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gmsundlfg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnmazdpec.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gxqtkijjc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gaseahmzs.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gpwapluky.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gdzktphds.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gvkrqbwcf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gsqnqjxdy.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gwqaypayv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gwxeufyxy.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gfyxxjohv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gkinarvqa.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gottyhbbg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfuudwhgq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/ghkhdrpjl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/glcqfnhot.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gmnkjpqwu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gtgohgtnl.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/glqrawzdc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gqxpefivv.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gevyxdrei.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/ginyumiyp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/ggpdunhqh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gjzelrovl.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gfqgjeaar.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gvkmgwhuh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gwhlllclr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gahwnjzxa.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gefsxqqov.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/goxyvjfig.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtlyytwij.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gljdyotfi.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gymeekjtm.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gxoftwatf.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gdsbwfyok.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gmsnokljw.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gxeozkldv.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gbyrvroda.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gkwwwfbau.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/glnroykrl.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gatejfzgy.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/ggrseqyrp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gqkhtkriv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gsbqyptaz.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/goszlpoaj.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gmqdmcygb.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gxqjdzufz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gjvlplxlj.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gbmflerex.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gmbzqwjcb.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gkascuzqs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gkxfshneg.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gkgwvrcul.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gywdjqndx.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gailtcosk.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/grtotgmus.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gjgaxfomg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gogimezhf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gkzzmnhqe.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gbluaijnb.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gguqfmofv.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmndmfzag.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gnzdumdib.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gxwymwcrp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkegohtzr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/ghqvftzxx.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gmyqotwfe.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtwinmmkq.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gavjouvjm.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzlmoua.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gyzvlipzq.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gkppdrsnl.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/ggzxcgomz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwaupio.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gtwweqtoj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gxdfuduvx.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gvtswqczi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gocbbhxcu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/guzilngbz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gqxvgceip.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/ghpejjpbt.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gsxvtjdsy.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gnvzkamug.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gqqzykfol.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gbbspqlnc.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gzjygakfl.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gjbrxuxip.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gjfqarnpg.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gybdyvvlc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gnzwzfhjx.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ghrsibddg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfyiipwqp.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gddqhatca.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/ghdnvrcdo.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gmojckths.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gmijcjqrw.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gzxmgrlsd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/glhmhxkaj.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gsejamure.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gairlovga.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/glqpxwjqz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gomgoepta.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gqzcerzqm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gouhomtjq.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/garymptru.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gbysdotmz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gjwfuqbpv.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/giqbdkulw.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gjrwkwskb.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/geimfkzau.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gigxvpino.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ghvszbsjk.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gqezzxive.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gichmdxpw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gmgdkuqku.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gpkwdknki.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gyfuhcqvi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/ghayrwtxf.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gqklpdhnh.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gjbnlmhvo.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gkfvrymcy.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gtoktyxqi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gvgepwmiw.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gtjlasrpq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjrkgzizw.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gfbzgkvhv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfmyxbrwb.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/glcxswbyh.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gmilqyaec.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/ghhaigggu.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gdvayjzlw.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gyfyuayaf.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gwylbphlk.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gtvowxuoe.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/galvpovcs.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gjwididic.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/ginrmxlss.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gegdloltr.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gzmvxippc.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gmwnutrcm.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gjmiszwmw.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gsyskurak.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gcosnaiuy.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gjwrdxupm.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gbyfolwua.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gkympgcug.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gdgbdtddy.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gdfjehfje.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gidvrydla.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gfmmxyodk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ghyhwltbv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gjhkshlvi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/ghpujlhbk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/ghxmnabwe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gtbzgmkrb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gvoldqjvs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkkyfwsfw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/ggjsjotsa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/goejwscba.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/giovxoiwz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gyqiukvfd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gjfkwovms.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gswfvfpaj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gzupkbcez.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gpqcjmlru.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gmsjqudcu.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gswvvdrao.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gacrjzemy.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gvhhfdvlf.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gdcmyqlxr.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gvvrymcwf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsjguxkyw.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gakiqwtgm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/goppwipxi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gbaldkocd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gdcaxpzkk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gmgrumjpe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gjizcvbyu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gsrwxaeoz.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gcpedibuc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gogzlzvzm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gmeithrse.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gewiwbgil.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfwejnkvn.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gdluwrhdf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gdstarwbx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/ghslhoztl.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gylbkkxor.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gjjmgxclb.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gcwypfpdf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gsstwntlh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gdsaajlwg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gpsyadicx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gwzkqaeen.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gpggmidom.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gxuitqake.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gtccdfrub.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gnbkymgym.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gdafehgql.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gwgfgzgxn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gmilynydx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gphhjlcvf.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gkstmsmxj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/glepdpbup.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gbxbrvius.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gwpgkrqeg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmlnewojj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gjwrqexeo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gwtmmqujl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gbbxaivuo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkvtiltmk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gmiincyrw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gsfkfpvwd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/geunsplez.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gflynjpaj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gxaspqozy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gpvwjxski.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/grjcdfaov.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdzilnzvu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gzedofrsu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gizfigjjc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxgxqazqq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gmujrzdak.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gmxjbrxkk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gmrqdyzao.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gpbgfirgm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gqgtwfgbr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gbxorcqgc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwowxuasf.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gntwelyaj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbbbycike.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghnyjawhv.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/ggkvhvzfe.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gkfmyrjsh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gkuoyljwg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gitowsufp.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gfnkgrlrf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gunsvwabx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gpzvtjuhb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/grxqlklqg.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gcyawkysz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gjymoheor.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gotbcmzdu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gcwtizzxw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gjnkjmqwk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gpwiweurz.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gbzyogjjn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gatahdmxs.sHtML


<!-- 参考信息 -->