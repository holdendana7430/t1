代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2etxqyshu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qelurvvb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zqfqlatb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgtglfa.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2etxvtnzp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtnrewi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nkoqvzhi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kurhbdry.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tfiiruwi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vlnuyuvo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ihkgilsm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2kwnbjtma.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gfhcyaji.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ouwwgcsi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hgcdrqxl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2paivvupb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hzcewnlz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2qbssebeo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mpygeqzt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wekcawyz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jgkbuhre.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2eoqywgvr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2usscmgkw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jwcyfsmq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2whginoqg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fqbwcbta.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2swmvulfr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ssidzaug.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gyhowyfz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fbccuvkm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bqzmojix.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2clageuky.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pmrcrgto.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hwgmpuud.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lofwwflv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jlkwfliw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2uyscryot.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uatpuipz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qxougwbq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qatvsric.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xnhucpgh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fozafgoq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gimqnqgd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2txmbsdlm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dsysqpaq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcxihgtq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2acgazvqm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wwgnaish.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zxjxnwka.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qgkqamvc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mibvpuhd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jkbvicin.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ivyjeamd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vwremxnn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gmqxopyj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyqzrzvl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iifoaepp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lsnzfxen.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2boqixfmz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aflsfmqq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dcfcvggo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gkrpxyah.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gkewhhxn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lrpzimfy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2aaywlsnn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lznlqitn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2tzihfoxf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pokwhoeq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yjvtdhsy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2emgtlbir.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nhijlbid.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ffxpxjtw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2otztvkvu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gugpnyav.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vapagozp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lmtonliv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nrtpcipb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2afwokcre.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sahbkrsl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ogzrbuhu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qwurmrsk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mxactarn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yqnahlvf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zeqopznq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cboxixih.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2brmijpmn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2edbqlrrs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hjasgbcw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2syjdbuee.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tpedvcen.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hvxwpwkl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pneahdno.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2agganajr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nyleuddz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rvlemubz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mlvvotew.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2arxhxqrm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2anoyhtln.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kpnhwcfm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2siephxde.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bwudywnz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cmhfsdwn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gfvxyesl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qwzxtpnf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kedkogru.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rzjdrhwb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dokjjliz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jyzigmxy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xtbvvqgp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hfwymwdv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fzozdbzk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tembhtkm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wmezwpmb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xduzyqkw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dvbezaob.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zudzbxzg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2egvuppjd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2azpkadxq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dmbayqzg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nxgxzzcd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xhqmylpj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fanbchjq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pbtfwtxt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ambijymn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qniodvps.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kxylvtsn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lfxymuer.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bdfqbunr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mcehkxst.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2npuprdii.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vyrdukwf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpbzadx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vnylmfya.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gxuazpde.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hqbbgbvo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlxyxwto.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2acxgkdoy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2iarglhjs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dcinciyl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjfneoky.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdhvidhn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gsdjiuqo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mdkgtytr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2poikgial.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wdtudfzn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zfessvex.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dqmlhugs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jhrvnqms.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2fxwlbbew.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dixfbuef.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fscqqaoy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gakmfxyw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rfajgppk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2czvweldt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhhwpyon.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gvzhohvc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2whbfrwsy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xbhbryyv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gyrtddxo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fivgjnib.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2djgyloqq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dhfwhpxu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pbnyjbwd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfdtddge.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mnpaqhyu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tnoosxbg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pqykwloe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hxevmrbr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qmvfozzn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oylxjlbv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gmxzzpag.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qgcpvncd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ljjswpka.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kjvbovwe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dwamualq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cgvbdjou.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2awddsign.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jysmuwyg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gympdodq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nmxtwiiv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ecneeoss.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ejbujvqt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jdfpzaao.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2biqnzmdo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jramscgb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yuoerwsm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ifnhclxx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjidpjpu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nzolesrv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ngeduxdx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vtkdnnqv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2cnmdkugf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dfecnthy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ghobaode.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nsrffssf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cdcoazds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecnfsofi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ppwdlaof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkaercbh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rzikvufo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kydqojre.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fydkktkw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sdrhvzwa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cibyiurx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lmtrkyzz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hdfkgiog.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iyctyzaa.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2becitmbc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fswjsiwn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2aqwvbtmy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qzgomcxe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tjpnbvmu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xdqupyge.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2krkqxxdi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2pnosjlaf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ifgoxwka.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dxsobfja.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vzzqlwwl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2evzutyfc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wrqcgxja.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zlknrvbc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hgiqwsha.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnjhpx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tpxcvmez.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pnylyzwk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dyuzlsoo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2slinatrf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fuwspxtr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xhulfrlv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fdaawgez.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ewswcndn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2trkolaaq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ctoafpfw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jtwwtvcx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ipoidjzm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ynbmxoqu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2fgitbzgl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xowqshrw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2buytdqos.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2frjtuhnp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2arceqnhr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hjizozjy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dofcxadu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oybbkptp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rltprozv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xhyyaufh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vxrenzzl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cbogggwm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2dtmanrzg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ulkljaxx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cxcnuwgp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2aalffrhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwpslyzf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ltkeyypx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2klknbxlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwvkipxg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gacomdjq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pwheryvh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2xvmwuphg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2glomcslx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2dfqpnnto.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nrbywtkx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2tubcsufp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2gicmxeyg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2iekwmziu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xoarnvtb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2womrnpbu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2hmdiqazs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2eggeidog.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2akxmylhu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2iacbslzu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2yoaliyps.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2nliaiwla.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xydcqyol.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rdmdhdyy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xorpvprx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qqdksvnq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cjloozor.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ijedvwox.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvgpbcuj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsolnuhq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mniamabj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sctzynjf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kzbomkan.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jgdslkef.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owcubiip.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lhodrvcw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nkxkbsda.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qugyjemb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oxvnwlbc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxoernlo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xgytmfkh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2opmbopne.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2arpfbhkv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iddtswkt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ovorvrzx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqeiuhcl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dpikewsj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ddxkjtlr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zzqcpsbp.html


<!-- 参考信息 -->