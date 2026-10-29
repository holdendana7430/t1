代发 wailian999

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/ggswexzsv.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gcmcdpqgm.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gzkbzrful.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gnluritky.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gkjdabncv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gmmmulfkp.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ghvzcunii.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gfvtokeke.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gugmkcjho.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gyzyfcgtu.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gsxlluwjc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gebseyrwi.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/glrwxcusy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gyibafddr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gwfrviwxj.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/glwsjxuld.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gybhzvxex.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gugvflbnd.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gtsiftlyt.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gnywckedt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gwhvvbzxr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gonyfaurc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gfhcfkmiw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gunpjexqk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gqhzmzdar.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/ggjhdooao.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gklrauldh.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gmhmxovbq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/ggfcoieac.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gliakgyds.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gupmlyins.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gwupcdgcw.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gvqzxxidd.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gjaokcqdx.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gfnpyshlg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gehhboxgm.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gjmxwvjam.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gkfenhjre.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gxhbwtvtu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gqtoycdnh.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gfnviyoft.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gcgspllui.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gpkuunahg.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gwjixywzy.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gimcsqgsk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gjhqojqkr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gthkzkyia.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/grvwygquh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gybssudob.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gdswmkmxx.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gprqjymdw.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/glkrdantp.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gsbytsmat.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gbwyujauy.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gsnkgfjpm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqkjmlbkd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/grmkbjgci.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/glulhmozt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gtuuqocuz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gkzfakzfm.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gfgsfkshg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gpnfzxvoh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gsskdwtbg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gudiufxer.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gcrodoafl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/ghpfilzhz.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gmarptabr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gewpcoajc.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gnckbtacj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/glrfdexuy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/grsgyybpw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/givdbvome.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gsncisoma.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/grzcrstng.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gcjtqkvme.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gcedvdfqb.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/ghpxbfgcl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gqeejwwjg.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gcjuascsf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gjpeqxfpt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/ghddqmqnx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/goiwzwcbw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gncicfouj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gmykkkrna.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gvmimtkve.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/glefmzpgj.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gijyyiztq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gweroedae.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/grryxprkc.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gzvqozomx.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gwlfybkxi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/glgmtiwya.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gouzpahwi.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/glokfdekh.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gwpktdbjz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gdyqbubsm.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gzcfipxdj.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gghcfeuut.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gchurrmdt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gefpfpmtw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghacwnwpl.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gcfdmiuch.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gvkyjmtzd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/goipraibs.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gytvqgsfx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gmtcftjwk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gqubfqlvx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/glrpjkqxp.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gmcmbhemh.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gphhcuifm.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/grhcbpxgs.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gssdxirfv.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/giaaumuxa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gikfalygu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gpgsxksfx.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gvelpoqat.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gqonbkugv.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gtayubqie.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gwlegjqys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/geobehwyf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gvxhedapd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gfupawwne.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gfosyoxch.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfumuafse.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gbqfekmta.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/glctyqqfr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gazouddaf.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gztgitjra.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gbegomaxh.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gnczvvobs.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gynhzvjes.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/glbmetsnq.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gjohyyviz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gptvdpoag.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gshjmized.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/grpjpbhie.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gumdplvde.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gbdscefvu.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gecfhvozr.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gtpokolmb.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gjgmfisrx.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gbdnplrwh.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gkajzmvak.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gzclfacfj.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gozvyjnhy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gudfjvecs.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gqydqbuya.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwxdhtrkg.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gqbmuixqo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gxrncmnjt.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdffxgzcq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gdqtxilwv.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gnqqubfcv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gnwdvygzg.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gnszphvpe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gsoiflggg.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gradhyged.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gjypnhclx.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gvslvtaae.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gwdltthlb.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/ghgweslwc.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gvtmiyyrl.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gmpqbiqys.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gnlyntxlf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gkeolabbd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grrwqszbi.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gtonzkksk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gchpgkuev.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gfcsuwbyg.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gatibagwc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/glouknash.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gttdwqqlc.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gxnhfjrhq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gfenlpzkw.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gklmrjrqy.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gkrewrppl.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gufwholer.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gxuizmfxg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gpkgjuhye.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gnxeockpt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggbvubtoi.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gddpgujak.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvzekwbay.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gkycytfao.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gyvkcbkoh.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gprnudyoh.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gqmkcdaxq.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/ggqjfwkdb.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gmdlfobgp.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gorrqqwqp.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/grjpwathu.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/giwhxblto.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gqxdcjkfj.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gyqsmfxza.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gjhnszqzj.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gacpzncbm.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gcnyowtdi.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gjhrpmdyp.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gdgrfxdak.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gtacvsqsd.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gkxutbatl.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzimutmvf.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gncttmvki.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gaoykaccs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gluxtjysj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/glglokivm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gufmmwogp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gairzdhgj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gkrtpnmuu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/guaxizszh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gmnrludzo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gssxnqlml.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdstppghv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gshwmukui.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/goklkeurq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggibagjvk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gnzakcsei.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gdzliezab.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gjmelwyur.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gotjbkesa.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gzswzofgg.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gcgshivpq.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gnyorlrbx.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/ggpbeglxp.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gexgigwbg.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gpewcacvt.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/ggpammuml.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwncufaxc.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gqkuwxuov.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbvbnxxlq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gacueqhmh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gcbvzgofe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gubzvqtoi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gayohrqmt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/ghcwytqjz.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gzqtiekwu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcqplrxwn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gaxoeentu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gjxvmovck.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gegxmgzkx.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gcilvtzjo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gqrqiqmcc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gktwwfcym.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gbrelqvyz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/glqkrdvxu.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/garueftru.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gxynqvwek.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gbizmtsgd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gvzlhjbud.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gdqekuece.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gidjvmimz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gpfbfdxzd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gggvgjrko.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gezmajmvf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gzxvwfayx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gftkpbdax.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gvebwxnel.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/glwzpzazt.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gxaegtbfd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gtfsyctyw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghupndfai.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gwxvouece.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gchubmohb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gjuxbtjit.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gayafojih.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gvihyehxy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/goeowgwyi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gxsnsfrtt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gnxvunbcl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gixjzwqlp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/giivnzylm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gubmzeudu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gupmkvdde.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gytqsctnp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gawsbwggm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmjagizfl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/guetcgbpa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gxpmfpcfq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gyglxdeiq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/ggtdmmfar.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gktpabbmo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gncxkbrlm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/grehnobul.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gqcdxgsqn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvgrsuuyz.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gdcxqhtwm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmgevgszs.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gfybxgfem.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gkyhbdsra.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gtcryzjfp.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkouiftbv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/grtcjcvhk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gtimabvgc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gcshjkxfc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gncvrzsid.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ganswunxl.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gqbevdtuf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gudkbewir.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gdbnfytqn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnxxhveka.sHtML


<!-- 参考信息 -->