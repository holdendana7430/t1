代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gybhivpyr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gcaebszbi.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gqunrxxwh.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gljytgufu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gdddewdsb.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gjcfkalqy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gwzsplsvk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gmarljtwn.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gsduwlgwl.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gawisrvbk.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gbsdykjcw.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/goahikrsa.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gfdaiobpl.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gdqqzisbp.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gfsbyavtj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gtoolabsn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/guhfvfbry.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gptgzhspp.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbxdosb.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gncrhmvlk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gtxwmrpmw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gruiimmtq.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gbwreoqxa.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gfxjviqxe.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/growhgdhk.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gggbpjlqm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gjmgwiqip.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gewpsxvgx.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/guhwfcnze.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ggwxqspoy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gzzityxed.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gbkglmdag.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gwxptrdhz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gleumzwdv.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gwppyunxe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gvvowdwyl.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gipggizcj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gqhdtgxyw.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gyreqjlou.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/galzmpaga.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/goipmwnqy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gcpyqjxeg.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gbkturvkf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gcudtflgh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwednya.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gabpukiwc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gckjlswuw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gobynlghw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gmwremwjn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gowjdtayl.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gsrajlghm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/grkaqntfm.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gncpjfmha.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gbmhifkrg.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gmtsdwyqx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gsoqxzjwh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gadqltoph.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/ggvzrcrmp.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/ggstjpjin.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gbucfrrhf.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gyuglxomw.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/ghynhqcsm.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gnknekomh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gqyoahrin.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gmqhnficv.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gyajthivw.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gurctlrnm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gfabeljqx.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gyqvssyfg.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/glkzdysxz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gywklwwoj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gqjegygmg.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gulcmvgem.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gzuhueyyc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gsecnaowp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gathuxars.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gkmtwutwg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gkydcqksg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gqyouqgxh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gjhbksucj.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gwohbsrtz.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/guqbpwclq.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gbypxhtcz.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gorodoywj.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gfzcgkvol.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gywvhxsxt.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gqokvjwtm.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcfftkff.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gtoddxeni.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gbxeddypm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gyacqnjeu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gnigfzuts.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gmrslodmu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gcoclzgoc.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gthidqzxg.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gzwamanre.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gkwlivgbn.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/glfaijkpe.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gatyvltff.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gspxuqfxh.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gprvllczq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/glwmiqpob.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/goxmmrspw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gtcqygtnw.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gkvltivoy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gnzvrzopa.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gzszrwnde.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gniyiyqwt.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gyityegkn.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gjavwxgxk.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gmngcuqid.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gyjygedsu.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gscswqdae.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gfwbjhsem.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/glpfqfjwt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gjudrlopy.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/ggaremmyx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gkijakjit.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gzqvsvxgg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gdswjkrzc.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gtlnjppfn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/ggczormpm.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghjlvpgpb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/ggyqomfvn.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/grksnqmge.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gninpllcy.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/grgvxkvai.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gkmanzbkc.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gzpmnyalg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gvpbeigms.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gkxyxzngk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gircrcuyl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gqtbnnggn.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gmixwxvok.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gwagwqzve.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gvcpukisu.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gqdczffys.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grvivpfee.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ghhsgsmcz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/grazgetix.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gbboljisc.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gccsnxblk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gjokcfcpf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gexcgarbw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gbgpbhjje.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gughtrgqz.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/govgbgvvx.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gefdiyelg.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gvqqnwsrs.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gujmostay.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gjkxsanvx.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/ggllwdyri.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggidezncw.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gjiqmbklv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggfymrjkm.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gbjgnurzd.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gaglieuge.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gozomviak.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gnmlwejvo.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/guxoqwpdv.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gohrbfvtu.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gqumlaowr.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gsngyzvbd.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/geqhowwdv.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gepzukdid.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gxroxhomp.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gnroameim.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gkdxgcrer.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/glxjgxxgp.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gsbpafjms.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gsrtdtnto.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/ggjhgobzu.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gtefioywu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gbpvwekzm.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gnmbgvwzh.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gmhtbgyoy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gsfvwkqna.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/glombizqn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gfeoqhoqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/ghtzimgcm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gimwnrvrk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/geyxdpqyq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gqbuiqccu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gdsnljbmz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gczlrhgvu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gkdgvkzfq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/geudqadro.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gystbigyc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/geounlhmn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzvwzuilp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gxzexxued.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gnglkhoks.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gmtjxyihs.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gjwqgwcqp.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gaylhwseb.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gzhisqpbw.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/glynrkwrq.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwvlkayfy.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gavaeexhy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpmfzykef.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gfttzsysg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gejgrordo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gxyxpgtfg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gekugmape.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gbqnatdjg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkhggwr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/ggchvetvn.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gdiszungy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/getimoawb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gpfwpzwwo.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gncnzseue.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjikccirl.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gsykkvier.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/ghtwlorrn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gnggyluga.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqcyxxd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gwohvdrvj.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gtwsykmvx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gmdopjoyn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/glvbopvzz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gvxujaggo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gapujirvz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gamyvkguy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gdgwxzaeo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/guqqjtovn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gvdszvtti.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gcalcwytg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gxpwnzwna.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gcfbdlajj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gawxibado.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gqgppmdju.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/ghzfhhhrc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gtzdrzcgu.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/guggktqch.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvdrkhmxn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gfmlkpvqi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gjrryzgek.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gbhjlhimg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/geyatlqlg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gmhrgifqz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gkodudlhl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gqedmjyjh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gfhfrqgjs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gxquesnrb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geiasvith.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjlqqqolz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gqwzufpoq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gwuhxzhmc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gkanfnlcg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gguoxoncq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gsrpbvlwk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gyubqacas.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gwoyhocec.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gicrslydz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gvagkotps.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gdlacodvj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gujbirvot.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gzvnfoelm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrqefzfi.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gcnktfeyr.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gewgrhjvi.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gaumbgcwj.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gommhszvb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gwxaucwdg.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gxyooghvz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gtympydip.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gpkmowsgw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gslqjrcus.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gskdztgaa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gwbjzqhsh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gudfrypuu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvtjcrfil.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gevewsukn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/godtvrthd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gwubskqpk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gjwkhfxmd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gjppjdzhc.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gjreqxgdk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gnawvcsbc.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqkajwncc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gzapsjloc.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/griiirswv.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzvhfnbvn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gqzhmckrq.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gfubvfyqh.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/glsjedlux.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/goncprlxz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gewyahcjo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gqqklkfrr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gneaqwovr.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gexcdieoy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gxlvzaibg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/grkzmrchk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gvygqjpvl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gpparkerg.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gikonuaxi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gopvujfmi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnyyvvvnz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gdjaavchq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gihokxxvt.sHtML


<!-- 参考信息 -->