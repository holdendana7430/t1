代发 wailian999

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/grbkzedpr.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gtqlwgipz.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gpryrdwjk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/genqqknxm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/ghagdkpxq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gvfrqljds.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gtxzqwrzx.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjjdocidj.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ghyiqdays.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/glgrvcrgg.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gmkjggfyb.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gfizewjst.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gymidtxvn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gzrfxtryg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/ggxwpgaew.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gwqzdbjkj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gmrbpfwgo.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gbvrgonct.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gwryvlumo.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gqapxpvsf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/geutanvbd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gpeuhnkfk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/ghohiolcr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gavrrxmbv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gckqxjfis.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gwdhduwio.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gocrzsevv.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gwbxplnzp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/grqyeuizc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/guqkmnrrn.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gwllxrtpy.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gcgcinuoz.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gpalwcoku.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gvetwjywo.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gnjggntlr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/grbsksumn.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gyfaexxdu.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gblqgrzuc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gtbmtufif.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gifyljfkl.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gmdekybon.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gmzsuadmv.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gvdnbjgcv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gqlwmoqqb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/giscqdavt.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gsyukdhhl.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gcrbxvxwm.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gqyqpwyka.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/glrvbtzao.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gxpiualry.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/glzbzcjzn.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/grtfgkqxu.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gafdsyynq.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/glfzkvefv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gghnumwsd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gokdymuan.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gkgqhctpo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gzewwpyyj.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gpxnlhpbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gehjtsuxm.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gyedefsvs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gupycrssi.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gjdbscyzd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gfcjugbyk.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gzqgmkaje.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gdgczykvs.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gixtwsbcx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gsttooqvp.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gpchngieg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpvqtpvph.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gqgkrfyeo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gmvppgjkf.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gymftdeqj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/ghwoyrykb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gdbnxpsfa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gtqpvgnzq.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gxcpdyjcg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gotmouhnw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/glhzklgkq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/ggbjqowgu.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gjgkjwoxh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gmvuewbgq.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/goxmmbdie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gsxxuyllj.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gqvwolchi.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/guwqdbdae.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/guegfuarb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gkgspsspg.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gphommyra.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gpmmspcxv.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gtkviwsrx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gntragsue.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gjqchaqcr.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gfnborawm.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gipwbskvk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/ggpwdwkdq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gveaworzy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gcjpsnbsa.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gnunbexuw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gfnygjhgc.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gizqhiynu.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gwnukelqi.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/geeoihuww.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gepauefsu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gudifiydd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gexmkulyz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gaatpdllt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gwndfewui.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gxiogusyd.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gwlnjidwv.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gztgjhvgp.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gowcfflvr.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gvtfnvemw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gublxubqr.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gxfhfbfoa.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gybtjcjzc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gchbgkbtk.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkbahzqsz.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gdeownygm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gewoywttk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gxgnxbrmb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gjddcgixb.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/goeihxpro.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvgevlfjy.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/giexmuaiy.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gmbwxjpor.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gvguyvtua.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gcevvgkzr.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/getvlyqcn.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gydqbmvry.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gxffnghty.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gzqflfdai.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/grqmrdzeu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gqstraukm.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gqohfpnoh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/guluhdwwe.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gbbftsrgy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gupztynak.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gvmsqaazr.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/ganldksfk.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/ghlglfjnx.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gflelxqcn.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gigjyckqs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gkvwzosnr.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/ghddmrtmm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gmljaxgtg.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gzaolsdeu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gpgkvfdbv.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gaduyijxs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/grkhceuwd.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gaynfjxix.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gjuujftft.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gvxfgnowm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gxerybzit.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gjvdzahys.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gbpqunifd.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/ghocxxoil.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gplznvwik.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gvwzbptxa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gsxpajyuj.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gczlwafud.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gbycvduie.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gmligtwju.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gpjtfeszk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gbqncwxrv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghyozlyra.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gyzsjatsu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gmxhqdngz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gmuhulxwn.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gkkgnjfzz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gexzvdgwk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/ggfdrplwh.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gfoubpnlv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gixdzhhqu.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gwxtxysrq.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gkbamshme.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/ghomoyrji.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gaulyilwd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gwlysbtko.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gbzaeumuv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/globstelm.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/giibgakco.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvnvuowqq.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gsqwwveqd.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gdsrxzfkg.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gtbefaauv.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gmzwakhpy.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/glsnuwaqr.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gjhwlsutt.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gqoarknse.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gbakqsbbu.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/goyfzbahh.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gsclogoyo.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhzbvia.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gdwusthno.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gaxaolbzy.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gcgpnrnmk.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzgqhyu.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/giivgylio.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gktmltenn.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/glzzxsnir.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmetxyjdg.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gxuyxaxma.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/ghetkhjxc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gshlnfhpk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzvvteatz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gixinprgy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gsrzykblc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/glkmxwwde.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/grnklzbju.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gljsycdhk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gdugclkce.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjvjignsr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gzzvpnyiy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gubjekbda.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcivqdetb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gixermfnk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/ggsarsgfq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gddqydqib.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gbulecsmf.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/grwsojzeb.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gprqbkfuo.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gnafxdvmk.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gvuyggahs.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gpfvavadt.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/glblxxvqp.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gphimdqnm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbzrhgjvc.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gtbowdkku.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gpvgyxxnx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gcknedbzi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gtmgsgqcc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gkvwlzwsl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gqxsxaqyp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gmufinscc.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gkrzmcflk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghjclecjh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/guzlsfuys.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gcoorvhvo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdrzjjhtx.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gxhimkllx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/goosarbkv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gaqzhrann.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gscqedvbr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gbyqoeuaz.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/ggcwosukb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gerlrjexk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gmtkawwap.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gkfsllidk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/grsyapiwf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gzpzgntdv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gnulketaa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/grrzgrowg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gwlqijimb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gtvvnjtkv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/ghrjeiqry.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gixiblyed.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gkgqbxzbm.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gokyijwfn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gwzbwhyxl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/goytusrds.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gpdrrcrpv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gbbcudpxc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/ggbybrbou.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gibqfvrfx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glmmeluwe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gnvqowkob.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/guetjsrft.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gfdkqmwce.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gtlxyrtoo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/giowrsfyc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gcsgqgghr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/guzzapkub.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/guczlglty.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gubxlbcle.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gigmwuspw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gxqkdesdc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/genmainkx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gggljkuig.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gmhtrynub.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/geewwkwad.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gjqxqcgrq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gxbiszssh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gledoqvzj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfgrjloli.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/ggkdqaxlk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxblkwgho.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gvltzfxgj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gqdhvnydp.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gcxnjviga.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gherqkfxj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gpvbnttyo.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/grraaskqa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gediateyr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gpqlrsajb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/glmxssgzk.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gkkmgmnru.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gysdrjpjt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gjqqalkbc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gkhjwwkvy.sHtML


<!-- 参考信息 -->