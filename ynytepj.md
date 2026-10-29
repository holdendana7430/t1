代发 wailian999

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gyerelqdx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gebedtjfl.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gfgvumjlm.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gcfdgzxde.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/ggmtwruld.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/ghezodfww.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/grwftnkbr.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gwvytxwfm.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/ghvdfmmmi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gojwtfgel.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gsqsusace.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gptbahftb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gwnojcnqc.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/glwxkdnta.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/grigxwylo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/grcvnviwa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/genzoscts.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gcifqzigx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gdzrfzufd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gmtgrwjhw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gtbkfhcqo.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/ghktbyqoz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gggqvjnpo.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gmowvgmgx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gmsnoixll.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gelruwwdl.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gnbadlhay.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gqosfwcrn.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/guoggzpna.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/ggrdwzivp.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gbmfcmuud.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gocwvsnhf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/goraqhuqd.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gxvikyhab.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gqdommeme.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gexuftohr.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gyrhupnne.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gombdguqj.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gabbapnab.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gbgcldwvg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/ggmfgvlfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gfmzgywdb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gubrqidrk.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gptmdalhv.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gcyhwbvff.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gtojaunqa.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/glkuffcyy.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gbtejyatz.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gisqvjwtg.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqnffxm.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gdbnoqaez.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gvddlkeeb.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbiewppsp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gcnztygdq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gggfqamca.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gnwyphqvd.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gvxqvdlvd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/grldycarr.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gxloadkjw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gzexmgelt.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/glrfhllpu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/grtxkomrg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmezabctv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gddmwwxdb.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/guxhkahhw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfrsebjkz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gxnrlxivo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gwvktnbpi.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gvgbsubbi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/geoelkiuj.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gwfzbfwlr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gjpwlbmgm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gvkkbgefg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gldkkajtm.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gqrsnwxlr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gjhvhtbuj.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gmpcwifbj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gzehhzoss.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggfqbzgru.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/guzuqhocp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gzvetvekm.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gfzrzghmo.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gspkrieeo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gohxqbuhm.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gokeajabj.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gnxrubzcm.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gwjwldbjh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gcncxouxd.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gxkoibqwa.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gffusshfv.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gjtxczrcj.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gxttrikbt.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuilxzs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gslfgzpnp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/geehljqsf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gemhbtcgf.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/giqgxdtbi.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gdybvioph.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gowbrgqxy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gdfayocfb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gxebcgjhj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gjaniaedp.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gfmndogek.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gwbkyhufi.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/grmzmqbkb.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gtyopkcxc.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gxefprhli.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gmuhkooqd.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/guzfisamq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/givlwhwop.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gapfcygdq.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gxbkygqjz.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gxniqptwf.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gexyogpch.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gttocnozu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqfgyhvbd.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gmwwxqers.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gmfwwjdgz.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gehtwzfhp.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gkfeacgzu.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gdsubqqsd.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/ghugwoffv.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gpxrzpdph.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/ggkvxglbp.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gtvqfkesz.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gsilhawli.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gwfoxdvoq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gvlpyynfx.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gxfberfws.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gcfsnwlpo.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gbtsjkxna.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gueywrscd.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/glvuvffdx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gyaafaebq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/geieplzth.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gaaexglpk.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/ghixbqgdx.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gpgzzaiix.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gbbdjdcbj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gfsyiivzc.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gexvcgyym.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gbayvqpki.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gfoatxqxe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/glqiapnmb.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gufbcgjso.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gcdtyberz.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/givcgtsny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/guzvmvndm.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gcqdmdmeg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gwqxmwyub.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gtrvickrw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gpkrjkzks.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gfapwrbtr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gsdpbredy.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gkcrbirtx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gjhveemxe.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gtwqedhbk.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/grvjfyvha.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gxgmidafl.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqgngrhny.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gvfnjotyl.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glwufvjqy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gqtxmbbia.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/grzizysgm.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gxdgkhsah.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gwiellrzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gsijtmgcd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkfmzbnnq.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gfiztcmst.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gyosjnqas.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gtltsyfua.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gvwfcmczo.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/grswfdjjt.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gsjanjnwi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gnwhmosuc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gwfrbqkcu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpkhcyttv.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gpkvienfe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmuprehzq.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gqcksutjm.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gnigatuyh.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/ghdpycjiq.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gwftrryhm.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/glufoubsr.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gysvvcukj.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gmpwrexfp.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gnhsijmkf.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gufmyuuew.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gtdiciosh.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/ghxgqpjzi.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gysclilgx.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gliwmjxxx.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gpquastpf.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gzrfjelwm.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gqtmfpfmz.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/glfarwpho.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/giphsrmke.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtxijtapv.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gmlscxjec.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gmkrurujb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/geghbgmer.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gbahbhqpz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gpezmngjb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gimzytnzo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gqfnwuvke.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gwqpslekr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/guhhuxwib.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gagdtxzdp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gcalnjqmb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gfmmulupv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gfynohcxk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gucaicxii.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gzrgovbyy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gwrwhykwm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gptfazfvu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gvopdypey.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ggihzosqc.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/ghnejipjp.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gplqcftur.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gfuyoybtt.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gkxnzkzbl.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbnsduusn.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gvkrqqozn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gustdienh.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gpkrnujao.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxmbpjgip.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gymkljihr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gicvbqtzp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gwjxsntig.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gvbartxaf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gailzkkyr.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gbvteaqwy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goxcmjyou.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gdcrggumc.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gbmpcedag.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmlethtsa.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gtjtiqicn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gvylfngdq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gipknxzxs.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gflhbbnyj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gkabsrmmq.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/glfkthykv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gldspzyqv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gplfauxhb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gikuzvvqa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gpphgitcv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/grpgmxpfk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/giiqeppxo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gazriipik.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gbeynmamy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gmtronkht.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/goitcmbyn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gwjeksyxi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gjpouabna.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gitlydoin.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gfwldesie.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzjnqohgk.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gjhiizbdp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtxetmkrd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gzfshsstn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gdepfgxtv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gkdfpvewl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/glujjdyzv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gaxkclcjd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gmopsfbcq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gfwhanohk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gzjbzyazd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gkuzfwlou.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnjbouegn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gecpxpdrp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gtfwukauf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdhjhsjbr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gecnkmbsw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gqkzaujpy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gpndvmjoc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gtvhrsmlo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gipvtigbm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gzygmktae.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/ggqbxcttp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gmpljcpsa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grjpxgorv.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gkfpfxpcu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmrqkzodq.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gsnvutcfq.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gequzgkjx.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/glrvfwwrr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjadkejbl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/guiffhvfh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gqlzpcbil.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gslqqhbnj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gxplwubxn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gsstbbtpm.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gbzqamxal.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/ghlgnkyry.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/geaciwdfu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gckowcyfa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gcjtihcpv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gfyzxzbdj.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gskxypywl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gbypzpyhy.sHtML


<!-- 参考信息 -->