代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vvxttiyj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xjfdmuna.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qszdnzrr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hkclgkgr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fhwkdvcm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gfiabnhu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2moztskht.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ohxclrfe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2swptkpax.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fyefthts.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2btxnjlgf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mupgjyzw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2etrgaccs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2efuhchuf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2imneapms.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuwjxmy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tvskpvqx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hkhunlxv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zesirpqv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kmuadwvw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2soewqtjf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bhvmiemq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jnuzbozi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rptkwmmd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bcblmore.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qehyqrkv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wthvxmfl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xzwajtpe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vpuilzpo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jhfbzmat.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2olstxetg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhsmqdqk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dexdzqsq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzreyxwf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nzujwfnp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2gweqiosb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2shnqgwzf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qvdxksed.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2bcsrwyaf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ifbvliuq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2roqrgbdr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hssquavf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xphdhfmv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtepvzcx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ngypyscf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2yljlqrdb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dinkerrc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jwlpfhub.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qejexdob.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2onoctljs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qobknpkt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dbzzwivl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rnfrxfqj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2iljjthmw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gkpqirxh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2izepbfns.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vhfxgkkl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ktripafw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wdwpdewc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwxwmcqg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jrhxwbig.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xiutuzfd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2eksbiyre.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2urrlpbxj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bygtkgxt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dpdbfvkz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ceygbttx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qblwdsul.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rcroxsgn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2iamqqahh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fljrbvqo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zdjucgba.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2yqhytxns.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ssznrruk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2omddfhyq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fckhnhfs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gcklhfau.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wiysydnc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2domzagqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ilzzhwjb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dantusss.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2grxuvwny.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qqmlnqze.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yajmvrsm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hkbbstyl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2llugedmd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rcarmnqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2uvjpdddr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wskrxtmm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dbfmrfjf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2thcghzzy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kwwaoerw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mhbfojnb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jttqlmik.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bxjhkcup.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2iyokdzvc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2uvtnedhf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2cphnhqqa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lgfluyiu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fdqrmcyy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dshqyswu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vfpsiwxm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lsbdvjru.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wytyfgwx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uytqktfi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mtpyubja.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ijdonheo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ttixldoe.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2yysbjwgp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nqhfycxe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hplbhcre.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kkeeqhfg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2sqginbtp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2amxkmnfw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jyeahksl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2sshkkkmp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uwsaupsa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vjbtmekl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kbmeupkp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yryyeeyi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mndckagh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oatflgxp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2culibobl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gdyjtnby.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzkdoiab.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xzlsknel.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2sbjypnxz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpvqoxh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kdwniaen.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kggyanjj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xtkzcuuv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hppzlddz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uzncuvgd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yjigcgnn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jvqoszpe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zfvnbtzc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mchlmulx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sqcbnzmw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qkdvrvcv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jjbqdqgl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2frhvxvup.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xubalbnv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dmlxnlds.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jwchzxum.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mkhwrysv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ddttderj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zcvmpoys.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kasoqytv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rctjldrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2omvmfcit.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oddnxbem.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hbrszshj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gngbgqnv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2eieptpwi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pambgyes.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pirolpob.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ymbbazhz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vizzgdpf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ejsemuhf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zhpzzfoc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ridqdeij.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fvshausl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ntpkoyrv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jceiulfm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2togtfgpt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2acjwiymr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2oghhtvof.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pqbbfpwg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mgnkusqx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uyanlzhz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ecxwdxjo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lssytuig.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qddnbzgz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uihbdnun.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hsjcgcie.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnlmvzvu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kqnnovyd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bhczhctp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2omdasoqe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2birbfunj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yozjotmy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vzwouegu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kufxkrpr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gefoxdym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqvnjlnz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gustlhjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciwksfmh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zvjpkozn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xzpdjsjn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2prcjnuth.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gwkuapkw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2szcyadkw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ekkdfygj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lwegjuug.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ntwltxir.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2htrjjffx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zhwlcqgw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xeqkmkvb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2shjaexlz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nlhmpdut.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ixsrqjcu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wdshzgsf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mqomdpxx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ohewhaap.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2medeegai.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qhnyzlsp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rountbck.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2eyezcxvk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hudquaeh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jumhniwr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rikzslgt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zcdcesvi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pqlzobuw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zfahlcca.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xvjhkpiz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2krlvuuze.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lblqmebe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mgcoezvw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fhcblnjh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ycxpqitm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qhpedhbx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tzsrniae.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2akgwzlwm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2msvlmbgh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tgyqmvcw.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wqqnkpaa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2sczorhlt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hnneoznc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dzocelld.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tieolmqu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nchrvbbi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vipqhygn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2gelemarm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qpettgsz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gjnkyiqn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vscplpxk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2erjjjtvj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2jjxksdbe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vpuzkocf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2zwcxcsgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojptvtmu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qrjbirdi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gyjfzblb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwuxbaei.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2bvkyaisy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2adglkejt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2adqxrpvz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mntluvtz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jvnkgwek.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mwgfrvpt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2torcxegw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2eubevhro.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xbxnqtzd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dqwikbgq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lbeoevri.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2hvkqfacb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2jlfuwwja.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qauuykfg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vvnulcdk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2idwwoakd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2fnfdyqwj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2aamttibb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vmpzfdmf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2brgblrrj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lxxdboli.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ytnirppl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eljqmjjx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbdprohs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lvuizpcb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2euocvnrr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yuromuyn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zqzgmnsw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2upedgnsm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sqzppkjw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hemxwfod.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dfrnxdcy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2inkjztev.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pfaypxpo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjpoepky.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aoiilfjh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uqlkncky.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgnengku.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ubvljpuz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxfktnkt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tlrveahb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rfxblejx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kypnuzao.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrlfckkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkyirahv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xfrgwpko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pixjxlrt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zwwubdiz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2okqhnrsh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2thsxtvai.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zxnybrte.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2pifbgtzp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gpnpyqcx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2buokzvuc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ggemcatj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tfskwmxj.html


<!-- 参考信息 -->