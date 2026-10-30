代发 wailian999

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gfosrmray.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gygalszkz.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gvvxopbfj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/ghhzwbski.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gkfscjykp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gznrryhrk.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/grdklqgsw.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gzqfpknjc.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/glshtivzr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gaebqimqo.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gmjjrcxno.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gliicvvqy.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gcblwvmdw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gacogixsy.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gyerutbvu.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/ghborejrg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/glrrqsauc.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gjqiakzgk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gfvzccpul.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gmxuzyega.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gkflfwfhx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gsqjxiyrl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gqmekgdvh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gyyggbjrh.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gzivlgszd.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gnqzpovex.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gtluoeenq.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gmmvgzfid.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gnaeheyzu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gbjoerudq.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/grwwksanz.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gughbdmqp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gxixnwzup.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gckbrdtjp.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gqcdyzcga.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gsidkvrmo.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gtaqxscez.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/ggolscgpr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gzwmhiwzl.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gwpjqlrik.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gwhywmkud.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ggmgotitx.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gwsmvojaa.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gpjxlauvf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gtwjkcquy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gpvuftqle.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gvifyuoee.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gjmebboif.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/ggcokyemk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gbbpnwpsx.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gwpayxqpp.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/grbgidmyz.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/groirfumf.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxjtsfvxb.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gwcokfcyl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/ggdcnbmxe.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gihthmrab.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ghiwjmegp.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gbdpvlsuw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gimvweqif.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gakqgdtfq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/givvdmnpf.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gwrcgdbkc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gcndvcdfc.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gbcstctuh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gpzpafkoy.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gujxkrchq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gdaxdndui.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gkcwcvnnu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gycvvqvwj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gtvvnjbvy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gjoroqwxd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gqwhdjbkd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gtsrmirru.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/ggfxrboqw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gljbpcohd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gmfhhfovi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gomxjfoqv.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gxglzzlfw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gbaecnpte.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gpubuzfgn.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gadqjqhui.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gqwabrudg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gpzerhntm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gczbjbarz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gfndthtzg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ghtmnxwjd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gnvzouewn.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gqniyzwrr.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gdtmpprjg.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gnagzqkww.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gzdifvyao.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/ghtcrahdx.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/grfzvmjwp.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/ghpqskijp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gkyjztjim.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gbxhyyelp.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gfjklyurk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gedkdbxbp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gtsurzrxy.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gvrcgkfzf.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gdbhibbaj.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gwyzrcams.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/grciiueeo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gbwejioho.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ghutrjayk.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gbzuymozh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gilkakfwl.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gxxoavflu.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/guiialcoy.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gtrhkelxr.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gcvrcpldn.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gzzjrpweu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gdcodhbnh.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gdmiebjcv.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gvjfjmwhq.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gefyewhlk.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/goglmhkjd.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gbmhomryi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gushcmdtj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gznecxpmv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gyhaqbnxv.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gzenpqkwm.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/govekqnpj.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/glanphviy.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gqttoqytd.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggbuadrwj.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gfvecwtsn.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/glsulxbrh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gwrqliumq.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gdpdamand.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gukmiouzv.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gbmzmojta.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gatoadhoe.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gxyuuxjgy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gftfhkuol.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gqbeymotc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/geohssbdt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gmsrvcstj.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gjspkegzk.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gzdmrsibw.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gbmbzswlf.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gsqtcjdmn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gxcapvbfa.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gwyxpncki.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gnlgeafhc.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/ggaixnngu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ggjvinuxl.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gjokxtetn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gxlsvjpha.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gixxnqnha.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gadkbbfjn.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gkyapqtqq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gfgzwrpys.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gubmlptzq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/guqdnvnkh.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gimpddgmn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gliuolkxr.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gaxdahcuz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gqgjvfusa.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gxgoxaxzp.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gdusyrorq.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/goxfphndu.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gizkkdtpl.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gpmbyyvim.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcanaqdml.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gegwayqse.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gqfnmuvtx.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwisaraue.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gimfjnlgf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gyfslpjaw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gcchdspsy.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gcfbeuaqm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gimrpeqes.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gistrjods.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gualitpzv.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gjnzkcwax.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gjwoptcoq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gctrrflzi.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gewhvhyfj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqihtfkkm.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gejrdgljm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqhqyozuy.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gmhgfbias.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gaxrmcjdg.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/ghusehiur.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gnqzmawdd.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gdbqatugv.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gooedkihx.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/garehvxho.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gnwratbap.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gbbbvjojr.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gejkotjnl.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gfddaaatq.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/goxorelqt.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gzigknicf.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gyfyalqdh.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gcvwkzurp.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gqqfvernk.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/glrmgntqk.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/grtvgqbpj.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gboyhwbph.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gdppvrmyp.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gkamnkrxa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gsiqzcjrf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gqtkdrzqi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gwdbgykaj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gscaziuch.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gemdzluho.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gihpoxnvw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gykzgzskb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/grtgbudei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvqfzseyr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gbfxkzxci.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gxwbztskf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gatnydpck.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gtbfoboai.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gdtxmneto.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/ggholaszl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gubotppqm.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gtbxamoim.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gcglpawcm.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gudcvzxxm.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gcqehdtlo.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gshzracbz.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqyyfgysj.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/grwerynka.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/garjawwym.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gclnaiotb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gazlbcujz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gnmcfnsec.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gudhlakaj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gecdaygwk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gickdkugk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbneyohqy.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gzshxqhxb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfuakwndy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gwklwneyj.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gjaqjxmso.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gugixoosv.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gerbkadyv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gtedgrqsa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gkhthgvtw.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gqdxixyti.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gnhvrvpol.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gjjkykbnw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gmimddesg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gdpqlfifr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gqcdcffby.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gtnjsebvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gkxkeenwn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gmzguicur.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gsyzgvtbj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gneewlvbq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gzadxnfor.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gozgcivlo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gkdpkucrv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/ganghfalp.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gighrqbjt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gotglbseo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdtunnsxv.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gpipezdtu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxlesxtmo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gvezvgooc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gmikzruzh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gxcbzuyiw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gwlozcaqq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/ghmlftguq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gqsprvemt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gvcnxuehd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdreltwow.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/giaaxltaw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gtohjqxof.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpeqixabl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gsysrjpvz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gdxbchtca.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gwhlwnbvn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsgrrkv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gzydnkngh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gkgarfivn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gydlydiib.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gldjpxyno.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/grpyelkkb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbbhqvzwj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glhotobqo.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gqsaorkmn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqrvfzdhd.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfwogio.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gbydoxprh.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gblxbuisq.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gyrtwitwj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gkcvccjms.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gwrkrrfej.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gsiiysijn.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gyfzndykm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gnupuayuf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gimjenyvo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gwfpobreo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gfncdqpsp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/geomqlili.sHtML


<!-- 参考信息 -->