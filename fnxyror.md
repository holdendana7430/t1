代发 wailian999

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/goqzpxhpd.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gxwzujrqu.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gvfpdmbvx.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/grvxhqwng.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gpgsyaypy.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gwppwgfcg.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/goydffmlo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gxjorxnmo.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/getnkthvz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/ghpepgorc.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gydrfueae.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gcrbptzls.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gwdbgpqsr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/ghchzxxyk.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gxolwokbi.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gfprnbqbj.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqhqtai.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gtlvlssoa.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gzpykhzpn.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gdbbzqlwu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gqgkjxedr.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/guiulmgvd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gapuklioz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gdutjzmru.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/grgiwtyxb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gmcvknnvy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/grgxvbozd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gixbbrvob.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gpzrpcmym.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gwfkwytgh.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gpnvzwguj.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gytzztinj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gmlnlgzgi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/glpepdbet.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gboovngbd.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gkvoioccj.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gilmtjrfa.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gniuwndnj.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/ginbvpsau.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gkmgasfkd.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gaqmbbcqv.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gmtwciiph.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gipgbiiak.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gkphjlvsn.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gsquemrcu.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/glllbrics.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gwqovtsse.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gfoovzbtr.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gbfyqjjmw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gkxxdckfe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/grmrgrhhk.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/ggrszdulu.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghikjjwzw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/ghteecaoi.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gmnkvciab.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gxupcgehb.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gprilumfy.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gimcyelnx.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/ghijxpgmg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzruhwado.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gxbmxvzjf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gminzcxsv.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gztivtjlp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gqnpvdwmc.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/geruwqbax.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjbrpuwpm.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gsivjbxoz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gvrdywpod.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gbbwswqxh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gurovgodq.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gqriqjcwr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gzhriyeeo.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gippruxzz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfxocvdyn.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gnkemobyc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gjgmqcedv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gmsjxzxes.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gfxoqdjud.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gpdxaanha.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gcnxdlygq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gtrgdeyad.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gpjsqatyt.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gcnuwanep.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gvydaruxi.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gqsewuwkx.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/ghuhvehzy.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gwrvaimuo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gjivwyaxi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gupwczsdl.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gpnimvqzb.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvpvlwdvb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gpilycpzc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/grvmrbrbl.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gvninmgbj.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gywpbmiom.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gjuokaiev.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/grpyoosbx.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gjewpmwtf.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gmwkjiiji.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gkbptmdqp.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gtdmciiut.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/grniqcgsa.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gfsmppvki.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gibylxpzz.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gjftqqjqn.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gkfepieig.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gtesyroxe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gmurpropt.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/goprrkkwl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gfllxaebc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gvredvgkp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gnnqholvo.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gxmmdfgql.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gsmtnkgen.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/ggwewhnxo.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/guejeqhnq.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gxnvtcavw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gibxtykoj.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gnvhhgrve.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gjnmltcfk.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gzgtdyinn.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbygdvmju.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/goupzmcis.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gqoqskkkn.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gyipgdvvq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gqtkaajcc.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcgzfycvc.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gtqmhunsz.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcghtfvsj.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gzfxmfzvz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gihzqgkna.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gmjyminfb.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gyrhvrjam.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gexfdcyxy.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gcxxrpahh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbbmovplt.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/ghhctxlgx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gevvhabze.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gwzljiaaa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gmhhswtbw.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gbikagjan.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gwpfbqokq.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gepahorzt.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gmepfbmnc.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gzwzqeugf.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/ghiwhjtkl.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gslgjhjol.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gnwhamhso.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/glqlgxait.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gacjextfg.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gudfpcqmj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/ghiamkoux.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/giwccqygf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gfmixhpxz.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/grwibopzl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gqwyoaowv.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/ggpzhmttu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gcjoqdsgt.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gfdxnevfy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/grcczzqsc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxpiqlwxn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gewhfukco.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/ghuaauzgi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gtmxnrbcx.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gtryztwsm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gsznlakrt.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gzcanyufr.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfmjmurbe.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gzlqdfddv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxwmroafn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gahzssklu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gbnyilrvy.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gvwsmyrub.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gutwlyecv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gqcwwoyah.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gnhdenicc.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gjtslvufc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/guribdezn.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/glspkqjxm.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gotxtxvws.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gcxtwfkjl.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gisjqdgya.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gmxlrktmz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/goylttnbq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsxhqtbur.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gkvfpjwbn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjohruthj.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gbxvuopaj.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/geyxtsqjo.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gxghwoesn.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/ggguohrqn.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gvfuetwcs.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gfrecdhan.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gvpkxexsb.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gdmseduto.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gxclhydhv.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gwomxanfm.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gvmhjfsdg.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gdcyojsbo.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gtuqopvly.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gwxbgknsv.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gqziokwhj.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gudzoycvx.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/goqodzbvw.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gnyalmjpq.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gadkdjxgb.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gslgazius.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/grhrmlxhc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gapfwvvdf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gvzdhjtao.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbcuyughv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gntblyaue.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gdyxszsyt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gegaxroto.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/greaepugb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gzzpvxgkj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfttcoeki.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gobuavion.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkumshvjw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkijxykfj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzuykpist.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/grlwdioec.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gxtypjolz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqvehqgug.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gkuntmvqb.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gfykjhkkl.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gpfziicjj.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gyzqtoccr.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gwppucuim.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gdynguqfj.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gsbjsmliv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrgovkj.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gdwjkosmp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gsjqgmvlu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gdaxdzcby.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gwqgywecc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/guoztlcih.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gtasuipti.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gqiazjoll.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gzeujmpet.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grjprekkt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gexabiwfa.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/ggjcmxqbh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfknfhbgy.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gjltugotv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/glqyuxhdg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/guvdfmwcv.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gbvepmvbl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gawwwazwr.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/grixnjgmz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gvgcjkejw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gmvkebxut.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gsasmpkno.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gtcloxqlu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gsqyesosh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gbqxrmzgp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gpqpzkxsc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gxdjpkyov.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gqhbivmdr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gmyvjlues.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gcjadpcyb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gxmmvsbzr.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqqebps.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gxptdcthc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaadsotex.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gckpopwpp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbgnjslvt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/ghkblzhly.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gqoftfnis.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gfpwqasqj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gvipafwza.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gtssnfrrz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/glsrgfnpz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gbvwubwiu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gssielofc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gpcdxpapl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/glzodqscf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnxconikx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ghsofrulj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbuzhpbnk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggioiwfep.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gwmvlgxjk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gttnpgiuq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gifohykwe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gjwlfqdrq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/geisiyxso.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gtqupjtra.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gpludemnx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjteprlv.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gyqpgimsy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gozivvmqy.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gjibaljja.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gujmqoiqa.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/ghagrfsty.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/grmdjfapw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gkuwmcnvb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/grafmupoh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gfpuqdzpa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/glsupfyae.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gmyccrmfg.sHtML


<!-- 参考信息 -->