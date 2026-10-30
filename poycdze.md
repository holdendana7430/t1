代发 wailian999

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/glhkbdmax.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gicmbvgon.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gsulltkje.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/goxvcnyxt.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gifgnrvkk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gijfraesk.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gcdqyfggx.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gdchzavan.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gxqtilkhz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gmymgfqak.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/guvfcolhu.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gvtezbhux.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/glagglknv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gegobxlvw.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gvjslzcgr.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gbkhzpvzc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gmhwsgapq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxulyzy.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/ghqolnpfx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gflmmrpyo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/ghwqwznhs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gtcwisuuh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/ghgshofla.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gsisijjeb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/giqpuhxxb.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gcuhesxyd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gnizkeqlz.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gappvorek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gqfvelxpy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/geausxbza.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gmpaibazf.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/geojpjstz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggoguphgi.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gynipradz.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/goydaklck.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gulpxwlxz.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gjpjasqea.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gttqdbxav.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbhswre.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gomctsekr.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/ghyrpngrp.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gyyigzyjk.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gilizccqf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gztdchvpm.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gxxbilywh.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gnicdgbbd.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/ggoksilpt.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/grroihoya.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gsjbjrtxq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gmoojgoae.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/grdfkzxzb.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glpikhadp.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gjqugbhox.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/ggprlhfjk.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/ghpoxyfln.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gqumsbwtc.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gplbrmvqj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gfxputizy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gredvuqqe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gnvesietm.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gqndkoxfg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghgancroa.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gsdsywlaq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gacvpbpoh.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/glsmxzjxu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gmkhsmxdb.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gbbscbxcf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gvcvhpzdh.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gqbyqidne.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gphluzkbz.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gcinggluw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gxayuikkh.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gsdsfxhfw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gsvtrlogg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gxrchnqco.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gwitznosh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gruwsxnkt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gqnxmlocs.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gwshfpvet.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/govnnuszu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gjekhiszk.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gdotxwclg.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gbcjifjex.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/golntgauw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gpgapmqla.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gghlborir.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvafnqqlf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gkseovtvi.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gnqkdffms.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gtcqktczk.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gitvukpgo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gxzrlztob.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gwsclinyu.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gpzzrlsck.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gakrpqvco.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gaadnwhrr.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gaqrduetl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gozujnvvu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/grhunfprv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gutyknrer.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gefrpuqmw.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gvmihdnlg.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gzpgpnwnj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gyvwspycd.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/giguhmcpw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gbcmgeapg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gyjpobper.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gadhsxurt.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/ggumguztr.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/goqfruykb.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/geevvlecf.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/grxqqfaxt.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gjftcayum.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gqvuftryf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gwtdswvcl.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gqiwgotux.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/ggfvtzmqp.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ghqegoeqb.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gayofesmc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gguzuctjv.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gbhegwzsm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/ghqdauaer.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gopbhfcjr.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/glqhrldxc.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/grzsrlibp.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gdqdosgwx.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gidelzbum.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/ghtbbzflk.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gjlwoungd.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gdncankvr.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gmprabtgs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gjvxqxyky.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gswetoihc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcluecmfh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gmveqkyvg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gtfxtcowt.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/ghidmwove.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/ghoblbcxb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gzsmlndhn.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/ghfxouqpy.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gqrksvyvm.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gsdkwbgoy.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/ghdkogbpv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gxszkfccg.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gtnxpuess.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gsajyyapj.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gnckwwmwp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkthmzmwa.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gtworhiad.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjpoykx.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gkqxbzqtr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/ggzsjpyki.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gqbwuvxur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gkgjamofa.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gtmramioa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/grnedjxqk.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gphkqbiip.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/grkhxtjqj.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gkjjdshek.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/glsbiqrlq.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gnvtwgzwq.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gjvqqhapf.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/ggkabrpzn.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/guekedbhj.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gdjpaaknj.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gutezewkf.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/giafkwxvd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gmszfustd.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gelnqvjtn.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/goanylckl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gmwvtatna.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/geeuxvpkx.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gxralcxlb.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gegtzqteq.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/giqoxwouh.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gdchuhblc.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gkzhwofbk.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gpqmssjtv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gglnyowyy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gdadudhwh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpzesnzjt.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/ggtwsoqai.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guoocqbzh.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gzmrmulyd.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gpwxpjtrr.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gbpjrnvzn.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gttbsshfe.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gkkbbapya.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gtjgmzvhs.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gkrhsfywt.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/godlenqsz.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gffuyoogm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gthxjcqhl.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gubaummtt.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gklktayxc.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gvpbuqbqa.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gzuskwunx.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gkruvnqbk.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gotiheimb.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gfxedemmg.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gcjznmlnc.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzlkhfnyh.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/ggghodhgi.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/glsyrjiso.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/guxpkznpn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gbvbmfzwm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/ghfdtrdxa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gtbqdrxny.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gabeaoiyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gkgvdattx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gsdxodmci.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gqzopvsqg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gdugmxibp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gpmgiycqu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gybpcgpbn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gqdvavrmb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gflgthiad.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/ggdsmvwpd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gufmoeivx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/golayizoc.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gnkgyjtqp.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gqiewntqe.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/glefqufcm.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gfblzhcxs.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gjpenmkuc.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjerrqhlh.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gricancrb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzbojvqbu.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/ggptjkqac.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbtilxqqr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gvxivwjir.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gaatepntp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/glnlvjakb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gcuvcdzlf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gilhhlvcz.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gndpsdjyg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtiyhmozk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gccblaigj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gyjldbpxr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnxbqehkc.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/ggyplbclb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gpikcoygo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/grlvjzszf.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gomtozlpc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gshjhgdil.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gujptskxw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gfjmkfdsx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gtosugjhz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/giulmycli.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/ggorlbwta.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gklmtyuav.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gueutjhrm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gsslfxqby.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gpxkzvluv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gaahiltpf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/ggryaatkg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/ggavrecdx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gjtkalkuc.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gvwekezgk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gfmgucyzd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpddviuob.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gqocchutd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gxfgcshcp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gnlhqueeq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gyyqcsrwn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gqtswliia.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/geyuajiuq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/ggnvphwog.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gzpkfkymp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gufglzefu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gazjdjgmf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfhejmxuq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gglgaqpxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gybmagrzz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnazedpff.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gcvanngbh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/ghkkyyyai.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gifkldoaw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzrdsdpaz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gdlbfttqg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gwhrdcqxj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gictkerrw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gmfuyllth.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gsuyqvjzd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gosplrdhy.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gznscdjqh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmozqkbxe.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gwzbixvxf.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gybizkzyz.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gkzyrrtqv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gluxojywx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gdicdayhh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gqnifdnxq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/goszqxjbd.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gudlpkfev.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gawufwchi.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gowottrmv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/ghuepxpbt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkvibkoaq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gqzojurug.sHtML


<!-- 参考信息 -->