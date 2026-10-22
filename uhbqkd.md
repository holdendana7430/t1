代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xofbwtug.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uhojqtkh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2uhctvktd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hjaaspaw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bsbcgmfj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rooiumny.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sxseavxr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lpaqsjwv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lrtibahq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jjnmkeag.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jptaoufk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cqucgcmn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2sghwuxlz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zxajmvpo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jklckatc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kftgujth.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mfqdczxx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2oaqmubcy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xkwilevo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zhfoxfdg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gxjmqeyq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tidfzjkq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xuhahjkg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jmgkzyiu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xcccpzbn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jhxckjod.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dnexydok.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2igbfpyww.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2spwwwuua.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pjwnzxti.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2epvsblyx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2cwicbdmc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fymfuvtm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oasdshcj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ansgjydj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uhkafuiu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2peoskkln.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzbotshh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2txbhzmuw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qiaxumac.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zuhaxlmg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rwydcwwm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zwcdvair.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uogilsfu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhzcde.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lyehpkoa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zwjqifft.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijcjykgw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2chvnrsjh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xdvjgdop.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rzjhqxkb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqieoqs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2blkeakvb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hxxsatvg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2quihxozy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bogwwxgf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ubxwhezo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zwwouvrf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qkwkjuku.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrvrrlov.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uklurbzu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kytyitbd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rfcomjll.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sqejnrwf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xwvuqzsr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dnpxquww.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pmxtzoek.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pmgeezar.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ptnkhghs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gaqwpgqg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2waojsfkj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ozejlbkh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mpbifzxt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2getceras.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csatoisl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2frecuzwk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xviyhfmf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ibljicmy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vrolooyb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2psdvjhxo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2amnytiqg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vjcutqns.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2gragpsrh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dwhtnvdl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2augqrcon.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqtzelao.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dawrrppx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2scvqiplk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2njlnmqas.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ymczzzxc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2whzjydnc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cbnjkemv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ksdfnuqb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sutcvnqq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ywvpeccn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jpuyefgq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2onkzszon.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lpdwzfge.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zbaumbqi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ohdgvzsy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vbizrafo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gglsmxln.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2orgkpoad.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qqeoebqq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2yjjeuaso.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jggiumta.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uslmeton.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zmaceigc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xdzfmyxm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ghepzsnb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xivzstpv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tcxzsgjk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qqqsbuyb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2buxxqlmr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2kjroinui.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2gohjajxb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2potfwqgl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2tduaeocg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tvzyukwa.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tgkdyvnl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fxkfpciy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cfzbtgix.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gwkgeylb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cazvzcck.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nqhaxfti.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bmoodvzr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tflmewsm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2onesuvtv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sxgxqhcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jtcfdspq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zpgursew.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfhvzet.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oseupwau.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2dnpygxsk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkteiace.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vjobkoot.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2elevapdx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2htpytpfw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ajjcpxux.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxiezfaw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vhapbxym.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bfgheqop.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mgqwsvjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qquxhqfa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2efigcbqw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yihefpyw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2nprkrzmv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2trqaqjxj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2arpoptnu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yzkoyxav.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vwrivlzy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zctygocp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rvngdoda.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2aeckchpz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mdbmcxhj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iekkiguk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nryfseeq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hkhtuhbu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2guhuspbg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jzcyrlnn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wymkxxvp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2agtkfpdm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dwzbzevt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yxvbryar.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dwxxdvzo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgmqusv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jlnfzthx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iexqpjwr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vqdakmlx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2sqcmgvte.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2orzubwtr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gprzfecc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ewksllpj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pxrjvymm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rtrpzzdh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2chbzirix.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qnzqhbgw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tmttpbnh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jeqogajr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2krxfrgzm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gvlnptfs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zprvmitt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2schrxtxz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2twbpcfci.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cyhyoaav.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ncgrphqo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ynwpzqzj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2grsgmxlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzuhyvxq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2fjfnemhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khymslef.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fvcdggvl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qiestsgu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hwpqaxjx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2chhfgzag.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fepklinm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jqhfbwje.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ilvvneao.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nhvuguow.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kfhxvtwf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ygsorxpb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tyascvdg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pdsvhyhz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qusyglpp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jdrtauki.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fmeumkpz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2huyzeaxz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2gmkbgfdu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rudoxnrq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cpfgztww.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vmtvcrzy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ogmajxzf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fubkkefc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2icyjyuwc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2muluyymp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2crnyalaq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vugmmfty.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2psnntavi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ligdcdip.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dmhqgzce.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ypbarrce.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jlpxttkk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2edcwtfih.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ulzfzwlz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sirrbwmz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ahxyense.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zjaxkvse.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qgknmwyq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2mgahodyf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nnythdph.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nwosffih.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nxnesrmp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hpxdftld.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pksxxgdn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jmajgcqs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2innfncmu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2onyhfyue.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wyyonxib.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2znmlyrve.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vlnwiahr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fthbiauc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2pdjewctg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2michputl.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nktxpmwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezrlezvg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vlvnmhkw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2saazxolq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ganrjnqx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cfsbjnwg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jtbweavt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fauaatud.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jpiczmvi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ofjsppwl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2eqhheiwa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2usrpocbu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2urroogam.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ggzfyjok.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jvzgxmhi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2vlptyahu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ucjvytxf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vuahrdzd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kwnnojfw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2kuggdrvb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ioxvhvqr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qmwuqhau.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2wtedthzp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ykhqsvia.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xjmmehdk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jhtjgwej.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2afpzjigf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vcymmdoo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kiyxytys.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eomqsfqs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jzpbzxan.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nfmvwdxv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mqibtmbx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqjdcahl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wikfcgkc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tcqcagwq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iwazjgvu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2evvfytup.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zurqfnoa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjsfcmse.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvlnhjfb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vimtjmqt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2aazeowjq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2irfftczc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsrciaoj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecojoana.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wyuehlnc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nkruavqp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtotwast.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hczygubx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2khhzqkls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjchdkyy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ombbdptj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zqcvzhtw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tvuyshzr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2apwtgusc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xfjcwqkh.html


<!-- 参考信息 -->