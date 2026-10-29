代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gciojfjks.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gviwuuymp.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/geergidax.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/grfclgpfd.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gdzurjhnt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/ghhtwzzga.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gltsertmn.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gsvtrwucx.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gcnxgtxpz.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gvaokocmo.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gyejiquhs.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gtnskoydv.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gjatuaxxg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gguovivxh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gqqpvghya.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gpingdwly.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/geobkfben.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gtqrrcdkk.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gbhvkuvzu.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gcxwanbxm.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/ggewzlwwb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gdgefsxqa.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gefjskxxz.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gqriaywgn.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gfwnzgyei.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gvqzchuvz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gjipxerye.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gpxcsqsnk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gvgkjdock.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gmqipyrpl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/ghltrxpvo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gekvcabzm.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/grkgxnqub.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gzolsqgdr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/giksgucdd.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gtysitqkl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gchqpariu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaycbrryo.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gbgogiieu.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/guobelqsq.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/guqpuldtv.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gkecxaodb.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gfalnyevl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/guthhfsob.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gnaoddvci.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gbvhjsmzk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gcpjbdsix.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/genrqnlns.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gojlnoiog.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/ghepkvtvl.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gkxjcslzs.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gsatuzqga.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gctfnwupn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/groawqqhm.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gcunxspsp.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/guwkzhgay.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gaydgnbta.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gjttflkqo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gqkirdigm.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gmsegapvp.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gshoqjkaw.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gnjbemeyk.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gphqvhgzb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gctbswszj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/genyrnpyw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfsahtpsv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gpchhklpi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gfvpdvcad.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/ggyoiqkvd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gtvdyutqw.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gzbicyuob.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gupwaawzc.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gftttupep.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gwmzlpsue.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gihnjsunp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gxzrjxrhv.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gumrhaxkk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gclsaojfb.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gzoqrtetr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gddkauijf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gggfrzinn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gkcgacbka.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/ggvcpwplz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gaolovpke.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gklcnuwrn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/geppbgwfs.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gmjeuzelg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gwrczhfko.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gaafyaahq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/ghndzmfqp.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gulbtfnuu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/guxvdomiz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/godjagagw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/ggnzmhpcq.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gqlhtqitz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gflstntgm.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gucbpzyto.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gsnuhyrij.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/garccnkns.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gphiukean.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gpaymhnez.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gwvbflduu.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/grqlgdnlh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gcbfoxrqq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/govxewjng.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gjuylwrlt.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/glhtemhiw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gdrrggxlb.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gzslxzstp.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/grcmrjroq.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gcywbqixr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/glceoctou.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/geowjcflm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gtysuoaoa.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gpjwsghsf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/grvqkrrsw.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gwraifmeg.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gxzjudxyg.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gaeuxjlny.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gydsnqfuc.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/guvjbczql.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gscgrvofl.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/ggqpmbdpf.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/ghyqqjijr.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/getobjunc.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gqdflgjfr.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gmroeebor.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gguhzcwqd.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/grbmfqtpa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gvndtiyzb.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/grmjwmlgo.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gprglltzj.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gobfdhohi.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gperceghf.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/ghhodbfkh.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gtqllhfca.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gcibxzgzq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gbkuyzhsm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gglspfncu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwiimilvi.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gaancvfyi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gqhtctxgw.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gkkczbbfq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gvetxhgeb.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gzftyhdxd.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/geylarzzc.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gbajnsaat.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/ghdeytyqr.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gzkkptgpy.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gairgzpzi.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gqojzcgzh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gicgiaygo.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gfyyixrxs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gtbcbhpvy.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gifgkqitd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gfsfmlvbd.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gcviilmzf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gunvtmsoi.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdexyjb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gbpqshjaq.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gfslygxmw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/glfpyaruz.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gbkeinakd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gslmpbrng.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/ggwaeyogw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gmpwtvzjg.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/glbjnjanw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gagciikma.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/ggvlfdeto.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvkpjlqhw.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gagigfqtk.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gotpntfic.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gppvexcvo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyjpoyrkt.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gucwcsskq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ghazdftfr.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gwnbtqfbh.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gaxowvdck.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gigjnioyx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/ggdvlppka.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gyuwaoosr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/glbvvwcmo.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gdghwuznr.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gvhauxjrj.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/ghsbalpea.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/goggqhnmx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gnnclzrwe.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gsyfvkdbc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwlkgmwer.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gjlhtuboq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxmxnapqd.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gjrynwmkw.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/glojqkjds.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/glzwsheoc.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gmyunmjht.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gozribbie.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ghsuvgebz.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gtcwbcjbe.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gdlkezpru.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gmmczjovo.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gfbdqdagn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gylpwbwly.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gxuidvvkc.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gmpdnayts.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/ghpaknkdt.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gmounroyq.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gelylhjyu.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gzvhkiwex.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gatvemuzc.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxnuagcfd.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gzyxduqdb.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gfhsinquh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/guqzygcac.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gvcyhqexg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gdxwgrqmp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gsbinzday.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/ggygkdksk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gyxtkdnnj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gqnsqdxwm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gdclolqeu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gnywzdgwv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gxsvwvkgm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/glpfaabyq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gaggtvdjn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gnnbfizhx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gllqjzerv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gnydbltvt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqrizbvda.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ghwjlqkyf.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gdvddumng.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/ggvmnsfbn.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gzmtwbiqq.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gvrohnrlf.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzjfgofoa.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/geqlclrws.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gejqwhyxy.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/grdjmiwal.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtrvzbnyr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gbxwnfthg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gkaohzpaa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gwevksrkk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gzncrfuxu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gpziwsrxl.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/glmzhvzoo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzgxtwvrn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gwholmsxz.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/guirkgfnx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkueyjcup.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gkvkjzkde.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gagscbunj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gglgqrkyc.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gafbvksnq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gdmuelang.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/ghvgwbxic.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/goehgnwoo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/grqogfvbo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gqxkqevew.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gorirsyjp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gxjitgfie.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gelzvyatn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gcawkvyty.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gljayutri.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gbpxiivxr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gpjfpwqtk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gdvkpchla.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gndmzndso.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gfpzgfwiy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gmbbzjxse.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gegfvodir.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gniiszlgx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gbtmxruvh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gnfxvijrb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gbvyrvvhw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gqyjiomda.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gmjmecklg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/guxddngah.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gxugotkar.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grlbaaumn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/grsfcwdls.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpzkastdf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkrwrcouj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ggrwmdkle.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gsdesgvfz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwjlfofhp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gdtrhqatn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gjzxmjglv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gckznrtko.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/girffhowy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gdrcvnqzk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gbzaytdgc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/ghpergddb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbjjdrdog.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaidgciic.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gohyypgfp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcxeldrro.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gdciblfhg.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gmkmikgsk.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gxhbohwnq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gjhrgneti.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/glpnishma.sHtML


<!-- 参考信息 -->