代发 wailian999

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gcfcmnpwp.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gvhbrtunu.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gauksqvmz.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gaujdlvlb.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gpgftfxdz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gxxgurqqx.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gewbekgmb.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/glbwoxkzu.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gcjzfwtpc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gsspwemqj.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gvkykpsnr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/ggfygqnos.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gukebxpic.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gtmhcudru.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gliyzzioz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/ghuvjspox.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gljamtdam.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gbwrbpodx.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gnpzbxxpo.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ggeshczbi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gqzshduml.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gapzvatde.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gprorkbyu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/grhgwqvjl.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gfvoflmlk.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gmduclzhg.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/ggukbqkjn.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gikrxmwvu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gzzychtom.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gquwmoaet.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gxulpeops.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gfqlfzjde.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gexvljxeb.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/grhcrnjjq.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gznrjeuob.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gqaxtmner.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gizvjqevs.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gjeckiriv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gznatonip.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gvxerezql.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gdoxtzhla.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/ggcmboyfw.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gzfwemneb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gpdaeihuc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/ghnjzhhrt.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gbylhvlny.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/ggngoeuph.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gbctlhhgn.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gaddfazjt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/guyftbmlf.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gqtwishfg.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvxmggjmd.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/geootnzlf.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnynwqsuk.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/ghounweub.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gqhudysym.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gdavlpihy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmouvqcyb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gdhhrnioo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/giwhrgner.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gfknbsvvs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/guxjxmcqk.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/giyaywdqu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/ggoiwudsp.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gkmvccwkx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gzgidwjqd.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gapliewmi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gxykbgrew.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gntapknqb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfswlxywf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gslbrpqwv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gfypmrfyj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/ggidgashu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/ghcmxyxpz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gmdjsgrla.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gvxshtmhq.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gmmxwfbir.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gabavjeap.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gxqxpwwvr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gaezxcxmc.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gdjrdlryb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gyeoknqbh.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/grdzsupdx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gvkinyunb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gxjvluypg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gfjysavgf.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/giuhcjjzh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gybwjypny.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gobjedzex.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/guywxbmga.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gmnhqkiio.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gueuxkhbp.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/goqwmdlmc.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gvdgrskee.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gzrijomki.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gclboyvde.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gupssldvv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gceyyzdoa.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gliqklmpt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gzcqxuzmm.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/ggeuzflqe.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/giwlbxewy.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gyqgywwsj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gqtlecnfj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/ghidtpqwr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gtmeghexj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gznsxdjph.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gfmkyyyph.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/grurbmbyk.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/ghqxvtqbf.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gfzdcfxzi.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/geeallqqt.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gppdzujyu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gqvjiqqbg.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gisgocodx.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gkmxhltcd.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gdocexewx.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glppoljvh.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gujpdyuah.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtekqhxac.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gxwsmtqkq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gakncxflf.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gsvmqhjfq.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gwoaklqcz.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/guftjtddb.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvavtht.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gpwwqnvtp.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gnfmexxay.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/ggpkajoag.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gtwtyaesb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gaeiggjnv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gcarzwfay.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gnjpznird.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gkwqoqxdi.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gcgvrylxr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/givkhmclv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/grtvfnhis.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gyuubshmy.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gkbeapkzk.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gzdshgdsf.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gjnaeqojq.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gwijixnqn.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/ggdtofgnn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gmutcvegt.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gyskoxayl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/ggbjidezc.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gqiohuzgy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gqtedanrp.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gffdlwdza.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gayqlyyaz.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gqfyrvnjz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gtylnzhlj.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gwmqyguuw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gpdlqudlm.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gzglgxqdw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gktfmdrxj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gezodmmwu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/ggyavwddq.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gkyyberjp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gxaoazwmq.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gjeoonizv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/grertjwxk.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gwsvyslhd.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvcbwcvyf.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gburfxfvw.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gsabedrbt.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gartwnbbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gcpmaxrzo.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/glbwsqios.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwjhjcfyy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/godjidnob.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gxpzbhqsj.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gopjzhcta.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/geuowufig.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gkdldkblm.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/goodumemu.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gehlcbjci.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gsxlcxilh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gsvfybcxd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gzkapwuko.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gianxcgqd.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gxndykcvp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gybkiemal.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gfjjwyhce.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/ghkugjycd.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gjobdhnpx.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gvkezdouy.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gaeigojza.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gsmegsirr.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gunnjjggt.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gpjhfdgil.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gtlywfnzy.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/giehlbsia.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gbgdzdoza.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gplceoqto.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gzkblxfmu.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gxayymbqm.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/glmuplsay.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gsgwjfyow.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gopreqtdf.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/grfbscwoe.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ghtfuiorz.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gdqlmeawy.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gqdzvgxjp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gnxcpgygm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/grmyonklc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gnmzhaoei.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gflyvubmt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gozqwsdzl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ghaydtrqq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvxqohfcf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gooysajco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzyznvxxk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gracyxxmz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grkstqohw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzwavgllb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gufxxnytd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gtovbodrs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gvvjkowre.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/guodbqbgk.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gvbdcqwqc.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gdnixjeqr.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/govhhouqy.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/ggrfrrfzy.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gigzhtkne.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvqdaeniz.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsutdbgcw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glafknefw.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gtzefelwt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gumrapcsi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gaezipsyj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gnpsrsrvg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/ghlmqaerm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gbkeaetmb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gzknyhpte.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gosbqskui.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggucmxgrh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gvvmkyohz.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gtvbycxwy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnnwjjmwn.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/giyasiaop.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/guucdougo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/grzcipmxt.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gkrhippqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/ggfjzbnsr.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/ghpprfvpw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gowjaytjh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gkvdblwqb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gqzudjkku.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gnmdiawxy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gmgbwiuiv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gveomjqrv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gmcglgnku.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gzbnnonng.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gsnwiigfj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gunumscml.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gjltvqbpp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gjysnagae.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gvzetcazg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gghqfwfwx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gznmcoxac.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gnvswldkv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghlpgvbjc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gqxglildv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gpktmjlrm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghrmleoft.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/glvfmlfrh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/grbaygwxp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/ghojitske.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/ghlhorwlj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gvrooftwd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gyjictvhe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gnyzxtmjc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/grdinwdjc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqenyihlo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhsripef.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtcxhxpsm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gwvwgmdzu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gbhtcglrr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/giwriuqbk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpimbmbld.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gpgoztwpi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gevqwcgnh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gayboitdb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gstsvvrpr.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gsneqybrs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grendtytt.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtlysbjbn.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gdxtmsuzt.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gfwtrqkcp.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gdmtrxpau.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gnvjwzpun.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gsiawyxgu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gsgadwmjs.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gjcvzzlgc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gugxulfgh.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gldbxccxl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gftcadpbk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gjqkrigfp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/grazurgcu.sHtML


<!-- 参考信息 -->