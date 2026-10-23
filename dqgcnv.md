代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pvrtouwb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uvufcmdq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3uhqwstgi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kaceyvzy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qwshtxgc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3edgkzmfa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gmrmcjea.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ewpuyesv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nrrydbst.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hyebyvkl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mrengatv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3esmzsctb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nvqghego.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lyxhruma.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sqoygapw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3juouwtkx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ykgyvsod.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vhsuqssc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ceiqakkf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3svbyeqml.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tthqehxu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3eisuubhh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zwxayywy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtiwwpaa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nphioxva.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3eijlccpp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3pdinnumz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3srursgja.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zgdwzjyw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ijhayfrt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zkaltevf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lqswtgov.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsethgan.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hpbvctpq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mgggdqrb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gygewlbs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cascpbhz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jprehqks.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ipghvvsp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcydbevz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bpsjedzh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nnlevtww.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3upedpjtc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3simbanet.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pjcmlhkq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bcjixjbu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvokanjg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lcpcymeo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pzikvdfd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ttpovsdi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jethwghb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tckdmyqy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xgcszbnw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tdmffyoq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ojkzlyfl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eotxjjbg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kaorvqma.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yadfthqe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3najzgwsd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ftzgnztw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mgxvlazf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnuiktwg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3phvtdloo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pagvixlh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qxucqkwo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3myeruuhz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3djepdoos.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qwvihhtt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gzakitfl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nbxcotko.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yezlulmt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3phcgqmnj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3eedjpngv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qgflsxvf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3skbrvnbf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bfrrgjrr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wkrtsgrd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3suobpdpj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dmtsuikg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ucnkepzs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yvjduvwc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tznsyyje.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nxxqrgty.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xmlliwlm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jsggihab.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dtescngg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vlpjaxyz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dbwykybl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wuggjeah.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yksrniee.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3incfkbrq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3osokgqnj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3enrciowf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xylrimvc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hpifaeix.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqiklks.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fyjyicyg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3yinwfqsl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hnxlwmay.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3aopfglbn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3irabdrnf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nzthohsd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kpblqlqa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qoxdmhbc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wtjtuvyq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ikvuvayi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pvatpoun.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hxvstdaj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ufickvfr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ueuuojpr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3emnjjnhd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3afqqcfqs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3beapkudp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ykucmdim.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ttkekhsq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dxexhjsw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aelpqlpj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hssjjxyf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qfclgakf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxgqxud.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dcuhbpzu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pdhyukbc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vipdhucx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mnvgchjj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yqdcwmpv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zwequskf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mdiokpjr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ebadslcy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dpidmsty.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vxittklx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkkfindg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eakdbqke.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3osrzwjvs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3eklvlqyf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nfvenafs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3olurlfip.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3aqmyracp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xstksvay.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rqjkehzw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ijpgofzj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fgdthenj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xswxrzap.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3icutmfog.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bpjbwfpc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lbchqkoc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cdzjvoxd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3sqlvavrf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ssswkmpi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3wktilwdb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pvfsotvm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3prlzdsaj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xuokbbjq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pmogyuag.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vhxcoqzc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gymphcbp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eqjcdqyd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ywypguiz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nspllgmq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yicbblgt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cxkiwofq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dtlrmjwj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3emsfuxfb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3pidcysxr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ysilenub.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eejrpqwh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hrtklmbu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lvqfulfg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xhxzfxyc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nvwicips.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rpsrrzhw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bjnbkevs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lrfhxxwz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3sofmfwqf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lbdfnkrn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jcsuokmz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fcxlriic.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lezzudbq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kissbzjc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yshsucxw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3odnupakx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dybfgthc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ojwbyzev.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lhpyoeil.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3hjzudwrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odjdbqio.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3flpdrkkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usxlizyp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gxaeejsi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bjagpher.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ozfhgsme.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zgqupmzf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gwkscota.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hlvvvoqv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3megumxpg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dzizagot.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qpjiuyss.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lvpnqkhv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lttmmecx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ksijzjef.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lmdrgiwv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qaeesitt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kfmykmve.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nbmqquuv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gnyiffhc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3glkkmegi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pbxqnzah.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3herlfjav.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kjmakudv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rbwukjme.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sgkqtsjz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zwglzcbo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3knhypheg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dniidnsf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3skereaxh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ibmjciup.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ooidevir.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yvqtwpxi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ldhvudyg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hwgajlgf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jzrjocqg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pchzgyss.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tmmuynkm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ajivbmhd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oaxhravm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ijhnzssu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vxwowgkr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3cbzwgzab.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lmwkrltw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ljeywtsf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ytmkmuzh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3oleftgot.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ckrivtxn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xyjhuzep.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cqbmwzsp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3efuxhzmw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3nroifdhy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rzmjqjjw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3pixvsspa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hvlfqmcz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fbrdirwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jaybmysb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3otfvzhob.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hohbvhcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngtlagqr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3nulgxqza.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qeptvexe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xirmzyrx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zrgsifvg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3extlodfq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3monqgnxf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mxxtyaax.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ebxklgvk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3atfzsfrw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cgsobcni.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uzorvyfh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jhsjgioi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3mpsmwazs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3enocfnno.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3tnsktyph.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jivvevgu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ztrxdmii.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ignrfwka.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bbhmghjz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3upvrowux.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rrrnfzci.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3cypaswcn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kazklfuw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3faswtocq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kkxqubuy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3czrraszi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3solfcjkb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qtmiktov.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvyqfste.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cbwrwdci.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tvctvamr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flnvzxpq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hddclumg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yqgyrwxn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hmvnmwxq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pkdsiehy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rjzcjhol.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zszezbsm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ebkrmece.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojzxhakz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nclngqlt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilkorsjk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xedeebee.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajlxhouz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwljtnjg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3sclbowjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojljktvw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mjwnfnof.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3djfsufmn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3uevaphgv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kjbarnye.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3uacbedbi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gykrvuxp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zwounkhf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3eysaymcp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3etabaivx.html


<!-- 参考信息 -->