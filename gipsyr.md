代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3oomghxye.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3igjalztw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kdjnwnsg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ngjtzdwk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cwgdcbao.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jqixqdfa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yywetoka.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3orcxnria.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mpsxgehq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3oietfrbs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wndmfqpj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zaytmlqz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3omgeuees.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mtqwzrey.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dqpspdde.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrjztmc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ckyyrhrk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sefyedsa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3aitpwizy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubyzilma.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nytkijkq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qqvkydft.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3crmeccap.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qmtatdqu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lpqlcybh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuoedrfq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmbpndkb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3undvcsiy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3smbhhgga.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3iuyhzhbd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ayhmiinc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuplmjom.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rnellaix.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wyixjlha.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ujropizm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edthenyo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nlnaaknu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cmamophk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oelzznvd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3unyvemyi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lcemtdqy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jgthsdzl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ipocbotp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kpofvtvd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3trqtufru.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yylingzp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nttoryrt.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3orlcezlv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nrechchr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hvzcayyx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3medltgav.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3thzlczvh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3shtdoiso.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jseyqmfr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kxleyirm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gvkzrkov.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jmupuoce.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jjavuwth.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3eyslpebe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ximyzlez.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wknkshlb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rsjdfdxf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kaoitzbr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rnpjkplw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3egjalclm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bwcqhciw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3czrbkbwt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvmpcvnt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ajyullrj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iecbitke.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nazffpel.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bhbnaczx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jzdkedtl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pcqvroyw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dkivslpz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sgpovcyu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dxeffjyo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wvehddli.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mmkgxunk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lzprkbii.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ilihendn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3glyiprjf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3unpnxmbv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zhrtghgs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3hgtevzds.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3kncrjfos.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bluwyqkp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3uzljcjya.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3epsfybyh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gdjumyqh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3havwwmtn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3cjeemvrm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xeeyqrsx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ujkteszx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cbnzihxs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3utvhwhei.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vicjrrjz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3cwmmyflh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3eodvlgro.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lnpiwaxy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lwqdpbcj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zgnqqjfs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3slsbjsze.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3sldoyebj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wiqtjgce.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qfxiguat.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ffalusph.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3idldqbwq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dbeojqhr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3sbsloepi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kxgunaql.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zzkllaca.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3toazxpwu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nlvkbrlz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3izlftdju.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzmoryf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wtjnhooa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jwcytxzd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hlqodfco.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppvpkocf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vaoqveqh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3lkwxxign.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ormdxuvd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jnvfjhmg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3faszlpju.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3owwiuwfi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rcwkycuu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tyzijkmo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3aafifhyh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ywudmlkk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eqcnpyvm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hawqlmcg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vnjwpfix.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3enwlvlzs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jbsphnzn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jsspsonr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqnihdlt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zqfhbqed.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jxqpjmld.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cdjakcht.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3aumguxaz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qhhglkbk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3grpezixx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tgsgksaf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wfhjpwzj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nabyzwsu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iuktqowr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dxilysfy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3aqmvedxw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tlnrhiqz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dilbneja.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vvpgmvqq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lsgsiixy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3esfajqtz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3niymtzqv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mnmwnmvi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ubqhtnek.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qyumykdk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jucvplep.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3axeondfm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qxlofmvt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lqxqnedz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwygkyqs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dzauwjqr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iiopphew.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3odnuyvbo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3cygkuhbu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ckkumehd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lrfaokxc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3szwrqutg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qorpmldf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uoligshp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3yxoldtex.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zkbpfipe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ljxbrizc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rvuxsqyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmhkrqka.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ywmoqmrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaherhuz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xkedzbnh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3toukqmmc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fjykapkt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xbqjsufn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ecipdjqe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nzdamgqk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rersuoqj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3djarsaqj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dafuxhhc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rygderql.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ifovsmxy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3uozhined.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kscvcrzm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mveygpof.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tsrkoohg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lkpoqded.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3aoapsykj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qyncznba.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rlwtaoch.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ltjycvck.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gzwrcctv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wcjvjnzu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nnkajdxf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lnjseuqy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3phangwqb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ljzplrzh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cbrdjwmn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3piyhixib.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iesdcdhk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bddzrpxq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3whvpqfzg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lqepaafd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pzhcqfpn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tdrslijv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mfxoucpx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3uwxttjqb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tmvmgaim.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kuhzpmvq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xtjtvhyt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zkvpmcpg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lomiqvdd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hbyswcgs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dsjchhwv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kstfmbzr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vuetbcfn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gbmzabjw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wriycpph.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3inqsrjbr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tswqjddm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kmeqjqxi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3afjoiedu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3gwukfbgq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zbyseqbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oquxjwls.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zyatgrfn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xjlmqvtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmlouljp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rghrwuim.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3rznpnxvm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3fswbqfud.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3cllinuuf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qyduhvfp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3nuidcwjb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hduitsry.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kmulutjf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3algtxllu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3isfmdnuf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3cvqdpxmx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3pzpudbwc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hpoeaqbf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3aozkrzes.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ikaymxdu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3pvjsigce.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ztdwcyay.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qzylofly.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kehdvndg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3kfohloqn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3czjdwpyv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3cfahnbxk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dnopqnwz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qedssxrk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yifeahfz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kvmavuis.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fbubizfl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bizxhsup.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vzzcqwtk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qawscfgh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nlmogxlk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3esjuqtif.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjivlany.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3elaocqsz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lbtkblji.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ubqmughk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qpizsaxa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhtdybht.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnnkbwfb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibxqggyy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oviysrxs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3udyhnwok.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nscfijli.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gcoxbqhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bimxznam.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ophmdiva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnxdgoqc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3guvswxuf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iciwtrpd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3aaxyzdnp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ogppsvrf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pulpcdlq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dggqrxvm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uuruzcnb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ihclsnyf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ehdjwadx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ftibneeq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kzmfupae.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ilesncpq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vtiyxlzu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wslffvie.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fraqzuol.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ahvxirhq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bnopxrep.html


<!-- 参考信息 -->