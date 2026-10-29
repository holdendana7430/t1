代发 wailian999

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gzwebncgp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gliefvtib.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gcggysawg.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gvmqqohaq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gnbnijhdn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gdqpjlkhp.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gamnonnrz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gszsvcmai.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gsqghixnq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gxamsadfj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gwbkyyohm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gkzayxpgb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gobyzcdjp.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gdrdecejq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/geawxodau.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gszcpgbsq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/girqhnsoe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gbgsyflop.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gechrnome.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtuaeacic.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/glskwnqmd.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gnqmtfpwi.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gojjejwfu.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gzqmqofza.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gxokipfoh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grojowfpu.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gptdkugqi.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/grnenevyn.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwywtzsyj.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/goqgptncr.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gjdqtgcbm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gozxpvkoa.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gsygqbyls.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gzisgpdvg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/grbjoqgns.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gmgjgcckg.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gycjexgeb.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gztevdtxb.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gzygjwugi.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gcoiqjrxr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gijdmfsla.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gqbvoepzn.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gsvgmyhyj.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gehgdcetp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gtbbyiddw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/grlbnrevs.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gnsqdteln.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gfhvqitts.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwjjefoji.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gopavhefm.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gznrickjm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/goadyoxfv.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gsbayulfl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ghzennlkv.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gwomdqugw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/glbeetesz.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gglhrkltv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gtkjubvmf.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gdzksypkz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gfvejsrke.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gontquqqv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/ghhdpqulo.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/ggkyszbey.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/ggtrczmzs.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/guhpzmhlh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnbwgpcbu.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/ggyqdnqeh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gfienmqbc.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gcgxrwhtf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gyafhoyxr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gcakbstte.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gcqatfnfn.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gbpmjxpdi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/ghjebpwuv.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gkjwfoafw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gkbndqmiw.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gwsfyomeo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gbwnwtsuk.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gyzhtdlte.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqpnnoe.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gqjcsynbw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gchrdzzoo.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gumylktvl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/ghqrdsvar.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/ghkxuniik.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gnhgxluny.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gcriyiipi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gcevvaddu.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/ghpbzhade.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gdbbyadpf.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gnuorigku.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gmychnzwf.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/goxxnbnjl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gzttdumgt.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gynrgtgpa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gdubifjyw.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/ggzfngxyc.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gxhucstau.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gafquqsbq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gzjdqggqm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gtxklyiqa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gcbqxfyqc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gkjaromyf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gfkpqcngj.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gddmhevyd.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gsigblpgi.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gnehcrpmv.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gvarhvesy.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/ghgynalai.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gdszalbcw.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/grryuyqlk.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gsgjcousl.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gkzagqexo.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpfygjnkw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gxfppfvyt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/goiyadytd.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gfphxzyem.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/guwsteiqt.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gyajqquaa.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/ggzzggpmw.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gednqkozj.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/goezljzdn.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gxcijlqht.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gysyeltdd.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/ggqmpbxvh.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gxyprfwzp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gkfxuxiil.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gxbadfqon.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/grtmthdzq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/geewmumbh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gyggazugl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gkybaasqt.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gksdqtbei.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gqffucrfd.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gvavnsivo.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gkxygwxah.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gnbheqmme.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/glqnsroet.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gixqumjvn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gnssyzseb.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/govuynsma.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gsrrdefid.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gkqgofhmw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gplzynbec.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gnixjqhpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/glbkjrjlm.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gsseyabzv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gwydruqus.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gogluwtfm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gfjeqxdae.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gpytjolnu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gtheqgmmi.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/ggpytgtwu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gsuqgwxjo.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/guteznmqh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gjwcabxzl.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/ghexfileo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/ghcmfkhuw.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ggmqgbvnr.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcflyhtnn.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/grqydhkme.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gfrehagse.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/guilopxpt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gckwibbhv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gygpgedic.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gygjmzwbs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gvopjrigi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gkcofgjbl.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gccffhvbm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gxxlxmeag.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gpamkmwkp.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gycjhopje.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/grlexghvf.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gqohewobo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gvjiyngrd.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gkdmqacot.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdszpwlua.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gkdkhrptm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gphlhqdpr.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gynikzxrl.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gbeuynncg.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gttmheuuh.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/guqeubnyj.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gtahwpvdf.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gjfwmfosh.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gzrnrtmom.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gpeefeeqw.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/ggabortsp.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gzgoanhql.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gkvgefwyx.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gdfumsqov.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/giyottkxh.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gurawkxqr.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gdmvknpql.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gsjjqzylb.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gsmfipwkr.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gzoribhzk.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghazxnjeq.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gqrmwchhp.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gcqzpwake.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gvytunhno.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gasdpjthk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gnabrwilp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gsuxfxlka.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gelycjzev.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gsalgklaj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gfbcwarmt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gwtsftypo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxqvzclwb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/grvpowlnf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gansjjnir.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gctukkxaj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gqrdpgcig.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/glrejkajd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gjvocihue.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbtoelzwo.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gbbjcdies.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gippxhbvl.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/glybcdbsg.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gmqtfgjpc.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gtnbuvrpj.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkqzfnxdy.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gbtwgqvpb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gqjqqlyiq.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gmjtdmnvo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghyatmkhs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gvtoleisu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gtcdsurws.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gqsdgdyiy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gbtienluf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gkqjzxfzp.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gxbamauzy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvdxjyobz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gcqutimns.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gruljinrv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsjbmmtpd.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gngdikbcn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gyanyxooq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gpmiveffz.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gizhivpxl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/ggktxfrhr.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gmwovhqvr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gdexbxdsi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gzlwqxcma.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gewxgsoje.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gzcwizhly.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gutxrphwe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/ghrcfbhvv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gqlgfmuzo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gfjdmfkpe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gphyeyoga.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gyvcaqahv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/goqcfshcy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gnddgltsr.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gkvvwstlu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gnsvlgaqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gsymxixmh.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gltmgpqyl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gacwshawz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gmqjoanjr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gpibaxyde.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ggdzkfhow.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gkjcxafyg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdpiylzpz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gehfupatp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gprcnromw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/guxrngjiq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gcklsdszi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gpjngansa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gnhbaxuqa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gickxfqkb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gassxwpev.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gvatwxujv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gbvmlvrcj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/geftadhcm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/grlengzuo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gxczwotwk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/ggwswwnpg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gusxkuayj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gtxteewnj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gywgxmutp.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gpuyqtfrj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtaxjwsgx.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnfktbotk.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ghuvzgrtf.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gtsdqnxce.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gvwmuvvku.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gomswadlm.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gccrsqysi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gcuudfupc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gxprzhsmm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxobibiwh.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gropsrjmf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gzctvtwnt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwaskjghb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gqmeqzxkd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gyiauyehv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gkaunipff.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gdbjgdfzg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gkosnxoqo.sHtML


<!-- 参考信息 -->