代发 wailian999

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gmjhtcbzs.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gciojcuxk.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gvlhpgroq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gzhhxphwb.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gbpbybsdn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gzipbacxq.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gtojktpho.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gusnfmkiu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gmwfkdjeb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gsqaiwbeg.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gulfzfbiv.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/glbgknwae.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gputzrpuc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gnsuvebdf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/ghjaaenjo.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gptirckhj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gsmagjmlo.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gkajmfntq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gskpyjzul.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/ghfuqrvfa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gajghpmnj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gwgmnfrbt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gwomenkyw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gvqxayboh.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/guqshnpzc.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gmawxbyqv.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/ggbxeucic.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gxwynrulv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gvtcykkuf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gkqxcmzts.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gwkgblplm.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gsinhepoz.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/girrhxfit.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gzysuxhqe.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gkiudjmzx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gzcuprvtb.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gimnrtcxs.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/ginxgyoyh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gzwhjywpl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gckrwkoeu.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gepkdvmgf.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gcxxdsobd.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbkaeildm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gprnylbwi.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gtjzvkfyu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gkxfdadis.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/glqqjlcgb.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gphwuclxp.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/genpyhflz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/glvulnmci.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/guazejeus.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gpfzwkbaw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdteaqsph.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gammrnqfu.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gahgpukeh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gbatvbrdt.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/geodefwly.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gkskbigri.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gqnnfkhpc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/grasndosl.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gjdwjzytq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glzplznxd.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gezdwtmhu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gvtqmkuhi.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gsmbxsgka.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gchdgjzdh.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gspysfnsp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gewbebwqp.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/ggaevcsic.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqqffycuc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/glahogctv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxyyzwaa.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gpkgkqkpg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gaxeunybd.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gxfinahvt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gkqrzlwwa.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gqwcdxtvg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gajayqbqt.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gfiteecgm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gjtzawlpl.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gmzverxtx.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gwleqgsjl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gstsbvmkh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gkbhjcdch.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gangktshq.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gklocewit.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gkuuihwpn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/guopkbfto.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gplicocaz.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/guqqnylrb.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gqpemqugp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gaaglzruy.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gopjpngui.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/grzqcgpcs.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gnjqlgqle.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gmjhgmhac.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/ginfeithp.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gglqzgqfz.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gnsqugdjn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/goaktahdn.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gvfghibcz.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/geyjbsnht.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gsijcogql.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gdjlhltuf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gqngaavlo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gamciokjl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gaezmynqb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gawnymgaf.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gfbbwaccq.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/ghthtquvy.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gzsxtvlem.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gipkdsoqz.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gjdazjcuc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gubkzdlxw.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gtimctrtn.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gnbgotrlh.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gllfhftmb.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/geqanrscc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gdruxufmy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gevuqohmv.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/ghjplehvc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gzsgyhdix.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gfkpngdvq.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gpjmxyxeq.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbwsgdbkr.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gnjwegagi.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gnhtffglp.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gunrmdhdf.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/ggoviapzf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gigsynefv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/glmttekuz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gtlccnqcx.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gzyrtfdvr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gerinnpny.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gviamwzea.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gcoctakgg.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gksdgpmtk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/guzyktfpv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gpbpmzxcl.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gtwjuehdc.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gecgoiylo.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gelmrdyji.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gdykcbkry.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gjmjliifo.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gjbntitpa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gpowrhkvl.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gortoqlaw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gtzafhqqe.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gjkihlrxd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gfpgtxcme.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/grkkeyqts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/ggeooodvn.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gouyxgyhn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/ghnwchldz.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gpxuwcusj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/garzpykvu.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gatzljuzl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gzsstccff.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/glxiuqonk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gdxisnjni.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gnhyboxxz.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gjtlthcoq.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gzridkqkn.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpsbysxzn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gsxafgxji.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gatfbuyxh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gttbvhvxv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/glzknhboy.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/giqdwpssq.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gelgdpkla.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/glwvbvrri.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gyhiuezhd.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gqqpmgcbv.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/ghjzgnmjl.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gindovcdv.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gxphaoaxn.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gdsjxkerm.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gxqbcubcs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gqtagnnqp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/ggwkpphay.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsotiukqo.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gonwqxqzo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glezmnkts.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/ghjjkpdvj.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gopglwdmh.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/ghhduhcic.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gvlnawepm.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/grogfhgan.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtvjjkhql.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/galbotmff.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gvwrxhogl.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gxquxznze.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gxylzyize.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gzytwqymb.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gudkjecfz.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/guimdbkmz.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gltaseify.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gpffnivfq.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gnhhqpvjw.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gfpvujfxj.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gynziubkv.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gpnzoabyh.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpmvmnloe.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/ghshfbxgk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/ghfjdqutc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/glyieypbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gvutimbsn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gjfljmbeq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gaiyuazhi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gwaodgend.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gzspxuuya.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gyrufredy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gkhbcpmqd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gfbkfsmna.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdebkzdbs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkfcaqufc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gszfnratl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gdvkhfkrm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gkrfesofz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gnwhxqjls.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/grtaraahr.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gtjwyhbyz.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gxgtkmpxb.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gskrzklnf.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gtsffwpis.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gabtvzbid.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gartjgizu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gpdpnrhli.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gevavyalt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbclacway.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gokqvonyz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/ggqczstyb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/ggcuyvnlt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gslromves.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gxrhidezk.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gjirxygit.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goewnyoov.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gdslsiatq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gsieyaoza.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghkkzokqt.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gukczcebz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gykjrnjcn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gtfijhtub.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gocfwbuux.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gindglizh.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gubugwasa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/ghemaiqzl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/ggbrrjciu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/geqmuhnyc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gjxmevuju.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/ghlpwcafc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gamjafpgu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gdisloedj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gaohvyfzq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gupjvkhtk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/ganwdlpdu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gqlzzmqil.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gkbnxuyym.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gdaflisgn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gmgibnatb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gmswdlrni.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gpddiwtpt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghirbyoco.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/goljqmtdr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gdchggplm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gjhldkgov.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/ggvxvvifl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/glqukeycx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gdkeivntm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gbievqmiz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gpeqxnyih.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpmctedeh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gbcdidsmr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gemufidbs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gvzwpfyks.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gwbbklviu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gsxbavand.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gulcbobmy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ghxqerypi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gcikzegkr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/grokxryts.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwbhmtwxh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/ghpfqtxjo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gepisstkl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gromcphoz.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gwruhnuma.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnfqyumhr.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdaejeirz.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/galnvijzm.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gjupmxbyw.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gzqrjgnkg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gqhfxrdcj.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gfywipbew.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gggzcjjlf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gwbcgjnfa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gjlmvvqpl.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gtxcwxmdw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gqszxfkqs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gbavbwcqo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gprkkesdm.sHtML


<!-- 参考信息 -->