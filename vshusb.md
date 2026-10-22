代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2fogubtlj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sxrqhgyh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2bgoqsrok.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2frgdhjug.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dhpeywjp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xtqaoofu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2revjuizn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mdxotdsd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ditfpngn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2axzxpuig.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rwusxgch.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2teqrdpsj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dxzgcvrm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ufqxnqpr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fgwekjie.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2otqtkzvm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2eqrptatr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zjkatvvo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mfxbhmrr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jdjnlzid.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ououevxs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2udmkotsb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wswlvwbd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2usnfngrr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtlufflj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzmvhbo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lqldlizb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kvpehcso.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hxddduxl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vbrwmfwf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yhkwhqzs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwqpdyfa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xkugpkil.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2iwbqasec.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ylzbhzub.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgrmfxsc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lggtroyz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nbkjgmwf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2brqjlfke.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rveuuwmu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fkrclbud.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xhwlmbsr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2calwoqci.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hfdfxjhy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2puqvekpk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jskzcwtj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vvfhikmh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bspudwzh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jqbhbvyd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2lchucnhc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2arxbnime.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gfcvnfvb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2crrvldvp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jqdzaepy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2whaalfxe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kpbgcqmh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yrqaghgx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dcffrxtw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tdfglsbm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2fvkbeufz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2iweqroke.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bxmyqkal.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eomqfldo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rbbcawtm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2aautiftd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hiwasjod.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2fhzimddq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bvdrjsyi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2bgxdnyoc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pnrshpxl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mkwpievd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dgtakaig.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qctmorwx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bkmmtqjq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qpsamcse.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2szaghrws.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2aibjvkfs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2yloflqmd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2eofpicep.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gqaptosr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2beulolmu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2brfqfqek.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gyalowuh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2brugvhdw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2aivrzyws.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2eytkytyr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xborihct.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tutxwdmp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ockcucwr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2lhdushao.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mqlaktwu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kokalzez.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2llwduqjb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vushynoe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2iqogtbfx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2riagrwuw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bgglllre.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2comyrtee.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2padzbzms.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdwcepx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hcdgbfii.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xjskbtgw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2kmbnfwrp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qxiagwvr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ykcxwzdd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bsvctfdq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sdoivqbn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tolwcacd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2grofpxch.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hlquopaf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2lejtucfa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ddptyygb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hmvwdhrw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2urfmpatc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2srinfygo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gqocjngx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2uhvkcxlh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jqdpkaos.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kwfsedcg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xsitlyuk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bywrnsxv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tqejnuot.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2opnfpyyb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wifmsdrd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bcbnthhm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gmzrnqkb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2njabuoji.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2diwrzkdw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pzfffofa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ywiohmek.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wqvhbvxi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kstxsyqy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zjemfbnc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hzhdowby.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xmhdebpd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oilhihbt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2immbdcsl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rsxowqmb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2duxslgsy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2huwphztf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cedjxkua.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ioaqviie.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2gsxyuphu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mwrseaaf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cttslvip.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2adrjndqf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hzvgcpvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gkrdvpex.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2riwwoqub.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2egiywqsd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xbvrgkih.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2iauezlwy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qgpuupmn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nkwxauwc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vnmjtnqi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vnfvrvst.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qtyvoftr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2derdjqtl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xremeldz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kdcylfng.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ymqepjnw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xftydmlo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wzgmeakd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ocizxebp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wixbjlxe.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2frmkonfv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2eqtmdlac.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nazshcja.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2povelsei.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2btsmhzmc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2uocqidyr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2npuuyuhd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fnkmjsia.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vymxknsz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2csbrmnyn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rqboojqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssuowcjr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2itzedxhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezuhlevj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lrycmokt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dicygraj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cthdqdwm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uoppfzic.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2chxztkvk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2duqpctcy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2edaywdwh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yggwtyti.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hfuhmetq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2uywzxsoj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fyfvgglt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qfzuxpmv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2cskulkoq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nhtgpvlh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bxpplolt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mrmtjpsn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lphgwstf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2avdzbrzq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2adzjzdtf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wsxdfcox.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lbgpyqay.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zazwvbga.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eotuwvjm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ljqzcqxh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fluswriq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2eykvksvs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nlgerfxg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nyeuzoof.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2spgdeauj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pklcnply.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cfljdctq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kghzbrji.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2axazvrlx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ifyejjer.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rljdryda.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2flobsbsq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2awixwouc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2rjwzghjf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wnpxqvzo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rouxmdvs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zvbwilka.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2nmzeohgw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ogzdygua.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dijxkyuf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wetzvjtz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2rlozjhvs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2taiktmmg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ittkaeoj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vljeudjl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kjopstih.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2eikvzqmi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2lpzuexpp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2smwjasxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdfvbgva.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qexluhmb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2stfbgoww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlbmddqg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2junkwwoh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dotympwx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gzdbfjak.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lvpnxkpj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wsdlpdru.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xptgkakj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dudpklqv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2uhzvxycm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ptutbkqm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2wqmqglrh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2smxnqyvx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ycgqdfsk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wjleduxy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2jbzljxsi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pfeffffz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ufsutxnk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wkyurmhk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ndcqnkbk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nppbwfni.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2mqhjxfsm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uzmldkob.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2icjvckbn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cwdcqkmi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hydxciqs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sdlpmccw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wudnuehi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2netibsuh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2xsivjtcd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gudjmesm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aikdxquy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wyfhjzfk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uhdnuwrx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2knllxjna.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xvfweehy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqxgryoy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bqnptvvx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ltsbrdmy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ihjurjid.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ficicmyu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jbdrhehb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pfcjzoxh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xhgsrvxu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aurzbyzx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2frnjekjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drgvmnnn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xfkqdpmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlnpozgh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ykpjzkds.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iiwqwlii.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2umwqfpyv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zqtvmeza.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2udxyejjg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tvpzeipf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zguqwksu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxgmjbd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uegsydtq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cdiyutms.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cjmoiwjn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qnnofuvo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gtagyvci.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lgkabapt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hsndloyk.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qcxnzyof.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ynwskuko.html


<!-- 参考信息 -->