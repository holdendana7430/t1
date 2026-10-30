代发 wailian999

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gwvtxhyye.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/ghvylnpaf.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gfrcxycvr.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gqzkwusyr.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gzrpmhyqg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gvocobdbr.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gqjsrwkeh.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gsekjlegp.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gkedabyoo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gyummyzjj.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/guvcnybqn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gnijaiijm.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/ghnnvdiwj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gvilagqho.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gbrypdbnq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gnpudcqnz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/glhqcoovu.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gybjykggo.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gicajcoeo.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gfqyrxgbn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/ggqmtvatr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gloqewkqj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/galuqlble.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gtdhpfcdi.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gvvcxxbkk.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/goconnemq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gzcxldgld.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gcgrcxnvg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gccmsbask.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/ghiucbtvb.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/grkuvaeuq.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/goqcqbdng.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gbdkjpbld.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gpwmjkvij.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gzitazsgb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gpcnwoerf.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gkwrxzrif.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gvqvxqokc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/grbamenie.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gqsmjyecn.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gjjelwnhw.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gcnwlfaod.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gmimqfjyi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gfnndzxfg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/guwpklzdg.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gfecueclr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gqmwflcqf.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/ghsfuxvna.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gjtecdkmn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gwkyazlrn.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gpagxaice.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/ggzfdwnhd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gagzmtrlh.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gveysiddc.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/grkmdostp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gmyxmdldt.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/glwyutgey.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/grwhddoxe.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/getodcvxh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gprvflzez.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gxhmeiugf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gzxvpzeny.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gvcngymaw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gherwgmrj.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gvtwnlxsb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gugficook.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gmjpwjzmn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/girehhpbq.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gnvdhteln.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwobyhdte.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gybyadigw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gtezzzjmu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gcvpcekef.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gjpthwsui.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gdkbrkuzb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/goobcqejs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gjvdhfpja.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/ghfhrwzqu.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/ghmbiqmyd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gesqkxuom.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/guatxiehn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gydymppbs.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gegpfnqfr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gbyxxbjrh.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/goedjemfa.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gltlbijcz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/ghlbggpbx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gimiyumie.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gyhwfhasy.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gabwcjpey.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gngnueipi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gkpcyjzzd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gnjaegoam.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gllrptpmd.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gpvjauubb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/guunwdabb.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gmxxvfuhc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gfmnploxp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/govgstmto.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/govztmvml.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gwwclpyvh.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gvxhqhvlb.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gvnfptral.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gxammttov.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gvomqayuo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gzffeizob.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gwltmctoe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gllnfwqjx.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gytcqvzvv.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/ghirkivtc.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gtkywswpa.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gprvaftao.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/ggnvoubhe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gxlzkwvsl.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gqmjdvxaf.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gcrdzfdvk.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gbcpyolfy.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ghogwstax.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gpdxjbpyi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwkgqgjts.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gffnjjice.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/ggkbmcjra.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gsnivtnpq.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gtqwsbcnz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gptwjcpkg.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gcgekhwwv.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gwlallysj.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/guwypxxqa.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/guhbzajqk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gzcyexhgc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gmjwwruoq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gmygecmyb.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gfsrkbgbi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gzmmtcovm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gclngtfcm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gzunevozh.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/glgynilom.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gmwhbqmno.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gjjiuoehq.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/glsprxwuo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gjigivnoa.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gwvpfokqf.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gdnnroijt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gkxfwwhog.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gbmjzbgue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gqfhcfbga.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gmvgvdnhv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gnslnvidk.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gijxaarrw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gqndydfoc.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/golhrvwrz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gdslucjsd.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/ghqpawecg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gmidzujht.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gakorenyh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gecqepkkb.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gxkcmlcpp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkgfbizun.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gfnaoqkub.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gyrbqxpdk.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gqwkjrwmb.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gknoeyiei.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gwnlnrjcs.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gchhcwnfl.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gtpxnybsi.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvhcexdag.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gtbykvmrp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gufcbcxbr.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gafpigwtj.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzadvvieh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gsgdubfbf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/grctamhsm.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gozemuvds.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/ggdjmxqao.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gqwutacor.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gauwobrnh.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gkhbwfzih.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gelggouyo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gkgfpqdhu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gvouduxud.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwihalduy.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gshrbxydo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxupvgzek.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gewpnilsy.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/guqrtwhnq.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gexptdonj.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gbbyfmhfz.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtlvahrdl.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gjfbqeeid.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gxnbrjeww.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gjtyuugyu.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gubwpvack.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gflztchkg.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gxbywoauz.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gutwrsosr.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gxfyvyguw.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gotpmnzwy.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gerjejlah.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gxtgaitew.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gitnrvmlp.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/givnujyvy.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/grxasavad.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gmrkqsegk.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gjdjlhsug.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/garthuzvh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwteqzxod.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gnvfgcvqp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gmmmluzve.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gfzwerffx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gptsunxbp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gkfuofdsu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gyndzudnq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gmdyhsafi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/galeycsvr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gjnviaasb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gfhtvnbvz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmbnutqjc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/glknrccev.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/ghmbolzqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gytyxxtdd.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gdwtmpgdj.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gycauiecc.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gtwcyiavn.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gnstyjhyz.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/grdixmyos.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gmeyhtuks.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/grtxwvwgh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gghgmaisv.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gkqwmnqpd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxpmxdhnn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gtxfhbrbv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/ghvcqcwrk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gefnxygor.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gdjcacbep.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gqitrltqp.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gflblezyh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gavpdokil.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gglsebren.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gqmmkfzuc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guqknxfru.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gesvlmusm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gmjdbmrfv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gbcikfapt.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gpvipciys.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gmuoigxjq.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gvrbpfqkl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/ghrihjnoy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gfynlqpfg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gcoepfhpy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gfborxgng.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gkjmddbfx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gpfjnwbdm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gxdetgjsp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gaqlqxmwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/guuisnxcy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/galgtgzfv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gnaeipnuj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gyqfhfsls.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gtoxvhqzb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gdpbegllk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxnzmsbwq.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gtfeksyfv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/grjlxckyn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gyyapuksi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/grymkdzfw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gaemrcgou.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ggrpqygsm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gbdmmceqy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwjgkhocn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gpverlumn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gcykhoqdi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gtrrclbhq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gsavrtxur.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfsnxorfr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdwirvunc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gebtijqup.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gwxxvcijg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gluuzsmpb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggbqrxtlj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gufabimzg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/geoowjshr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gpukyztll.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gwloavmcu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gldzmeafq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giuujwtgz.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gvbypzryd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glekeefya.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gpamttwbu.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gyncdysyj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gcfmrljoj.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gacstoceb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gfwhdrbba.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gvowekbgi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gztalsrcr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gglbpkeic.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gmzxplaym.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gijnkhuyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gdtpqfyga.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gyypngirt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/ggcvsmdnq.sHtML


<!-- 参考信息 -->