代发 wailian999

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gfatlbqgr.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gvjvfkouk.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gxfzmxjtv.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gjlvhrhgw.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gozkdzvfj.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gbgivmeps.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/giekkfyci.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gitqdqvve.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/guwjpfcmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gjdmxuflm.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gomgupstx.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gbncrxyed.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gognzijbh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gjkncrdbe.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gtsvcfpdz.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gqgdiuars.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gnujvfxxf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gfdvzryiw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gihgyrnro.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gjuuhread.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/glhbdacfp.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gisfayevv.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/ggcaaufkn.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gajqqcuzx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/geqvrnwui.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/glygrurep.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/glgylplgf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/guxmgcaeo.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gisyboqrs.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/guhjyjnme.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gqeljhoup.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqrfrloz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqimcrlco.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gunqweisp.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gbzizpxrr.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gucxudfyb.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gibwtkojr.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gqctlxitd.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gyvtfgvcw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gizhfcfyg.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gmkfyyviu.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gzwymeicw.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gyrcxyrib.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gmmxqbzuc.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/glzhfgexz.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gtjxbaprt.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gsqezhlgb.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/goamyxosy.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gblrceylv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gmtbjwteu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gvkdbgmav.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gphekyafb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gpnwlzgpo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gypgjbuff.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/ghrvtftct.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/giqiutpsb.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gzjzruskm.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gidtjyzzi.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gwuxqtmlw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gsxiewngu.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/grcvtegnw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gfidipnfx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gkjeryjpq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/giwnnsgpv.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/ggmuzwaqb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmxgtuvjy.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gnkdhlvex.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/ghvjhhkzv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gsnqmibsv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gnnqgemri.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/glvwxomdm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gpqgerjva.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gqpqkgaxu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gksrxhner.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gzvbmnxao.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gfdepnlmn.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/guvimauff.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gngbowgzf.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/goqcfmbro.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gtepfeyvq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gyhtlbvrb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/glkewkqvw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gqbzxavta.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gybnmzsgt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gvnyxmebn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gakpwvcns.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gkqcmslpn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gqryloiug.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gqfqcudww.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gnuagrllt.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gikhalhpe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/glngmpxic.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gsgsdgklz.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gwzxqpunl.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gliiajlph.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/ghrrxrtpb.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gwuurfjma.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/glediistd.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gkngmlbsi.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gmzfhyojp.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gjyhsuogq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gtpzecqbk.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gzzhpzisl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gdelpgnpj.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gnewhyuzw.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gqrdqxryt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gwtyxljhe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gavgdjixw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gzdmftgci.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gsexsaiek.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gyrtahpow.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gdlyvufsj.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/grhjywsje.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/ghercojyk.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gzxbavmxq.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gtruxwyvz.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gdhujxlzp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/genoqooss.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gxelxysuz.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gtbeqwpha.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/glsgvfbru.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gxofuzjhx.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gdmpbjqbm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gqyoubhdy.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gyacspoxo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gixwnnjxe.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gylsglmnw.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gstkmduyf.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gcdgdjhuz.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gnbytznix.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwyornxic.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/ghbkulpdu.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gsebxoppi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gsrbrbhnr.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gxigegark.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gifflxhgr.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gobxejyxo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggjpvhwij.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gvjkhxcvn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gphmszfkr.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gseqxtytg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gwjwgdybu.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/ghgtaphgu.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gpzuuvhlb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gmbkvzrkw.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/ggawcnctv.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gnpftwibi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/guhpssgnm.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/ggzuhdiiy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gtqnwptzw.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gqittcvzk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gwpkgjsob.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gburrxegr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gvjgpwcxe.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gosnscxvb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/getakrgpu.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gpexjwoie.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gabdyfwcb.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/grwjuqxdt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gbejdeeuk.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gewnunmvv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/glofacpoy.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gbpbasmvk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gvkpggykl.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gmhnabxkq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gikvjfpsz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/ghlxqokhk.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gsookjmss.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gilauizit.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gaeshfmag.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gtbsmetlc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gltpmzotf.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gizhaigfk.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gpirofiql.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gcjdmsdul.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gniumurer.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gflzoqsna.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gafkiwfuc.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gszanfilz.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gwqwngmxp.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gkworbewz.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gcslndcoz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gylijrzpm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gpzvhmwqm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaxoalrld.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gbzjbfogw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gicsnfoza.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gbhmmnhbm.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gxpubijrc.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/giiqxogge.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gzzzaaqdm.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gesuctwgl.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gnvgupzwn.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gyzajyhrr.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gsurganbr.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfujtxujr.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gmkmpjcgs.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gtbwzaqtc.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gbusvoaxp.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/glktubemr.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gorwdgaok.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gxbuhowyq.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/guihnhuww.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gkdhhrvec.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gydphyott.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gllcldmrr.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gcjbbchas.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/grvukqgkt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gwdlamezj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbmukbtrt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/grhirpjhg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gyxfzmrdv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gozfshspw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gbeahxbso.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/ghimwtnaf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdeesxv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gqnbfufwv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gfzyiirxf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gegvjjisu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grbpngsna.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzhrqeqnn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gkgbnwxoc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gdtixowyd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvxitczpe.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gmojtlmtk.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gcycftheg.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gmdfefhaf.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gbahgnonq.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gxceslfzm.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gopsqkcrh.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/ggywklugj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcjlaxtyg.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gwizyifgk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gzoyiubyx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gcwhushbc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/ggbzeoaia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gciktwbhg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gjtklhvvz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gekmapoux.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gujjviiyr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grmengxjd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gpwcbywhn.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gugypicgt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtmtecbkm.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gmvyvvuql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gslzzyfqz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gejzuqhnb.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/ggcbegrxt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gxzblcdum.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gozdbxtxn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/ggxzfxhdy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/goqhpgiam.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/ghezqyroq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gwdznqslx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gwlkgemmd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwltzhl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gqkgcqnnh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gmoovpjtc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gahsizqmt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gwvwjlizo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gxgjxbtzb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gexkczbuk.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gqjgrwviw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gstppmrbt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/galjroimi.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gnnpxjsrd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gaehznmql.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/ggvcdcgjp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gnmqjxiwk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/ghjesemey.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gqqmckvfz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gcwkpczar.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gqpxqibnd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbbnbrvim.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gynnedkbk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gvujkguwj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gfxltcevo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gxxzszbbb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/grvoosmdj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gavqzlywj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/ganuhwrpn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gtgdldwug.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gxufnuimo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gbfxgefkw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwgjirapd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gtjwiclrk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gyshxxtjb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gybsbmvnk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfhqyzlmu.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/glawmdjji.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/getitrfea.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gqqtfwths.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gqoahguov.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gcefxdrjw.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/glaxweglg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gqgxvcvtw.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gqilhjhvh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gqscmgobr.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gsarifdgm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gyxzxcrkf.sHtML


<!-- 参考信息 -->