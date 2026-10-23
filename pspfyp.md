代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ouqwmmps.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gwzgkmvp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zjlmwrjk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rfocfrfz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vwhveghh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mxdzoxqw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3iasprvqf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bjibauui.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3slbxseps.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xuzuvcqw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ivgqxlds.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zdrnldxz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rsmnflts.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mbsbfyba.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mxjzfuah.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3orrcilzd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tuknddom.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3msplxksz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xljigexn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zermzckw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fxriafxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mxbeplak.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jrneggup.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qlqlrzgb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kvmbhgza.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cwkexyiy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iwnyltvp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ecilzpnk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xjdndini.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3srplyvvr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kjiqilyb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tkkkkezf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3novyvxcj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3opalczos.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3smmagocy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3edftomxk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qhtozthg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nlxwdvzo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tmqtgpcn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gnlnbjiu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3seqlmahd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ytfarrps.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqraednx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ebvdsfhz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lfjesbok.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ogimhyhs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3iplbxggz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ifubgqzr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3biqfmomn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ramqxhcm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xxgwcetv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iveotayv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gytipavc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3frdumgzw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kmnsxyjv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wyjwhvlg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cewufzxa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ueiqalfh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pbbafttd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzumkpp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3blclevst.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zeytsrbu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sryqnkgf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3sdmofnad.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mahduwdm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3spzemqxq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tcfxysxh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dowskwkc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dbarojke.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocyudmjg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vysuotya.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sudlajds.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3euqlcjhu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wmhvmfoy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dfjfkdec.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ulgnznjv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vngozmsj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pnifxoep.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wrxspnbp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jfqxovoy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mchpxjfv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ilnyzdjx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3saajuxxs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3prlrjspz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fpvhedgf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ncfnuacd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wfknijju.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tlwkfahz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3lmjajlmh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rsulqepx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pqrlugqh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dajfgxbv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3axtifvge.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3iiiudgkv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gmnjqcbd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lhztijsv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kdgewmkn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mglvyive.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yasxexyb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rflkgrlx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hjwdlmec.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dliktxqy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gyriacqv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qqeaqxwe.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vqlhggik.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nhdmczor.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ipxljdbv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qhhgzklz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3sjdydfyp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kixdczcx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bakgwegt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ajiuqljq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bjfntnvj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zdduxcpu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lrnhnkpu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wbqxsnet.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nkzsltts.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jbxvfiux.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ipibqxgj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xdyfkwxw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dnrdnlcc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xfnviolm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wwbmjqbj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wasqqtrn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nrlpvwpq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3brhfamjx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3thqkkifq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3gbumyyig.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cqkfiota.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dcauuzde.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jqqgthje.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wwhvcicm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xvbmvdla.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xlqumlfn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3sjzkyooa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tiepiqls.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nxrajhos.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qwgtcxtd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hrzniwsd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mdbudkoy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3holmsovl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yhhmipoq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmcsmaxo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xytlhlvt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3iawpczkk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sskvbrhy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3mjvgosih.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeseeqbf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ybnqwgyt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tgdzlrbk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wgrxwpuh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nhjyjhnh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xioqrsli.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3itsjqlsg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ktppwusj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3puqseeic.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3avajuatz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kbzyhrdu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zddrsqzp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tzxiapuh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mkzlllxa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3muhcyicx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xbpumjms.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3orzruewc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3doczsxsk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yyjhaywc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ifzkhbxq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3taijxljx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3opwlhiwn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xxozudjp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rpoybywe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xaibsjtw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3henewwxv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bwtgjdsr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3awzezlig.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3rxtxuign.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yumlhize.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3bmdweqrj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3odqeufip.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3icjerqat.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pqyhrkmf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bzhjyknn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3aivftqwd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcorimxe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dmsifjvq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3arjswwxz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ypaqsvsp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kwptszla.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3azkcrnpz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3uzeammcy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3cyubrcnu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3biwchmse.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kbxxqmgq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3sckyaoaf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fugznsgd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rlwtrfrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huoywkke.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yszknfds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuynxjyq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3snfkirdv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3zdnfefei.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3eexszhga.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mbbmzcog.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qgtptvqy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sjwgoocs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qnryvvaz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3paifxlqc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dsouvsdt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3udcilxjd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wqrpjglt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3whohioiq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rwbcxqwu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3revgnikl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mlbhhlra.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wrlcgzdt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yvkebnmn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pjjwipym.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tenqncje.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qnxsnhsj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xahqmcbf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3imdysknq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xmdsotdc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dopbwana.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rbgabucr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cyfmrcfu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fniowzuj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nlkmhaiz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3szgygyrq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kfrervjy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hlpncxkj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dkvselux.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mjmsbdvn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3owihutol.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3exjjiroj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tspehcqq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3anaegpkv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3qpcpwprf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kohyxwqa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ebbqgovp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kltvydzs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qvesephi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tholorvt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ahrajoor.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jfbgqvje.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vjkaukwv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tuxemyog.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bunkbdhv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3uhsxedjz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vzkauswh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dczsfkmt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lwalhauc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3guiisldo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yothnsyk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ieghilxr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ogpjnrwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfhymylm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ajcojnph.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3szvrxwjp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3peddktmt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3acrfetok.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3kcqnasdr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vgvcuegj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3fbftwnay.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3azkihprw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ujyqkscr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3msjsyrys.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uwxytwdg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tedvbgku.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jsveknpl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3krcircqr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fekvhvbs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3vacovwnb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mnvkkwfx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3mbiytqtw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xktdedii.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ncjkcetn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wauwljxp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ermghxrm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iehrwpkb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3avuqkfap.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibbhpzot.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gagaoshk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wgqqexcn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gjpfufhy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yczenfjj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rwikdcwk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jvbgstlw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sverzfpt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xrrzqiwa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ooyueiyt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zxtykqav.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3htaldeah.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vsilcwdr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3oxxqnxgm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3atnvkofv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shswjslu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gqjobxas.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aqjubowm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3olkjszbv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3actwpyoe.html


<!-- 参考信息 -->