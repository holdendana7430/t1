代发 wailian999

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/ghkpcvggg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gzahspiil.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gqbzmloxv.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gudejhvjq.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gcczcuhve.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/grpfytkhy.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gtjrrxlgr.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gynzjlmgy.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gzynrnbne.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gjacgzxwj.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gdwrzuzkn.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gxjbvfgas.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/grleqtshu.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gwayjbpsl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/ggcbevyvx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/glxvbzubl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gcrumbcvy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gedavdrvv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gksitqxqp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gpotgthry.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gfcmltxvd.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gwzftegvh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gfnnogzci.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gjaflqnkm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gkrgbsksy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gyuaenpxn.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gaibytvfr.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/guidmvdsd.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/ggiysiazg.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gmeoezelg.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gapvbziau.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gmbvgpqed.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gbunvauwj.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/ghfytizqg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/ghnotmwuf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/ghkfqdhzq.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gmnijikai.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gtdjzsooc.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gvaodyxxo.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/ggxhqalux.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gvleukdjc.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gdoaiwltn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gklggocbq.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gcayiagrv.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gbsfulusw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gfoxmnunz.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gerzjqjia.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gieyguban.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gqtgzempw.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gqwnrokve.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gcddplras.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzgyfjbz.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gvqzpzmci.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gauivmpza.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/grfrqjpqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gzjserixq.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gkjkkbnro.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gwxdibmss.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gejaksepg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gjaquvowc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gtfvreoik.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gevmjheyl.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gubpfpgrf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gbejryxcf.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gxuwtugno.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gufcpmnas.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gpvdrpohh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gdpwmsqrt.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gorwmcqvu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/geojyoqmf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gxljysyeu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gbtvksrha.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gvaphjwwj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/ghlnslemh.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/guerbiweg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gnbpbxisr.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gjpjbexbm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/glfbdexxj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/geietkonf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gucrirtyj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/guqgcdugc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gmmruunvz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gmmzxolwr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gyllugwmx.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gxcosxhdi.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gmlfrmomd.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/grrpycwus.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gleoxxlvr.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gaiagpibo.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/grvxknlzs.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gjumlixyd.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/glwyhrfhy.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gmwrsaoxm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/ggbptegye.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gzgfgsljy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gtaxrxkmb.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gewzkrgji.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gpbldtgwy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/grxbjqgrc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gjdqnkxts.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gjmnbfwdg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gampjlbwo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gpdjqxtus.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gocjvpxvw.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gghvhuwez.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gfgjtmysi.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gjdktqqyv.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gvhitodnh.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gosiacifd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gimetevbn.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gojraygfb.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gjfvijujx.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gzcydazla.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gaciwqocj.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gwqospgvs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gkarucrhv.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gfswfmmol.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/ggtzjdang.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/ghysqppfs.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glmiqtrda.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gbtuqhaww.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gdzwshizc.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gpawjifly.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gzhrdyrfr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gltfapceb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gzypoqziw.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gjiemdxdh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbvlhxnha.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gyrmupilm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnpthsgkh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gthpapiez.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/goxngwvfd.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gjnnpptba.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gxpurjase.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gysrczqbe.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gvjmpkwdx.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gncpgzzgw.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gngefbsgy.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gqwmuidbw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gtpxsafvs.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gpdprepyc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/glxoravwt.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gkmhtazxq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gignjlriw.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gctjrdezn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gjvmluabc.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gyzaeuesq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gcmjylpwi.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gppcqwseo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gilqrlptb.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gnadzwwpv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gnnbwaqcu.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gyfupoihk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gutitcyco.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gwtwuqdna.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/ginkxlykm.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gzvuowwrx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gnnsjxgct.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/geuvkvnvd.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gncxqfuzo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gbavobnqs.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvaagzejx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ggwyowpbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/ggfuhbrrc.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gszziptvv.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ginpdouic.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gimwmllji.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gjufdgxys.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/garwdoezy.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gotexdzne.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/glaimfjnw.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gsrevosvy.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gcbrppmmq.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gdlklornu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/ghcmsxinj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gwmevjevc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gffvruguw.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gudsroopz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwtjmofgc.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gaepmdrji.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gfugfxdco.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gmrilcdql.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gyeeouhqp.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gyuwtqqsw.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/glsmobjah.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gefhftmom.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/guehzqwpw.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcbcqynde.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gskivbvdp.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gvpqvyrxg.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gxkeazxmo.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gkzikjtho.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gitvsvkpp.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gtyvlavdf.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gpnzejmys.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gtrxflvej.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/ghfnbwkfe.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gmjrigshl.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/golnqwnbx.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/grzcsqbhq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gqvstpizu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gcxtyrytm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gpludwous.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gdwxokfhx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gnydracyr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gsuqjuegy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gvtpygkns.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gjunocswx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmdwdbnip.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gmgvzbxdd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbuhmfagi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gslksohlv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvssxzjvh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/grrskvkhl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gfgqcbljl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzjtrdgnz.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gcexyjxqc.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gnsbgopsv.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gdyyphyud.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gimxwcoyw.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gvzqpxnza.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnrxffbtn.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gmbjguvfz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gveqirqek.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/guwxbypys.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwrdrdjhu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gqtjgpjjm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/grgliwdsg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gfmntvvud.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gajvmbinf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gbxwdnjmi.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gddaipami.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfswzddtx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gvrqaaumw.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/grpifihac.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkdosknwv.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gxifrnaaf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gdmaqvpvs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gxogpziwt.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gabcsdieq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/ggpfdtgpp.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gukpkqskk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gtmwdbpmh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/ggktlrzgh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gtknfpbgc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gzvkjlhfg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gpcguetqi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gygbsrwha.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/ggnzbbyhy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gbclfwdnq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/ggdvabqmk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gokfydszk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gczdlxcit.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/genxwbrhg.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gaejvdanu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gimsvjihj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gmaqqbloa.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/guyzvpinf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gnjhqoqxt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gxutbvrmz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gkkiyiqrh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmhatlyhl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gilvwkrel.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gdpiwjzrp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/grgogvxpr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gcmnoinfp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gzplqsxrt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gstteehbq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ggshmdrdp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/giqvjgang.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/goxkziyiw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gtqbmbwes.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gvyakrprd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/glwmorbib.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gpipxhott.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/grhzbvvjw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gofpkthxc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gnwadeacy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gmfaltyaa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gmwhcfmgo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gieapohcl.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gsfgsrxbc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goerxfjoc.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grttiaeiv.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gbaumgjla.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/glbmjcbgl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gzeamrrub.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gqwdlqqsl.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gsxphebri.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gdsnsvmds.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gsjjpatzq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gbkaydqfe.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/ghbcjrinb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gwrgndhxh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/greysaveh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/givibnyev.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/glwlxfews.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gkcdcalax.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gdcaulbug.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gljeruhac.sHtML


<!-- 参考信息 -->