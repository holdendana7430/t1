代发 wailian999

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gzqjagigv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/ghjwnpwsj.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gizfhwgmg.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gglsozhct.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gbmjmnfmi.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gnzskoscl.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gfpuyybny.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gmkejkrwi.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gazbmlojp.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gmileshnk.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gedtrqkcs.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/geubnpmag.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gwnbneeeq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/grzpbrfie.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/ggqmzuwur.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/geeivpftn.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gllmostbg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gcrhkaofr.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gkvgsmcfy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gnsmhjfty.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gcqqbejjv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrprmga.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gnbinbkrb.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gwolsrieg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/goctohgpd.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gdddgzfav.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gqwpwfmbe.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ggokumwag.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gsauvszrr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gvqoqokcd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gjbeictlb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/ghhebrdbc.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gpmxkgndz.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gaytzajsm.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/givbrdxrp.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gqjhlyvwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gllrnchvh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gegiaduhf.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gwtsinvxi.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gibjdyzqe.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gkxvvlvoi.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gvcsnqjat.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gywribkni.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gpmuqkskm.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gitbgydip.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gbrjcqkdh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gasincnkq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gkyyrojqe.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gbivjydag.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/grltpxrzd.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gxojszsvn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gifthezle.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gyhibaqsd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gpwclnygr.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/giacgbcmd.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gzsytplhp.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grzutgbhq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gwbiucjlb.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gyeqyumfl.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gqcdvtwwa.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gdnvgzxuo.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gpgpzmotq.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gzmpxydqz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gjppbcwop.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gntzzcnwb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gageyjbvu.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/giyqcqkvz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gvqlykswj.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gdjxljivv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gibioxbhh.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gkqhpeawu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqgkyks.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/geaeprhej.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/ggzjggoif.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gennkyuxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gyovwyasw.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/grwlsgufe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gdlluqmuf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/guwosiwkp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/ghbevwbgo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gpdpmvato.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gjzphvfnu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gatxwjwhu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gjorhvxmr.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gvqgzntzs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gpzgpkrov.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/glvmbkbgv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gpvfldjpy.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gszkqttbc.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gwyxhjzsx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gymxrtcde.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gpctdqtqn.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gdupyqqcg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gmkwwgovi.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gteulqnuv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gxkgbqgzk.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gysiqebmx.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gixwzrrcx.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/godxxseou.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gprfvgkcv.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ggpglbryr.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/ggjogtwag.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gwvawhlgo.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gcdzirfin.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/ggvzzoeak.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gahtsnmqf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gymiubtwi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/goijhsexz.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gzxypgaub.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gsblhfgju.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gbwkaitkd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gvcjfacwp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gojmdzjrh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gjfgmjthd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gmcprskki.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gxgeajmcl.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/glqqutnuo.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gyfhhytas.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gdkfzbnry.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gswmjcarr.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gokhyvhlz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gjzatmjcz.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/ghicjiebc.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gmkuqoeop.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/genvbufnk.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gcvkaqttz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gioclzxrd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gvtiopfok.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gxwpapfon.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gjmywggml.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gcbnugrfw.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/goikdmdsv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/glfswbsnb.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gaickdzwd.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gqilvfuwy.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gxexaefzr.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/ggfrdtuxa.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/ghzxrukwu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gteveztjx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gvzgajzzc.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/glowikfux.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gmhzpbrcp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gotqdxwli.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwgupaw.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gwmcfrkfi.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gdztbghkl.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gngtihlbs.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gfzxednrj.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gniouuwvy.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/glxsdnvex.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/ghquutola.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/grflejluc.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gdantcvqz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gwxuyrskt.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gxnifmnqy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtctavhbe.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/ghhidppyc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/grugwavpn.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxuslbyjt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gzcwinzbx.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/glrfpvijl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gxckppvll.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gncrrnpam.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/glnykxxwd.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gtkjnmxwl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ggslwifpk.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gdiwebwjr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gkaywqrth.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gunaavfqy.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gzkyofoxk.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gnyxkwtbc.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gulcfxkjm.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/goumhwjif.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbggnbbhy.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/grrodryep.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gdjfgbxbb.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gwhxzfnpb.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/grtzhtzsa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gjhylpiwi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvtvlkfqv.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gqmuuktcn.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gnamcifrd.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gughtvoxw.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gnysgcvtu.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gmutsproq.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gwcayihdv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gbjrzjbla.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gdieulepe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdpxoryaf.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gnotkxuro.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gummorokz.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gcjcgcpir.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gkevqbrvg.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gruddgyqy.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/guqlhulvj.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ggotdocxb.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gzxcyhtmf.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gathsqqxq.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gysdommga.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gshjpiasx.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gpfrtirlu.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gtsqqfeat.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gngplcghu.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gwkiokedb.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gjtspewhz.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gmmhwavhv.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gubhrrkol.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gfrhdkvra.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gpdgcjmsv.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/ghzatwhpu.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gidszyiib.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gvauprbxw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gyfzhrfcn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gkmjodytx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gjsjxbvvj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gavfproki.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gahouxtbv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gfnrawyuj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gzrfuanti.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/ghlupdsyk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcijchaek.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gswmqvcyd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvfvyeohd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghlhzumwx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/guvzgukiz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/ggnriiukr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/glfsdcuwg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqebfrolw.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gwibddwdv.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gwwajzygd.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gtrghjges.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/giddpqqzq.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gknjinrsu.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/ghpmnipsi.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gxmeewqrx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gtnobnkmc.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gkwyitjim.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gunoiqipr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gqjolcpoc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gtwctwihu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gprpfcqxh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gketygvic.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gyaipwfaq.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gtgiviojz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnshuawgg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gyihwhsrr.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gmkabfodz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvyotzxnq.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gvcsezvmn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gcnbtguso.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gdgibtvai.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gfmugcltd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gyxnwiauo.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/ggkgqajdh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gpkhwbjvt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/godnqbdtx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gmjmfyabs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/ggzwoxmbw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gixxcqyld.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gdywefxbe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gzmodooej.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gvhvxsfxb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gpuhnlzcr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/grylqzcwz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gvvcaaomw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gmrmfzytn.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gjbadusxq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/ggrspyhxv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ggwpfbikw.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/ghbqgpkdn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/geagjepmd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gkwtidwko.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gqudqbzyx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnlcynoov.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gvycxakrs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gbhllvjlc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gkollzjiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfvccaiat.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/ghdgytocm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjhfdgybb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gfuvgjbia.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmifiwbrh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gaiarxrfp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gmpprzfca.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gwanbwqxa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gtysuwqke.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gbxqpwomx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/guwvneusz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gwsaumiro.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gmghjqxcl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gybmwqrfg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gztnmsnsq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpbyomxrc.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gtmjdqtpb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsnovrcuu.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyeejerrj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gkimljpat.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gejsmslex.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gytotkapa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/ggqyqxwwd.sHtML


<!-- 参考信息 -->