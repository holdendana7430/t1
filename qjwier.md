代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pytvuqgs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lxdoqlup.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2senafbjz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfnvkpy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zcfmrldd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sdcsdkjn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zzhfcgtm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xujcwuai.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bjdkjxml.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lxkhgerp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ddqsjiup.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzxbizg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xhjmxrgy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aigoypoz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jsnsyuea.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nrnrghuk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2naxdwfut.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ijzhefem.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iiduqmeo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fdktjvxa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mbbdwycm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2grhrnpoh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fyooacyj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lvsdmlcd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dmxibyrx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vomehuoo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2grvjljue.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wwdpkqei.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2smsblutn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2guzvjjjx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mcjslpid.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxnooaiu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mdiehlmv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zevcumph.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2osrtnmsg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ztfltetg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2whwgzcjg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fnwdhkjb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mlqvzlur.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpetnfg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjzawnvc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrhinmwa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hbtgqzer.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2uyokqqpz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tlwfvdmf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xzutdrrb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qljrudvz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wlcfdmny.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tlropini.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cvgbfizg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2aedfctdy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ebzoivpb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2korfnsha.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xvvyefdi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vpnqabag.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hzmxgeml.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gizwhbsb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zdmoafru.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2yhzluerv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wcejeyfh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qxgiuayw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ortdvbla.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lyidalxe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ejqrnazb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xungykur.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnlcweal.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nyizgihf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ginirgab.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cxgswhyh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2manohcah.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2pvgiedfh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gdcmdgwc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hynkniqx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cyfsbetj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cxhcsnum.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gboevdcy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cmvkknxh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pixwycwm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hhjszomb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ulxmhmft.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxntqk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bgoqcqhu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2katamdfe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdpgtub.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ebabntpr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lekcggyv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dgwahelb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2axpwjjln.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qpyuhawc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mjnppyja.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2voussgpq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nehhbjfk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dlufxmcm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qlajazof.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2egosqlnj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gauoclhr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ziygnkaw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjspmmz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ocmbmytj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qgmamzkm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2clunpbyr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vsgorbkh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qtedkrdi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtdhtou.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zoiadocx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rslwdrom.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ffokhieh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2uhunorei.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uuzdlpol.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2yimjtsiu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2luufsltl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2doodkiyp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2uhhbfgay.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rvpvqvom.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2lrahvxfv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qqxtwlql.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2jtknxnqn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rnbvgivh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rodbtyqy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jugvyawa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2htaspbbv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yxqkelqj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tfgbitps.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ecooagej.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tioqggqb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rjmewooj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dvoosbsn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fykrxivs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ukracouf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2faspljzr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpgktdac.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ezypxkyj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hywbxihc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2goszohmy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2knwpaguu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fynpuvfz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2strgmzox.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ktiiomyf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jnmxuisz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sorqsucw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gfztvaen.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kyufhdqq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xhzqkynw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oonopczk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vboqtecn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zbbrntak.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2snkxoovk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rntouwmw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ygsxycka.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fmrdjikf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2nlxjumtd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2erbxohxi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pfwbrgop.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rgmexado.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2beppxjbv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2rzgfeppp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2nttcznxf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2brpyvhei.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ootlqjxj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ednetyri.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xswdgrkt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wtsjspug.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zurrpqjg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xstlavig.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qfuihbjb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wultrysv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lacfnjso.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kakarvxe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bvomsnov.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxwtffw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vztbofuq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tpkczxcx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dkyilebs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2holshfgq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2thqttjyt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxhiczsi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kxsjzfmt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fuamwbnc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kzwqcqzk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvcszfp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ghtpwunw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dobbidbx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2uijjntad.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ysbbpabs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qcwtcshs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2capgzhdz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2plwelwwd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ghkvupcd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hqhzpbcd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wlcqswju.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gvkuhgob.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nwgbewns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smejibzw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jjwfvntj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igzgscgk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2udozodvz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2axwpmhvh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mkimjrcx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mtrtlnxw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vocsdxit.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fwksvhrp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pxktgtiw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gjpximbl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ihybkybv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fxurxvrh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vkfxtxph.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2wwoydxhj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xaezrxon.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nnfyxrlj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yvspwxyy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hlvpyzna.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cygblmxw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2sgnxbfof.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ympjmudu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xtvimpai.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qeeuzeri.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ajxvvvrc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kynkuuco.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wzddmcte.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fquzidzm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2serlntze.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vtywrspv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wsvjcbzb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ractxlri.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gvdvcrdm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mmitnblc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fyhqfexr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gbyaqkkn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2egvillvk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rhoezhzw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ptkgwchl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qpmoqkmv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2incxnynn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2nlmsonsr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eqgqtrjy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hvebgmzw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ibycafzz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2moqeaalv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ryelxqgb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gqtpwqse.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wxvkgjsy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wjphoywp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2povzkcrs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wcaypnht.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2sqfmyszi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2izauithp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2svedgwff.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ciscykln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txdzjmri.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ydiuvuni.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ujsvheco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxsehykl.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2btvwnhhq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rpkjnkps.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ezvsohio.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2sfriwsny.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2dnwyhmqo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fkkuvjni.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2sqhxxjlo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fgfiliqm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2alskckte.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2utgmtaio.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2woohcqwg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rdayvjch.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2vciaylpo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ieqflmjl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2abdydkek.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2itlpdtay.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2torrchhq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2todgqpnb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ynthdahr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2zfdxcplb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2asbnhelh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2uqhfsqem.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cmdkhjsv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2uzvwkuhd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ordeopws.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mvqjoalk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wuuzpjdt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nrabzqaj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2txbedexe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2esbbgpin.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jnodxwox.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2unnjsumn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qopltrpp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qtyinehk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dbmitytx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqnqirdy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pyuperkj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xypxvnfc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wsyzdixk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2nmcmwpkv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2exrobxoe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dvbgduwx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fehvygpb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2luzjdsbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtoqpaal.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2sibbpwvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwksfvzw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2zmxsscjl.html


<!-- 参考信息 -->