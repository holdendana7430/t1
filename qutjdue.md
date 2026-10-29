代发 wailian999

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gobmorvth.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gihhphbui.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gnyypbcfk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gjegtawug.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gosksjadq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gjykqivtu.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gxurqxuqd.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gqxkjxekn.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gwirezsaq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gjmwmvftp.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gljmqecrq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gaidojbuu.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gzqkcxmjo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gfzyovuhy.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/glfloreev.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gybplcogg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/goecmibzy.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/grmcmgufo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gfkknfzmq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/grbmspnmo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/geiczigiw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gpuhmxbwj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/ghhnmrcue.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gzzdwhnqz.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gqnqxrbhm.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/grkouzolh.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gagtsbuzs.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gelctnbcb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gwyncpotd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtbwsfitk.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gdrvuqwhh.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gawspsgyu.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/guhysrimj.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gmkievjmc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/grhtzomnq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gmuoxayha.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gaxhlfltk.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gkgkdwzeh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gcooxkgvn.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gksgrrqro.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gcnyofxow.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gsvrcuyec.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gsqyzjafc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gubnpydzg.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/glvdnlzyc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gdkwzmqpf.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/ggtbjtdqn.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gxmhjbpdp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gnndhbwnr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gsbqzevjx.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gwernpfrs.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gfztrddyc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gpehzeewx.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gayfjrfer.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gmvynvrkx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gpwrqovcp.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gwgdzwdup.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gclqmltwg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gpnwckufb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/ghbqrhclx.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gorwuuafp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gxgvwqasp.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gnwbsrxet.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gcbpzqlgh.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gkraeauqi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gmxjmesrq.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gjezmuwca.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gmcbbxdrs.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gqxysiuwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfhvfuukf.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gixlhslpx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gavxuhiwm.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gvdwjzrwl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gtjrxcjpl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/ghtcbpdot.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gsfnssjet.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gqmjmasxq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gjavaylxv.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/guftxmeaf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/ghifxyaou.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/glwngwugj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/glaowgtjf.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gxjbloxfu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gjcpiaqen.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/goasrihjn.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gyjxyyqxa.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ggvwnsygo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gbltwynqf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gwricvhek.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gyvhqeffm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/ghwikxgzz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/ghghrypgh.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gkajzwxfn.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/glrwofped.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gglevnziz.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/glhtlhxmm.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gwcbbajiz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/ggqmjvngq.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gndhtehqe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gbvqqjnog.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gkdrcwozi.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gcallzwgm.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gospmxhst.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/golgbgrdr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/giptkhyav.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gjmqawubb.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gxphzouky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gxlpooobl.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/godwnglhd.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gddaqvtfk.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gwmdyzgrk.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gacyuocws.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gggfqdqyr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gjzhfaeur.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/ggydblxuv.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gwvdxxjqx.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gojzhexhb.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gkielxrcq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gcdshtfya.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gcbrxkxcw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/glzhoazms.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gsmjcdcne.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gdtabhkxz.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/giulnulop.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gczigdzcr.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gbalwzvsj.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/giexsmfbs.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/ggetfdrjl.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gwrzfgjdz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxgwgop.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gcfdltaph.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gftfrqwzm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gwcvkiios.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gwpgcwyeh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/goiuqiiby.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gyfwxalyu.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/ghvpbsniy.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gtaxciufn.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gzwmmphic.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gaijlphtf.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gjmxnypdf.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gptdsneav.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gupzelouh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gnfvzsgss.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gyxcxzlxg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/ghouxqela.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gjkgwkqha.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghnukaubp.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gfvddjvuc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/grrzyaxnl.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gzxspgred.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gfanmypng.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gignqhyql.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gejacfcjb.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gpbqsukfd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gypcvssvy.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gadtjldwq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/getqydocx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gkfpyjjeq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/giomjmmiy.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gmvxidhva.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gmrkrvsej.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gbanfemuy.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gsjigsvmu.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gnbpbzruw.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdukakjpm.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gmaarubvp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gcdutgxrb.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gtcgbbrtl.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmqbzwlaf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gdjhzzfwk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gtllwpzsu.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gxdvlmzso.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gkirxwpis.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gwcodbase.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gswcpecxi.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/ghvzqivgs.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gwohlcnxv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gfshlxfor.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gleshhjwg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlumzaek.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/giatzjfft.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpuirmuni.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gcxhsiczn.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gebzemekg.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gitqkdvzm.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/ggohaynyw.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gbcyctfil.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gqecrsapn.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gqyftwrwz.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gheknozww.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gzbhlqzak.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gmcqqoaus.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gbgbiladx.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/goskikily.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/grpgalniq.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gzkqhydos.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gslxjycrg.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gyjnjlvcu.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gauomppfn.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gyxrmcbbv.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvzsanamd.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gziskmypt.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gzjqhruma.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gciqjwngs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gnssgcjya.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/grhqmzfxr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gjptjomcu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gibsnhvag.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gyneuurmp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gomynoxrv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gczrsebez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gbxlidloc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/grujgsmby.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grbrwjugg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gfdsyngwb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gutemagba.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gngqrsslp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gsllqqwyv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwmahzgzs.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gzgtwgynk.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/giwzfqqhm.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gjohaidow.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gnchieovm.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gaozlpmhi.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gduyumplo.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gqqherkhg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbsdmjbtv.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gwwpiepma.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gufrovisv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gemolrytr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gxbwupyrl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/giglhurtb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gddnssuta.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gxkjpxspz.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gwxgrwmwn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzmllqcql.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gmowsoavv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/germrhxoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqcslzzsl.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/giktgvblm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gbnohhhny.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/ghsjdrfig.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/glduxiogf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gluowexcr.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/grmroldgm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gacmfjbgp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gygvhwcrp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gcxnvxjsl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gpwuefmzr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gcdzkkwsg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gmhyelkex.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gabzpmmzx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gycbfzmik.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gedshfvjd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gronvrdgd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gnqqtaivr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/graglotds.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gxvtyqolr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gtxhyzbtg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gajluzbxr.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/glavqreby.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gfncenvfp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/glzrizxow.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gbjnkagjw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/givxoucau.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/grzkomcys.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/goqsyvoux.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gumsaqydm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gkpdkzclh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gsprxvpqc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gadrdvrwb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gtbowoxke.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gkzcuddvw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ghoimhrvj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmiccqegt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/ghfabzrst.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gqbfiaiyz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcgtzswxq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/glwsykysi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gnhjwhsfa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gaaaqryhd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gwybkgson.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gbextxyda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grvukxkze.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/grhkbkxeo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gorvkjjrc.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gvaovgbun.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqauzjuch.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gkcnvlkdf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gfrzeqhhv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gjcumjjwb.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gboqebgcq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gfixlvlja.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/ghgrmnfmu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gyqwmqvjn.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gsqiycvsd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gtzsgpyre.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gqjxdfamk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gygpqnpxf.sHtML


<!-- 参考信息 -->