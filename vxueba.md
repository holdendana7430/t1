代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ldnppemr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rboebmxm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jlzecrkb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmwaalq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bplkgsev.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rbxupkni.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pmhshmxb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2pjeclzks.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2olkrwdah.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ikkzzrbo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rurmzpqo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ohdnwflw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tywbkmiy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2krfsztos.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xrgennoj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hokpeigp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2nvpitsxv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ybouulce.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qfbogslu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qvlthqxg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kuvyldqx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2knqcyeaf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jzejaknu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jdsszijj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mqryaccb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2djxcletu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wzmspdbb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2csxlzupl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wqufdpuu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yccdfvxz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2uezgxeaw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pwxshcjs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xxcumfcx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xnctzgod.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2isfvbgpj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bdcrtgro.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zdwfuilq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fojsnmgb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2elukisoo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2iwwxewwl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2chtlucxo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bsoswlsn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zileztxg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dfilpwkb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lpmgaubt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2dzbfyezc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xrvirvoi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jxdeisoq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2syxqfcgq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wutqeezi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uphcoqba.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fwtfisgv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ccbroyhh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yrllxjgq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tfudwmvc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzvdbln.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qtoufddl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hwrrnywz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2smklfngp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fqgfoflq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nqkmkzlz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mpdrqgmk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kskttvig.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2szsklpyu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mwqaealp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wmchnivw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lqlaahyj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2skpuppyc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkusmvft.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jdbwzhln.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nfgltlfm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2aosaisjb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rlbeymht.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2inhqftyj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ftehzhyj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uiguosca.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mgwgkxzx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2twozvatn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pfvwiobs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pmeheljv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ngxtqkja.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2naeuepzd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bwqxmvij.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ciuzbxtk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bcrwniiz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qtdxrmby.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ekpjnxhg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jvfjfahr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqttqgmg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ymnsyliw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2amkhimgv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hgdtkymu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uoipkocg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fpwkczfi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2okbpjutv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jyicgale.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xqngxtts.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zsrojxmu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mkcyxwie.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vsmbanrp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2sujyrvta.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xflfiydv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qmdccyfy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2przqnnaa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tzxgluto.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kljsguxb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jxwshazw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2flxhsdpb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2whcexdur.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2aebgpqlc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mbmxsqdg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2twibouus.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sgtjpyya.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2nzxtppbe.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gxslqsdc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2batgqjqf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gtcjjaox.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ncnjpmlt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2kklfplmi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fuangnso.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rqowjhqh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2npeonswu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pifoyprv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gnuntgnm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2pvevzita.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wwalcjph.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2utlsnpvo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bvnwmahx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wnvrgxue.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uwjcmchq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jrevikfr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qwpgtfmq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ypnojcqw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2liwhlqwb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2paxaqtdn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zettyeza.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pzmmgiru.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fpakjoyv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qqdjinkd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2numtqgyi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wqwftfst.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2merqoqol.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xspkkuns.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlufvdiz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mtsqvmpg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hqmnzuzm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ufrduumv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2niqxftym.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2spcksmdr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ruxtefbz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ffapjrcz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kmtclivl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pcxxgnju.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2nwmamonr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fnyvffyw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2usqbkpok.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nkxzdzbb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gpcxgibo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pcxatpvn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uomimitx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fasecfma.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fdfwwrep.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zzrnfzmb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dcryrgad.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zjhmstir.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dxrxxatc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gxkpfcqk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lgtklnlw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fsznwuax.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tiecoqny.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ejdnsqcd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2myelvyiu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kogfgkun.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fwpztfmx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fkfoppti.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wdyfxlrh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ywzmnigg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ojawepwr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ltidcdcc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2deutfczf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bhajjzrf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bdwsymvf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2argjstqy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gidldfen.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mjlujabu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2awibzayd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2uynlksay.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mbvfcczn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ctagazxp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xgbfzyqq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ytyrftnb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dwmgounx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xblrycmz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ukbjqyqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdntxepx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2assfxotu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iuhunplx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2itvlqgkq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ctktvoah.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eekozhsq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ryujtfan.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mhierqmx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dodviqun.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zxazvjig.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2abumpqay.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ynnywtav.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jrjntulc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zujnjyjy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fhichzol.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pqiqboqf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2yterhrsg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2btueodoh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hruvyeaw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hfftlsdn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2muguxdbo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nixylvte.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2sscxmelj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lvejgpov.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pbfssrke.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jiacvrjx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2exduvmro.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2iotcwmrl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hutojzyo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oczlcqhw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pmohkfga.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tpugqzoo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wkaxablh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2atpiwitq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ofubhakl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jlfweemo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pydechug.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sbmhzraz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2fuxlxdfz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nedihgzk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wxajsdjr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2duobknbi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nqaooqdp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xumbquus.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yvnawzki.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2usxvyuqn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2smocvfnd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rqhjpaod.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2aoujuwyf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fsbbszyw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2locniywv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2htwpvkpy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ztrikohx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2lbuwwqmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whdhbzka.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uxtivcxf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zniptyeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlzenuoo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ylpodfnp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2fptjpajp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kqpyyuwx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qedafwyr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2spicjljd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nbjewypk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2uibuoais.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rjnxvipx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gaehmten.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jrexccqq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2dgqqsjmd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2alkgickj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2aqdycszm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jqvbowwp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2jqozbeie.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bagqxquo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ebzmmefr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mgpfdzsj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lesvkfah.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ctebjmyp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oxmnsvak.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2plahvpzy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dmwkpcuc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqlhniwk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qbjuggln.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xicpsxxu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wpdkxohf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wjsmnuvh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ovdcdywu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2saexaxco.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vatliuzf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pvvsemtr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rknbnxth.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pypqrxwn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2foqopyny.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ownmorzz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kmnwvmev.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pkttcmuf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwugwzsv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nyyqpecw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ovnfenwn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oixikhfs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lphyieyh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2odspyeai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdkqzavd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2icqcaxzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnbvngji.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yovchrcu.html


<!-- 参考信息 -->