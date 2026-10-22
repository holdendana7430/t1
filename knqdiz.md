代发 wailian999

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ggjkfvhk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wybmmgic.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xzlqhagu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2htdentfl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nahzzrlb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2uhyjqrmi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xdkmtqcs.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zqznwjop.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lodtsklf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pbvrecxe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vxwthndf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wiaowplb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dambdezk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uucmdpet.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2cbntqcud.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mcwpjzdr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zdlkegfb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2djbabvuw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ikbhixsr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cicvzasa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bcgafrcn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axrnotxs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hzlfoqzm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vnnegzmf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qdzafosw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qooxryno.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uunuurwq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2absluzfe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qwvbcbat.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2sapxfwrg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bploflvm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkmmfkxk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xqhpsxid.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2reuicqup.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pdoajmrr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2muvewzwf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2crpuxmdl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lqbveakc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nlhaytjg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zsvqehjv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2juircojh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2udrctogk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2barmcjqv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhiffgag.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ewcolnbx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2apupyzye.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hmwfhydg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hoondsrn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kebhmmaq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2idvtthlv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qbdsuxnc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zdnwawqk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2dyrzqnww.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cafbjsdu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ydyombwg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tkchuohx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2sigcufjn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lujqdksy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dezhfpxb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bfwhogvu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rojxpmys.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gciznakn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cddunwsa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lqwolqtp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vemcdfhn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tcccwdgp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ksaerzqq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2clcssayl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ydvxaeke.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tkainctn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jryrgmlv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2uiaekskc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mmgxacnu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ueadysea.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2flnkpdav.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dqjumhao.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ndykpqnt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pczsqkeu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tbvicpwb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qrrwgtnn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zieusads.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jxmhwppf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2veimpgvf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eiwlstga.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bzxmjjuf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2awdgtjol.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sdegpgmr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tjbtonim.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wumqpyqu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2makbuowu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2aiimivyv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mviskndw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kyeawhqx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2sioysswl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ygxvlyfb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvoilivg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2hplxewsp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2diexifcw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kjzttfjo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2eockwkeh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pgtbehpu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ykwwmwqo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xpgfuaws.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fyuoytbq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qrqwbajd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2baaqyjlc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ftpsnsfn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nwvmtvth.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lpbtwlbv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uacfcvuu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2soxjidio.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nfcsbgcp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2pcflptss.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dhswrexp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2psqzfbtf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mifofnsf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ghwmcpoe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dqboxxck.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrsfcajv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yeugkval.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tbrpmocs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2curcrplk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qbobdpmk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hqdioaxm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2stfkfcwi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mqnfskqy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gnmvjccp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bdfpugjh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wjzyqwzy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bzaxbkiu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ypuwmdjy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2etiseijn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lmdbitgw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lpqajtvt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pdlujkmr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ljflpmbl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mkawugsi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2dnbxlhag.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lwgzhnwy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ebwjnrhe.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2stiivehc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hciqvaaf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cwxwgcnh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2upyzomau.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bdfadqsx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pvtbvuhf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2teccbgyj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jouxtdbg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jayyycxa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uohrcmxk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2idbpwcqh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jzjigdmc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qcnfteyp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nxgxjzhz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pyzyogkn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2miycmvgf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jqqoybmr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ldpwnwos.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2emtvnift.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gmyzcocy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jesiwnpp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qjsirmzk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xzewnueq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oklknpso.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2svjcfhiz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wxjrafqq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2llrywthw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qcilplam.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2crvohcvj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ugpfbuow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hjhfeccb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ftrignfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpwjfirg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cdezhyyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cczlrfuc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xabersvq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rqbpwtee.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xizglbcn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pkqcejic.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2spzoqiky.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qhzppgqn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ycnngjim.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ysozccmz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zneqebvs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xcfkwcuu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wgitemdb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mkjwguil.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eftrrcfz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gbmsbxgh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lzwtnbne.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ffrbntby.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rowihpyq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rzoaehzo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cgpayymz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2urmaiwnq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xqiepgni.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2enszxgkr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xyzsbgsr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2npvzgvby.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xzjetqmw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wsptwnsg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rfaillbt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jlxukqsz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2htfvofzd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nsxurbwn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2efsmvegl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2adbxaogu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zfyjpwpo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yfboxbro.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xbleclob.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ttfusowt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yxdbonzw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2efcmcdkf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2sybbcqsq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eytlsami.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2oelxdhhd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2fzievbfm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2czjevewt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2oeudvfnz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pfschvap.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rimmpvsj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2efnuwrmu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2eygclqbk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ttijuihb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dvlfxbsi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vxdnninx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tagucgit.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pwhljkeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtoxsilz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2oojajqmi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2yihbtrsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dklxuadq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2imwymlsb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xchpjaud.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nhdjzmjl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2oywfydfs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gsprziht.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ngetyide.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2zxpidfds.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fzbqogca.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lcjeyreu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gilgyjky.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2boqfobwa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xyaprhli.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2axfbqiwt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rkctyghk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2motqkjgt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jaecofcj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2dctkowjd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uypfwocg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nvujitqb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2wlxmtpbb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xpzruzrv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2bceaayit.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tntqtomr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rbsowawn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zcmvdrku.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pmbvrxyr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cabamnqt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kulgmnwb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2foqnwyuu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jbdbbvnb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2efvzneww.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldehpkvy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwhicksv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrbovizs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyyqxyxw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rztcobgs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wvqlhmxd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2melzboyc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmndqflw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2trwlsxsj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pwgtyapq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dnelacln.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dxcbfkfv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rwccjphp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eggopaxq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2fdmfsxhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktmzoqgx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lwnufhku.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zptarbdl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tfldhjkd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vlqklsyb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2qlklrozw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wutakguk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2stqghfqg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fqezzmkm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kvixxlcn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2uikzzjcf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2klajzgyt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hwqhtxqe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qrtalick.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dvudjvxy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2axtrhpsg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ccmrcrdl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2csfqouoo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2knsosjgb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uxtxcrtf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2jmelribp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2frsvguvk.html


<!-- 参考信息 -->