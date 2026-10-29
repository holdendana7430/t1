代发 wailian999

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gysprtvhd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/galclvkap.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gnzmyalyc.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gkiqfvhpt.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gikxvlvpa.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gqgtiqyuc.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/grvucnyub.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/ganeekofr.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gggwifrsk.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gvcttwcvq.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gjiztjvtd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gnphkpyey.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gyfclkunx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/ghtfporkp.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gnyfcflfd.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gsydbuyfe.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gotsmedrs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/ggqyrzinq.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gsvtoqsjw.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gkhbinpmj.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gyjavyxlp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gagmggnvt.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/goqtwzrzo.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gqflyzixr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gkcmohadb.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gnltwuqws.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gqeuomfbw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gnrexiwfn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gmdvhfpej.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gijnpntzh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gjwfdgkyj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gcgppcezz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gdhvkqfrw.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gxxkrhbyn.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gtnzdyzab.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gnfyrdwsp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gqvdepmox.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gjfnuoeft.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gvvlvahqa.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gxnfhdanv.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/glvlzxzdn.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/ggrehkrxz.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gvgjhsemb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gpreswbbb.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gxmhkbfaq.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gucvsyyuz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gypsrlskv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/giluijmbu.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gphvfczdv.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gltbkqxtb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ggucrgjql.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gonuqdbnd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gkgykxvjf.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gscvlxuco.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/glmtaorsa.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gkvvusdxv.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/goxxflxms.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gfgjxkcsn.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcrycuq.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/glscnsgmd.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gppwfefvm.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gosqkzjbb.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gmbcwripf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gopuaxsqx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gaamisrqi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkhxmzywr.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gbrpehzto.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gsnsvasol.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gjpiydgxr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gufxovccb.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gbdhxnfhh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gsrbhfapb.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gkhcfcxua.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gkrzvyovz.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gapxvispy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gmqvdehxw.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gonlanoyy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gicgvonbz.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gfspswexl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/glpdaabny.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gtkehjiwo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gardtfhvz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gzytqsjfi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gvbjzzcvf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gnskxvwdo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gyjxwboji.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/glyrvtzbk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gizhqceyw.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gcwzmswim.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gyxvtegjz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/ggyielgll.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gqihsopno.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gxqzckvzx.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gwstqtkpu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gupoxnymg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gsvyamlno.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gvudofklj.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/ggficvddw.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gpzpdlbrw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/ghmfhjbxe.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/glwdptctd.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gjswcncea.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gzzidsyhu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gxgzwukop.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gvjrllmmf.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gctuuhbxb.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gxbcynvaz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gatzwlxym.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gcwhwtxfa.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/grhqyenxb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gmuryjgaq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/ghutscocc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/grccwxaws.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gmegyejos.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gxzxkatrn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gqmkrpoxw.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gbqdknolz.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gmrsddesz.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gbgyrshix.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gccbnwcqm.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/goolvqqjt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gkqjqyutr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gyeqzrbcs.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gevzlosqn.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/giirgxslo.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/goobbkomh.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gaialrjho.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghcaqrdel.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gjmbtnyla.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gbgkuxgww.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gmsxolkol.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gpjjhoabb.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gwcgmrrjx.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gwaokydal.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/glmglyuou.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gdiprzkwv.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gvgqjozbo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gyrelmmbe.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gtpwjztfn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ghkxuoplh.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gnflecqpo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gecmdbtyg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gqnyvjmiv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gfpiyuhuw.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/govsligps.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gnomfiwqn.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/ggmyceqgm.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gpgqfufal.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gmfywsepr.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gnjqwbjmy.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/ghxtobqwy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gwhyqinut.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gycvypvea.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gvqxybvih.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gggerypyr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwiqnokqv.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gqxiemjmg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/ggynxxvhk.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gwvmmsvtt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gmhwshdic.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gebkymbyv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/genhxqyuu.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/ghlzywhop.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gqnjbtwgk.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gcpmhxkad.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gkhlsqqif.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gvlpmcgej.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gtrdevbjg.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/grabvbcpb.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/ggapjbfdp.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gppcapvpo.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvrybmfvv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/giqcrkvna.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gccqiuues.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gofviwcpu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gceuennqp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gaulsylit.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gltlljqqj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gixdqdnsu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gjgvobxhe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gqessoimh.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gqctaiqnk.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gnpjdrozc.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gwkmwvyjv.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gmoydzmlq.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gbnyrgrjz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/ggvyrsdve.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gydgqklgs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyzueyxar.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gbffttmgy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggnxiulto.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gxyqcikti.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gcmdzzqmc.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gaddnkynj.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gjoljgyxr.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/greafraax.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gxehdjdrq.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/greeznuck.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gyrpooruu.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gzhssshqh.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gvfvsmifa.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/ganknivjl.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gnvltzefb.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gzelqmkgs.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gtuhhdclf.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/guufsqqky.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gkhqajoiz.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gdvkiiyhq.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/guskoohmo.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gndpisohd.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gmqgvetxq.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gzoochwsl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gzjfdjblt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/ghsvixkqx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gefoxmocg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gmiyahrox.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gzzlnmmnh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gjfvqplko.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gzccgecgd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gxfxwsrnj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gijcxfhzh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsltdwljz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gsdmiowfq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gcxdyemkv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/glveyospn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gordjyert.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/ggtqbsegz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gshjoftgb.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gsvrvmtwo.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gerzinaid.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gqnzordvf.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gcscvusyu.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gnkayvehu.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqmehpfes.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gncidhdvl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gjdftucag.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gbabcezpj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gyqdxdzre.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/ggchpgkgv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gfbynpuqf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/ggdyyswmo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gkxozjsna.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/guvgnnujn.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/ghewhzsfy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvwuelcon.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gaubpnoql.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gyimwdkec.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gohvmdrry.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/glvugqbsx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gpqoetrpa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gsnumprpy.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/ggddlmwyh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gvciudqhd.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gwgwllxqw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/goivggeks.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gstxtuofp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/ghtwfyfst.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gqxcmjoad.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/goctnpvcw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gtvagtsym.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gbcrtjnyn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/ggwjjyaov.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gsopyvnlt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gddexotkz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gcyzhdbyo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gzfzpoifp.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gxxdnryde.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/geqmaffvl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ggraqactn.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/grehjmbwn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvkldehxi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/grnbvxqbf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gvzddsfry.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gfpwjtcvl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gyzqdafio.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gkietzoxn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gsyesvzon.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gjojefnef.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/grwdrqelr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ghjvhjzoh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gqueilczt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grykjivzt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gnthhxxaw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ghkicmwve.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/govmypoyc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gygzoognl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/giwobcbdj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmphxeexy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyjgvmdos.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gqeoqliwb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gcncxtcqs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gbxtzetfj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwztdviee.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gctfwvhbf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjelnxnao.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gpmtpxuxi.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gkmuhjfvx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/grgjbrtql.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gpjqlkpyo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gpjucxrji.sHtML


<!-- 参考信息 -->