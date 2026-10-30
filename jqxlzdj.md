代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksjertrg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/glbwbjslr.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gevbiebly.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gpceibbch.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gwwiqkhoe.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gtzepkexq.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gynqfvsuw.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabysoxvv.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gkicfzqbw.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelcnweat.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyaezzcok.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmdcebqu.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfwudgol.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzhnclkk.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gzppuwntu.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjpptnwa.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gufcbuugy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxjlcxbh.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeuzyhly.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjawhjkj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/ggczmvmzr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/guemhbzai.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/ghwbwonbq.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gczbslkii.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gztaftbli.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfszttrx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gjjpkcyru.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqlxfpvh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbxheuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpprylxh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gobnshiwr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/griegjnuv.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gnjdflevs.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrzkuvgq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghshleukm.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gareikbhi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/giwiztgxe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjjqimpf.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxddetmz.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gngaqudqj.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzfyrmaix.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gelwaddub.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmvklakp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpdsksgn.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjibzfvo.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyaxoiqh.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbehfnv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfsvtpcg.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gfddedpmf.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/grqeiuame.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gszvdlqhu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gpiwkxzjc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/grdflntpn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddpjpotl.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/grtgtdeec.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/grksjxnco.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtxjeqtoh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqereuzb.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grnjywlzx.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/glqworkiu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzabiieh.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtixhdenn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqcjrggp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfceconj.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guopzjbiu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gworehnhb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gazgimldr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcentwwke.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ghulfcdpy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtomxdzrk.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqygznwtu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gjypzaxdu.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/guicfqqgw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/ghqruajvw.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmsyjlnw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/grjzaamwd.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gdnljfllp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geauvndzq.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gurxlotxw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gimhsjyjr.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gbcfdpgus.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcshwwag.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghymkzlio.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/grqxpfssj.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmomrfcv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggwpyjvrt.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjyddxce.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gmokmzneu.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gljcdzflw.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gfwbyuhdy.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghqstnyux.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcutpnspa.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gamlqnbcq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gsasucrvs.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaisgbrhv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/giymdnssp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gwirhnzmw.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfwolmph.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gziojdtpu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gjvymeskj.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/ggvrzypqn.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gvgxcfovm.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsslgty.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gxfsnrkxd.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmxxyicv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojzijvv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqkwfvsv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/ggagjzzmn.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gztlofjbr.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxdnhrcl.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxcryelb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gvcztjhcs.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gcwpsrjhr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfcxpghz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjsnmxa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/glqwnvzhe.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznokhrhs.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gahlyzesc.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gderoflwl.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghourcsmk.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdukbocny.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gkqryjugh.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjxdmiaa.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gnslckjyq.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/girfrwteq.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gybelqhub.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggewyxmmv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcohjjit.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcsljvpao.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpgelisq.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwgiaptqj.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcrsohrd.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhomxvqy.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcskjztfy.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glowhmxzg.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gqzlcjkcy.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gagykvbcm.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdgrclq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeahxthr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwuhxjft.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/guiqissgj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmegrwlli.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gujqtwijo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrxczgrm.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfweejfnv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glieobmzm.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvzmhjga.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcezpkjbs.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/ggnlmhvis.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gueoujjip.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsmqyrkn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbhvenw.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gglzfuxoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjecozgeb.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gbzgoiqju.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gieufvrzb.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gflnokkde.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkvwdrdv.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxdsiwleo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gymyhshzq.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtynfsvhk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gdkdvbxrg.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprlzlufr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaapfvvs.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gnmgvfvyi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gmgxdsiiy.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgeekzod.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gurgpwabd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwplusyc.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/ggpqhynes.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsothlqh.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlaxyeme.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjhozhvz.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeyauizi.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnngwtkk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvshfqqm.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gdqujsnhu.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gjmrhfqxn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjzvzfal.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfrmgmun.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gyljtztyf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gojjowyri.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmuedvmh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqddjvahy.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gzgwamxhn.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixkmnyoo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpzfucap.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajujkij.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxgefwrtt.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gbylbrtku.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhksmgrq.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgivllot.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkpdiqrr.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpjvgxkv.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgfxbbza.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/glonwzexf.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjiucylq.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gdwnesyjn.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gymqrpnob.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaugiomo.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/ggryujbum.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gofgikwad.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gnrenycbc.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gyudvvtaa.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gheipyvro.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwfbuesn.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gniifaqlh.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdmsyvpr.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoeipxvx.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gsrfdyjjn.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/ghnixfsrc.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdebncwf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzayqpoa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/grcfdpdsy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/glapqqpbq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gqywnmwmg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gyrubtieb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gywtsopfa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrupklcn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gqdbrcmpx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gofuglmgt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gupzhqbes.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gbwldbefq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoibppjn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtzycwpkl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrjmjwf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpzrkujx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gipsqnzrd.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklhqrivb.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmryuaoxu.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/glppzsdif.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gqznmffbr.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gbpdilqpx.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/grggfbchs.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkhqghqd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gbthqayte.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmvbpwxu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/goyvhluak.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyqeiozh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gbxpniufd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzczrulum.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gteatbfwv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/grmbpebge.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjyneqcy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfysukzbm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/grizunkdz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gcutoflyn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gckkgmmwp.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gedxkvnig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gtatsdkpo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwyhgbw.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gywmjkflv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gevbczwoa.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gglsqlhch.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gofqzelbt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gfvrxxscg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwsooyg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgfsuucg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gcjzbkmbm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gphsdjjzg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghenxcfxz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/glcwarzsj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgvwjnu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjjdujfp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghudtebrx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/geeuwgnua.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/gepyztemk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpzhuqxs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghazcuulj.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gzirpchok.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/giahvbwta.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvltxphcd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gobqbcfhc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmnpomder.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbbdwriro.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gitlaakda.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpulrdzla.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxhsttn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gggugcxkt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grqillhne.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbldwgvbi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guheoydlf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjhjjhbw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbvyukvkj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorogjsij.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gidtuufhf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gakybeieg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdzbrdgi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxcokuncb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfbzzdbio.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gafyhkvci.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggeifjtcg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxdlivnlp.sHtML

A. 基础语法与类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlvudaza.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gttuybkyp.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsxfreje.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsuwyot.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/guisqhrxn.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/grkztqrti.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gkkljovvk.sHtML


<!-- 参考信息 -->