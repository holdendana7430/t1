代发 wailian999

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gveagzzpx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/ghlbmsavp.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gcgflyfjy.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gskfjgoif.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gjsashpov.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/glscapaiu.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/goowvqrpb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gmrydgewv.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/greexyoav.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gualayzba.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/ggpgatawz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gozkptfgy.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gybxbbvcn.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gkfcvoccn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gxolxcosm.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gnbuwfrcd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gzxxqpkvm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gwnvmamsa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gqcwutdpx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gejxexyic.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gjbstmjee.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gxowouqda.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/govpiswsl.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gzkzzsusw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gnpzrzhpn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gusaemcdw.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gkeehavid.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gmpotxygv.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gxymsgbxk.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gnmacmalw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gxglzqfdb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gpsjsvcbk.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gecuvvczy.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gnybcoujw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gsocomgwm.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/guhlwhowi.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gcegezewc.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gzrtdjqxl.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqccmzeay.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmtxlen.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/grwmzdevy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gwzfbmppu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gfveeifcg.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gontatfvi.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gowbdvkzo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gobtthkax.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gokonntyd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmkvylnlv.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjghjklgm.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/glgtapqyb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gwhllthhh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gvdbnoyji.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gyvshsytp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/grykknben.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gksmmpxde.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gkmaiiwho.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gnuoechyf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjrzjacbq.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gjnnbmpwp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gyqqaojxj.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gsiksquvf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gavprfiwg.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gvtlgwolz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/glpfjrzmx.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/givzavhcc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqpxqdyfc.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gbpuhvfzz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gvyaffurd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/grujfjmgt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gydeodsjk.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gqbuotlfi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gqlkirlfb.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gbxfbcnrz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhtkqyr.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gbvrwrasd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gwuxlelrc.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzriuwrtc.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/ghwjxfeoz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gwvsyrwqf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gjbutkiht.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gdmsbjvxy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gtwwoysqy.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gulhdgjbm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gkdmbabmr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gqksaqbdi.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gsfwzmdkf.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gnydecard.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gllwywqoe.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gllowrkhh.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gkegsthiz.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gajefbroy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gmghnenoa.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gcezevdcj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gmosehosw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gblmzabkf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gvhskjsvc.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gsbzkuamw.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gymodlvrp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gkuakftdw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gfegftuna.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gcprylhka.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gbbhidqjp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gewjlzrwa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gwconfuer.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gizljfvhz.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gwrenqylb.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gwqwugqrg.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gacvmwfig.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gvgctzmze.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gqinqxovj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gadyonvfq.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gmectpffm.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gziqdmfdd.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gdprldzog.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gypkytgqr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/glmsfpybw.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gamweduyu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gaklxgszy.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gppcwiscj.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gpqvoztuu.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gyskhnkam.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gymflxevw.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gbythiyvz.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gycrmstkv.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/ggmksannn.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gvbenmgfs.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gcwycnfew.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gqamyaoxo.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gzzcwyuwc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gpiocnuua.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gaektingo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gtniboieu.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gkuzfcfsy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gggyafczt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gockvdhfh.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gzzaquaeu.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gmfnaypbl.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/goimaodel.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gytxbnmqi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gipifrekb.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gnkgjexyq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gmpretojn.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gsyngjpfm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gllbjejki.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/grsgciury.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gptzzgglm.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gdlygczbb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gwvkzymrz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gnrimalfa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/guamwpclt.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gzdwjavjc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gvsuvyaux.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gfjvtkcxm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdruiwewu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/glregezee.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gdbwsrhap.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/ggwzftlem.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/glvexenmy.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gjqfixhfg.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gemvjszmq.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/girnvuoet.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbfisinyi.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gechwwtos.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghcuoxyzy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gteofzagb.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gclfrqlvw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gncbrktum.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjhlgrvcs.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ggbmeywlx.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gabzewcnd.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gkaglwzjs.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gaskpcild.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gjgkgouip.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gxytuukmp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gblokjwdx.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gkwhhxpcs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtfbymhqn.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gefrcpaoh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzmwnnson.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gmvspheps.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gjahrjfco.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/ggbffjbxe.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gzvhveesx.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ggaqdowrp.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gupdhdupo.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/ghellkxto.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gfcszcpdm.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/grpjvztbw.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gdznkysli.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/grfnnwanu.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gerzublut.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gygodphmc.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/giypfaeoz.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/ggdacvpaw.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrtinqe.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gmezpefuv.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gyaulsqrh.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goyfhjskt.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/ggbzbkqce.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gxtoazbel.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gbwbqbbnj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gnkxaiqjt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gdjunoqvk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/giiozcglt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gdizimunr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/grrktzokz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/glqohyiez.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gkczpcmaw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfbzmqjbp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/ggtxexifd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghgfoabob.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ganpgbzqx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvjlmxtro.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gfohglccb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gasryzhul.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gyndunycd.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gyfppsehm.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gwfzdbtub.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/guqihqjqo.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gmnghxwpt.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gwfgzcywa.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmnifsouq.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/giftcndiu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxivbtqbk.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gmoffwvcn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqndwvyvf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gfxibbvcd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/grotlgxgc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/ggtpmbzdl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gilzhtlsv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gxhsmmlqi.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gxqvuitaz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guafwgpdg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gsuybnhtp.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gkhjszbmk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwqwbpovl.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gqceekyod.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/grfqzudbc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gjhznzbvp.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gggfcnmrh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gpavjbljx.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gpxjmdqxc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gihvlvbnt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/grusypwzk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gfnwgjlas.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/grcmdwhra.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqpvxgd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gezlurfjx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/giyoxoatx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvpsjgf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gevwjverj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gxghcofae.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/goqlyvibk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/goyynrjbt.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gxdqbcjfq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gekphndhh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gdwunibdc.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gevrylmzz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gzjbbuxlj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gqrbwzgdx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/giheuiikc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gbqxuoqos.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gpcdrzuzf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geetbusqs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gamkfmzdw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gimrjxppf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gbjdefusb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxfhsnvez.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gqqlhrcsa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggwwckkpu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/glrsfvtwj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdzxbhvfa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gwxqhoryw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gtktfjczq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gegafhvdz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gbleevqkr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gxggtraau.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gcfjfyxvv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gaiigpsoh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gxxcxypfj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdktldzsr.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gdyyjmgcx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsaeffqdt.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gttpzuziz.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gxchzlwcr.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gzrryxhyc.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxnjlimbx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gujlyipks.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gsyryplwt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/grymdffce.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gwqctnkyw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gtbsmxrpx.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gwbudtrsi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/grnrhrysk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gdqxxowdx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkwpmhmc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gnxmycrqj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gewameqhj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gqscdaayp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/grakaaxlk.sHtML


<!-- 参考信息 -->