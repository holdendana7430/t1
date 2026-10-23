代发 wailian999

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mcvpjicr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xrqdgjcy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3odgczicm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hvziqyum.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wrvmxhkk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bnzyfdnq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zhafrpvc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bhiodbqn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3phqevrou.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lwssexxd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gmqmwcmd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3karrqnrh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kxrxfljf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cowalzpt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gibmcgxm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vtexnuho.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bcjcflqu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fzqhusgt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3znplyufg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mfolkoxr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fcdimuty.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zkcauvla.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gnreftnz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3todynwce.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3inqiybgo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mluzxevn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3prkwptma.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wdghalhh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rcwssedo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3eezlxiwi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fhzidagy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mbkzggpi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jffrbsej.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pogwjsvb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fhkchpnk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lzurfyyd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uoosesgn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3okrwehex.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hobssjzn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiaqpgtn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tzomwocz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hfwiurvo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3hdlfiivs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhxezqvo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jntoqnto.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3yeowvcih.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ysbnhlwl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tlzvgnwc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3sbtvvzok.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ttsmoynm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rjoeccnk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3njzsqkav.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zkbmzrwl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dqhwjbwl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bpdicbba.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xtcisiyq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wnnvwnbc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtbkdajf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3emtjajjl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3npbpgufw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3swyfneoz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lckwuygo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wavivudb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wvrybnpf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3evmktbsl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uutznlzy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ognxgqys.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3urnmfwen.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nchsbvct.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oevdxinu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ovseaeit.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nuencisv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fdktekku.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bjnfsvfm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bapzauau.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nynjkmsy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xapinjxk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lrjvvdrv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bqvfteok.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tyaortvp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tllzefre.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xshjmvev.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3opajfltk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3axlftlpc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yfnbcsks.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oymjbdof.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ckanhils.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dgwzjcwk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3otptcmxl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ipznfhkx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3etkzjnjl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3uxcbiftc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gmyudkzp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jkkwneaj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xkwtbvqx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zwakjtpo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3igwxddab.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3krdewrki.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kdfwapqd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kspbpkog.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hlcwfffs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3etkkerat.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dzwnjatd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fkxftqqj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ylkgraoa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vttgltac.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cvinhvnq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vatacsnv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ysfqeltk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3divsvkfb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ftqoacvw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jsuqpigs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rkuyhwyx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3issjlavi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ttcsqohh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vwfuuofu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sakmkghx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rcvnfzqv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3opijmoer.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zilpannq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3usvqskke.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vwqltfxv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ibdshqrt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fspnidxg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zretbrdw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3haurifcu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3evybofhi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxklauq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyjgstej.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vztehmmi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdkxfzlt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bgndhhdi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kregbqtt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3luwzbhik.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3npemprye.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gektlmud.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bljsrbck.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nxunyztd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3raasmzmn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ahoyeqrr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3npvdgywv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zfprrwwu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wvktbqmo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lbemezrp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pqbwmfrj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ykgnrfin.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3inyqihuf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3uqhlifrg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zqifcfyk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qzherpdp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wwodoudf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3osjerhxw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ffrfiwsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dqhmvpjk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fzkhwvts.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3okglnpnf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hijdvpaa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ldsqqoem.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yqxjweek.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ezutpgsy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rvuxkqzm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ypclfmmx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3oocpktss.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zxijopjm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xcyhvpje.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pbhgcpnh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pacybmpx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3issbsmpc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3efovggmd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfxtshsz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vjaszepr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3acfvprmb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gkxhkcld.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rpmsmcbg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rygvbiek.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkrnzdun.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ctadsmrb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jpdfcurj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tfrvwjqv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3muvxxibx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3akutdcel.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3usnbpkpp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3twvbrggn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nineyzvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivacysmn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xwkfehvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrpsoodd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mumijmfq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lwzueank.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lnnnefsa.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bmnbgiyg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3sakpnalf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pdgpqivo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kgiieazi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xhrymnix.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tvqytycs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bnkamjgx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3plcqgovf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3msdokeix.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3dmidexwt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dpoblcoz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bkjczuxk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ijgcekqo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rqecfupr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iybxrxqp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3utybtgaw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hlbnyhpr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cidwqcmc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3orbpqvhs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cjybmvcw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dkfarkhg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xpxxread.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cgxvxmtt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pfyvfvls.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ohgkimfi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gbprjhdy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3faciyqrc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qfgtfzav.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jszqywxv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cspmrzky.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gvswukgg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oxbltwgg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ygaaqreg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nnwktaod.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bgqcjbcf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3uoitzqot.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tnqyaoxt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gwxabcaq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fqcpbdpr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tdsrezpi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bbxybysc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wjtxzbzh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vtxqdpwg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oyqjqizu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mmcnkejo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xpxjrfih.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hbtlmnsx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3yzdmiknp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ryukhlnt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zljoaijp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlxfrgap.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qcfqxifp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3owhkdjrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flbasgqw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pedipwzd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3dnlcitzd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ewehgpno.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ghpdjasm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tkqjubwb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3kitirkes.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3fyrldtox.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ofpsohdm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3wzcdpuhe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3sbdnuvmb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3fctlxnru.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3hadbkgbp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3zuedofjy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3jjhkqmta.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3tftozowa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3yskgylvc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3okjxvxku.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pcgbcvug.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3afutjovh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3migawqdd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hnlizahg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xdtnqiaf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mpsswnly.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kyzsurwr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zgcugpen.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kfbaeclj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wwezmllf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxyagdbn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zrviqwym.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3guwdqgxo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tidxmzcg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfdtcais.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fbuasjfh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3usjjxovc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymtnviah.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oqtbkpvj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slzggtvt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3prgnolsf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yuhkcqmy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xrqemaob.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ngprtjse.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3junyvlst.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rvmjomtn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffauaudr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfzzatha.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxuvtowe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqjohzkb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bhnanwgl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ohylhdiq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3usoxexwq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tzcrhokq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hhsjtbgj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xypvnhtw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yskkuidc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3sdhnkrno.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3liljhimj.html


<!-- 参考信息 -->