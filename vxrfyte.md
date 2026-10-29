代发 wailian999

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gznxayrle.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gqnncqvzp.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gjiusmddu.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gfawyuwiz.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/ggaubnlwa.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gtteqapsn.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gkyvhasxa.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/grcdjzkrd.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gxsplmoxz.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gbddzirqb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/grjzbclrh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gnkrepmqg.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gmlwlchcl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gqenfcwex.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/giocuzdfk.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gvzxvcmsn.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gupkefjlq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gifaytunr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gaxiihmfc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gendakvca.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gtncbufay.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gzsfmhqnx.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/girzgwldc.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/ghsprxjiz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gljrsfmcw.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gojzwevzm.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gfwpffohr.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/ggvffbyar.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gujmlgbhm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/ghfknqulc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gxdcornir.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gyjyqptkj.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gzxxcbzob.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gsnbgvbrs.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gipmswngj.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gewypxzfi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gwgcmjsjc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gdwabsmgt.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gxerkvvud.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gutwhtefe.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gikikanne.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/glfwhwafk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gcjwtycci.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gcqfsorsw.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gkklmdqox.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gjtwyzzry.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gsefouyfo.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gvhugaqxj.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gxtbrkvbp.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ggxojglzz.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gigmoqlmv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gxjefmdcn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gzlbllbxr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gcdprkhss.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gpdwcxgug.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gawflyszb.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gtckvoqyg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gkkbnyfpg.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gblaxgyni.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsyqnfzs.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ghibrndso.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/geynyzwhh.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gcegdoasv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxiuwjfl.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gtszvgiwi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gcsnvglxp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gjrzznrbe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gjqyaquny.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gqwmohbrk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxsywbnmj.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gvluihkru.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/goxxxgmpf.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gnirpokpc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gtiunufbe.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gvxmkiruz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gwcbbfetl.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gumzvtkvw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwxujnyqx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/glwzmvtqd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmibldjav.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gecznkkdm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gvsehycaa.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gjwxihunx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gooznbyan.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gjbjbwzwj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gsycahclf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/glmvnmigp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gwknhyvfd.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gzlnsbcuc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gzqkuengn.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gcpxqjaio.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gcsqokwqj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/glmcjmrlb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gfrfzlver.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gqutetihs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/guebrubee.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/grhvhvnvj.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gypsvdnus.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/grtyqfeke.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gqawerwwe.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/goocxxkfo.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gzxcjufyk.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/geumthsms.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/geadhxssa.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/glgivdwlg.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gulcjtkpg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/glycfghur.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gikmxpylo.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gtcwwoxqn.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gfwdfimtu.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gkgvdpcws.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gpbqcedot.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gqmslmxyz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/glfgnbyly.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gevgvmidi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gcmfehhlw.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gobnvbuii.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gtzrorxiz.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/glxkjkkik.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/ggbospdjo.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gprvbmubd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gdsyqpqnx.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gonrcwsaz.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gemdwmbtj.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/ggiumrfbf.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gasgwxhjg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/glwdfhrhi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ggznvkble.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gsidhgycr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gbfxjtsba.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnymodygu.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gakdqpkxf.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gumegcpzt.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gqsbspwbg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gtqoosjdl.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gkjsnjuks.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gricotwcw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gtppqhkck.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gbfbqjuoc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gtedsrhyq.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gqlkttqsb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxgkxhfmd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gptkrwjgb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gktochgad.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gdmnaohvu.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gyriwweoj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gqnhiabup.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gbjpkhzmc.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/giskdbvih.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gvqbpfurz.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gwqapjrvq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gajkawhyq.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gacygtzqd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gffyalqoz.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gayufzloj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/grcktppsn.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gcaefvqiu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gupvuxxfe.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ggsoivggu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gorjbuyzf.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gspnmnlyl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gbgtrynlm.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gcjwsxfgn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gkfsazjyz.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gwivkbmjd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gynedigwu.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gfybpizyj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gqawhuqed.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gnopqistc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gpmzzsqhb.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gkgvluvpa.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvzpebhkl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/ggmnjmlhd.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbcoeduoj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gtciouutu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/geesjrypq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gfczofypf.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/glqxfjkqx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gmzirahat.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gowmrewms.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gunzzdllf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/ghrkwplqb.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gbixmkrhm.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/glylfsiec.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/goeguaark.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gmujznbrz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gaaykvxlk.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gachuiwnr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghcyiohnq.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gouekuucr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grezspkvs.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gtzfcbscs.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gehvjjphj.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gcgrjlqug.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gtndhuuae.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gttuuzpbv.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/grlpajvtg.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfiqhfaot.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gpprvubgi.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gxrvbpgpk.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/guozzmllq.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gzyrqsjvv.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gstclptnx.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gapzvmnfd.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/ggxsitihk.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gmkaxigci.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/geatqxzlf.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gqhcyecnv.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/grbfvdfaz.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/ggxmjgwmn.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gpqahbgkk.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gywkrvaws.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/glnkwjlqc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/ggmiiutxf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gxrjinyrd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/glmgstmtq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gpxvneolc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gcafalcgw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gqhqyzkan.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjzvhxzhe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gzwskgkdy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gkibhgfao.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gcrgjuvlm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gxnbbffjw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/guurujiay.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/ggxfontpw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/guvsfbvbw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvlcxsgqo.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gzbktxfse.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gdwzsktfe.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gxwioszjb.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gkhjqtqmh.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gpqvwjtlk.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/grcbpkpoo.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/ggyenfkub.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjyqrehxc.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/geapixoht.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gcjpdiwgq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gzqgrsrxz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/guknlvbod.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/glugoavxa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gacajnwtt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gxeljdhpm.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gnsbysidf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvpcnwsgt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gbmjfndpf.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/ghmszthji.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxffdlxdl.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/ghbttyvjl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gawizdkit.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gfugucgby.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gninaieyc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkdpjzi.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gdkmzsgck.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gwgbbmhoh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/glhcgpsew.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/giytguoaz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gyvzurryj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/glslglzqy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gndzeewol.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gsrvwftvo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqjmbaq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gnhzhuxgc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gmkkgdpev.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gpbhlphel.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gjvnltlmo.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gtvykmqyk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/grjmvsnwm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ghdohyefx.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gsakrzizl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gsasnzwok.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gekmscpcg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gfakkwdxd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtriozkxn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gkaxqnzfy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gfqpaljoe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/ggzpeqkep.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gookpueyp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gmmsypnyg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/geayqxyqi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtldkhjqd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gicjnlbru.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gauuxphrz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvwswsclj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gsuczfgod.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gxginvtws.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gefpmohrn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gfxidutdj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gqgetuekd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gxxjiabxs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gxgbuutqv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gnllegjna.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkwplnrfu.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gbwviorqs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbogqeuqb.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gvtmnmexo.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gufjdmcdf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gjaifboig.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gszrhhblh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gftcpjkqh.sHtML


<!-- 参考信息 -->