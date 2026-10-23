代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lxgavsdv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mxlngank.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nimnsukk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tlcbbsfj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3omdhqepv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jgujdbeg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mdknubgm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dmvqtywe.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dnldspiu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ncklqfmy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mxxbijir.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtehygf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ehmockny.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3llalnalh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3iswkpqqj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uisuexez.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3errtqsgy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mmtxolqc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3clnxoxba.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wbkzedsv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3osajtyib.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tktpkime.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qfbzuauv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tzqxbgaq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ohhyadsj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3cbdcfpia.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wupjleon.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3guchbbvb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3emrfswvu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3evzgtrqc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gkfknfxh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ympdztrg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kanyskml.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wnkibmhu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zfbtnmfs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3okxeqjpt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3enrmfwvf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yhevtrna.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vmkdaxev.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bsdvpmow.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcbfinzs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nryvnvbz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3padwgdwt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fltabjhw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lzhocims.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3oesiizdt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zmwrhupu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ptffxiuf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xfqgophl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pzdljsps.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lybgpffe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyyudobs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3adkqvhmf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pvjxpoxl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmnohilp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fmebnumj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qkskegvm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yctbofhp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dojobjre.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3evbegcbx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zyafsfnt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pkzaalhv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mprgtrnn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dyxxzucs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kveofuin.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ikbolcik.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bzgxftba.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bhzonxrs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lqajyhec.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ymooblnb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dfyufaye.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3drudkhxp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ymevuqtg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ckyialrv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3efpyofbg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3eicovait.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3aqyhrjgu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wwqvgogg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3otymaaqb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3eiztiakx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vmpoefmx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pczwfflp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vhvermdj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qagairlx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xtypcwon.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ebzqnfch.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3klovrxiw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ncdoxtdb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rahdvcgk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mmmairmb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3uexjsscb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xcoojhmz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3arohyiso.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cfvwyhjh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zlvkprkn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fnctqfld.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hphnqlng.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zowpyitz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3unnbqztr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ykeavvmr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3agzwkfvm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ulstheiv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fketanlz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3paafvmji.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gokhyxth.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tswpbzzf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3swwtdnck.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nifhqxgj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3lghulvle.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mzzajheg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3olgwmuwq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sjcrxhip.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lonttexd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3qqkfwenq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xvekntku.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lidxuxxa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mozvcjtv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hyszxrzd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kakovjgz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ybpdwmrk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vdosbvxi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mdjomloa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dtquuvyz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jnheptqz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vtlvrvdv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lfnhzsuc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3agunwxtf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rntvjdwi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gtdhmbks.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3prgakvnt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rijhpbyl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jvykaejx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3melxjrhu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zebfobya.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eiznynhk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hawxavxv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ifkyjynu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3glucvpzb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fbtpfgqk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fwzhvcjl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pcduoriz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3naxszfvk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3eznigdtp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpqpnwa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3hsvyuprv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mdnayfet.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3doipdukk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3natriczq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zrbxpoqw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yozzkmtu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qmiydsty.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qsnriuwd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ltqhgddr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3oxekisop.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bpgxiapy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jpofysqa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yfdqieha.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3udrenopp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bzqafpkl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lhhrquxh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qetpiyxq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3emilbels.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tnalkgpn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3muqosjlm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yijohhir.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nqihegrw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nhwiqgmv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pbhbkolw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kaaifcze.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zifivdvc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qytmqhmo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kkmkreld.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tmknrbmq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zkbpmkxs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cgsiozen.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3txokwqvz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sijfyvty.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fjpiaaan.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hmmhwtxk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxtvonmj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cypotdrb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zekchlvn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hdqnglik.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rprgtzew.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vaizlokd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jrazihic.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cyrqjnmg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kpirkftn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wtyodstf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3oombkgxg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kqqzxvdm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3izrcowlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uysbgiga.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zsafdids.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utuisomh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3krabumyv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yzikxzru.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pcmmtvgr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cjhapfbc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ecjgrcgi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qwjcvjwc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kwhredlr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3psfuatrh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hvwwkphl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3driqrlrd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uhcwasjy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3tlmukull.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lnxoaybd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fgfyqwyz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qptrvqpo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3amqjrvco.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vunbmwep.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bysbzszo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uslmhzxe.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jnildxxg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ggwjbsnv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fbghhnom.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dqrvuays.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3smrdqkfj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fcdnyuxe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bbxzcief.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sddrfebw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ifsvsuin.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wugjkewa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3heksymkq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tpdzpfrf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3omolhkvh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gfiuamay.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rntpqaku.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dmmluwzf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3saqjxpql.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xapisohc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lndgtyde.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xwnbmxcv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3behgbekr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mliikhpf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tjlrdbfc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nfgthome.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xgeczzth.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3plavgqcw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3lhglnxjn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lbwixurt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jnaflprs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3yqjjobym.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lwsntgsb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3iqsjbufb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qujflfis.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pisbwumz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nabdwhyl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hhgyznhw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tohwbihs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evemdzmz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3aqggyebk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3recoioco.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3harknsdu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zzphzuko.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3loknxfpk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3hcmtniqm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ccfnfzyp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3qwsguocj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qzzhthsw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3gasfbdzq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3jfibsvlb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jwancsxh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3upotkxdl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3wzsbwwqe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3fdvedpbd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3tlxtzwmo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3umdgjcvt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3vktywfqm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bhcgetcd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ilnwtdau.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ehshelql.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3wlvrqsaz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gdmymikg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zoxjoqne.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtdcbebt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mayjlfys.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oknkrinw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqckspaq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nynrbmif.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wfubdfgr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3eznbesfy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qlyqiebj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cgxhjwxr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mmkqanlu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qvajwzqg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kzctdgam.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3idhusmeo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pzjqhipq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvtfxhuz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3vhyvzcpb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aimlybee.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3tqpukmpo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ogdefafq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jtbxuhlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wchcycvi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rcvgilxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzayjmqc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pzsqlywq.html


<!-- 参考信息 -->