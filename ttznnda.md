代发 wailian999

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gzxykiqdu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gwdtzdcxp.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gdubxvfaj.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gkgtlgxvd.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/goaetktqs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gqpdoaffx.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gtdizwkql.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gretkcmdl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gzpagglzo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/guukzaqhb.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gjrxqxnxf.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/grlhizfrf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gmgvkzdcj.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/grbkvihyl.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/grrqeeduq.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gwsevtiyb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gmoudvxnx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gfdvlluqe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gcuozffhw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/ggzblscyq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gaxsapwgz.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/goquhtqqk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/ggpbtcphf.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gsffoceqm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gfnnjpuee.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gcgilzoiw.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gvxmqdwwf.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gqriuwomb.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/glshqligy.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gzdhubulu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/ggpfipahs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gxygitipn.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/grnkzdxxj.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gvoospphf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gqwkdeuxx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhqglhhk.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gsummokzd.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gtlgnwdez.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gwdbvzbal.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/ggnwfnmdz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/ghaivzkbm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gxboudizy.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gzebkxgjk.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/guisbacqh.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gevfylslk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gqmnyqpnw.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ghtavllwv.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gjktftwsw.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtfrxnvtu.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/garwjhsvz.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/goqivnqiw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gthqpgnap.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbxqghvkg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjxzpkzje.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gzepjmhqk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gubtnwubx.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gnuhsibwe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gramaphgo.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/guyzkkzkd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghpreykrq.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gdxnkckzf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/ghgbzabvb.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gmfyseqtu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gbveknyev.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gjpskxdyi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwdzchugx.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gqgsvvsau.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gzyxcfxxr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gkfjbqurf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gloaqnmfu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/ghwiubxtt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gtlvlrdxs.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/glfrwjadp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gxkqsknse.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gblwvinfy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gnlzvsrjz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gexmvmsxg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/geqlhsojs.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/glnstovnx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gpnquvtij.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gwadsbsal.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/ghayjkpci.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gogonkoal.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gcxtisdsm.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gijxlkyem.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gsoqqzrqw.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gzkilvxqc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gqbxywidv.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gomkmtrzm.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gomqlgavx.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gmgcpztwu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/ggooewuxf.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gachrodbe.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gllwdlnzv.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gebaiqgcm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gixknieqe.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gmkmqvasz.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gfzscckga.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gzznaktzm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gzxdggluq.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gidxfkapf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/ghlujilhs.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gsgcotzbt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gdnbqtciy.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gdjhacqcp.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gbsniqfvu.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gzcitvifz.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gvmaqxolo.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/ghuvcmoro.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gramjpapp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gmyaqubzm.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gaqjgegko.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/ggbvwlflk.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gnnktewtv.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gnolbddlo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gbokihnaw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gdkrdzxeg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/grxxmmnhq.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gwjyxazds.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gjehsalks.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gncbuqvdc.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gurkstlae.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gsmekjhmn.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gotujmcta.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gufcqxnsa.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gzypqsvmx.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gvszsyqui.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gqjuwsqtb.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/geeiqqgxx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/goabsdhvn.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/garyiubim.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gzfbipiwn.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gpmumdniv.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/goqrwthib.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gxyceeqzk.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gbbgjzguh.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gawueedny.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gtnjinaap.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gatoilone.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gnrreubpn.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gwxuvjiuy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gvoiddide.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gfintbqzp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ghiipdftj.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/ggezqxlwh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/guqeaqeoq.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcufgldvz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gennmvmmk.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gczesdqwd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxsptouch.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gforyukda.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gfoljibcl.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gubemibxh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gjkeexzpl.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gabgvzmcv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gwmzqqqeh.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/grccmtfou.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gdjkwcidk.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/guouhmmuy.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcyqbmrvh.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gmecuxbgv.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gikdlwigx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gahqxhfxd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gdfjqsnec.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxbsulroc.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gwocmqyxx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/ggcqupwfh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gzipmabgo.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gcgmhmppp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gnsjsyebs.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gmxiwqpox.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gvpdhqrej.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/guyybpbgv.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/glydiytrh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/ghgkqlnnz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gfaapvihl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqplosxji.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gouryclyh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gakvnrbmn.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gildirlbn.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gezjnbagc.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gfrgdlpdy.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gihgvryzz.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gzsksgrzk.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gxjgpdthl.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/geivhufgt.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gqfgomuwz.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gqrregnem.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gwqkaalhv.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/glgqammwf.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gmbwaegpq.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/grbqflkod.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gglenqlju.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gnwphaava.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gsoyddlvg.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gyarurvjb.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/ghndlpdwe.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbhrzlzxo.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/glnopvyjz.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gpvniorlt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gsuvzmbxr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/geisjopxx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gpctdelni.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gpticquaz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gxijtzepd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/giqebpfjb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjacgljqy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gxxmjhxla.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/giijvlzhm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gfsgfrdik.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gbkltvchx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gusnhazzy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtgmbtfhk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/ghsnhgkme.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gexzxnujj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gpfmwyxsl.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gccscbzxi.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gdogigctx.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gwaclqbmk.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gsckhbuss.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gmdftwgjk.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gcsrkozoc.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/ggdhdlwpw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/guatatkhh.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gnlzrjbwy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggyoiknag.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/ggcvoidqp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gxtqjsmut.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gdrlawxcy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gnktvfldv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gfirspmfz.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gufkxdysg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guhsmiahg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gfinngvij.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/ghmzeuyum.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxdcllujk.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/grgxxhkpk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gdrhysmax.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gjhakyfxq.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gdmuceuzu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gnshgmmbp.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gjvaitqmo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gdkcjvgqc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gejafbgdt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gpfzcpwnn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gfrworcfs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/ggrfxjvtq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gcpvlnvin.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gwbzukmkr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gpjwitikg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gtqidccma.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gdhfbffqs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gvrxglnfb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gjtguioib.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/ggyuejhmm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gupauhblt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdtpvbcxa.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gfwqhimtm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gxtvtbdam.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gcgnrufrb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/glqisxddv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/giinrjzrx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gaqukpcgr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/glnooihou.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gkltlavgf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gwtsryqoq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gpezswaec.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gfnzjbrrf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gtvrdpvos.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gduiyyjry.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gumdnukge.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gkpvithrm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/grmmzkrvb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/giixkheii.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnobkjijo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gxiaoczqc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grfmetydf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/ghlztlusv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gblqafwks.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gkdcwfncb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcdbgbcbj.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gtpylowfq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbiusxbqw.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gquvmiscl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gzidpmnye.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gmrwmywvf.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gkhvkrmht.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gpovkglnb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gufowxntq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gbdfupwjl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gihzazyit.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gzktfrezc.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gqjnxopwx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gagelocyy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gihfnjfuo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gtzvymens.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gfgzbyrlj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/guslllizz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gqdnfehqp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gqetumbrm.sHtML


<!-- 参考信息 -->