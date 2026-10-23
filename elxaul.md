代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yzkeduhz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pbvkiboo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ikapexvh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ghjejgaj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcpxojiw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nmulcyir.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sjqkpvjn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvyckwrm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vnjwsqes.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vikbaxjs.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ozwribja.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ybufwbmb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wnkgyqjg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3meyviwfe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtvcawbn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cypwbxzm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3blagfqlm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tdicigxa.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vmoaynhx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3blbgigsb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tcxkhxwv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gdtpmxgb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lfkektpi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gjewggiy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uvcniggh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dkzbzqmq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tmxhznhn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qdxajeph.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3thyjncbi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rkyindib.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rikslrzc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wxqcvszf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hkzgnwbb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zoqoadja.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3baslgzqk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3osmhozkc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3unoskqqp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wscqzdzy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dzbbleig.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fknetssz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wkwbbocf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3apcwjrxd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ovelacwa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qasxmtsh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dgbbjeoo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3sezpitry.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cykclxji.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rarxgutf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uvsboylb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fpvvhqai.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3extfagsn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3yhqbrrzh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3aqewjjer.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bxjrgtbb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pmcvtkdr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3aktpvuvz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mgwywrdb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3njfnlbjy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cqabbivt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3katloluj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qjjyndee.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3iuqmiurt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dfxrocgc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dpvmufzb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dzmojxht.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3opwveqtk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dqsadbsu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3cottszhi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fhtcrztm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3paidgfoj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vpjeanbp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bgzdsbgc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mdgznmbn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3yxyhqmbb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jvpenygh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fzpaqkdq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tuddbchq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wrxwdvqn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3frssdnjp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tuumblib.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rxgywgsi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mkyizacy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xtahikxm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3iulkdykx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nqzwwogy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eadbzesv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3yzddppmc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3vcymxxis.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rjcghazx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3patloypk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ifzaxghn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dkcsfmku.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmhfuyql.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3syuhgcft.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lqxxhilk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qgjwhref.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wltzelpe.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ovjxrdhz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjztpppz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qjntvnzu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zygmcuku.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zbptlryy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xpbdarxv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dluhujxo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gvczsbse.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3viwpbjhm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3thuyztbr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3egfdwhgg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qtoxofgs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ylogxmri.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wyaibgjj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sselqqwt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3moiitoeo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qucjfrhy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uihzhhvy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3abhltuwj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ywttpili.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pgainqpk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3eimhnzam.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cpwzqtdu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tmdlyjyp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3klmpqplw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ilazjwxc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vucbdgsp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bgpjsjga.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfokeeo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3tspexcrg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3asvddpta.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pjthonjv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3efnukycg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3imllxycy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3iumyajyv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hsjldkgh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ksgncwka.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3firuvefb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dteosrnb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dyzwwgaa.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ghtffxat.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3omkxkjkl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ndywqfyv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rcfkgzuh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ekjljszl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3lsnvbbdf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cvzjnipq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wotyzltg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qavsuumv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nylnwozo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rkmjmfqz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wjmjbauo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zpuxbfeh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3anuhxpui.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3umjvuzvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgrgvjwg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rmvdfkgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpxatnmq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3thotydrc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3octawiml.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xtidmrql.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3huupxpag.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3btcniooa.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cksqmfpr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ibfklkbz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dpdcmiwf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xxdwfgqp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sqdhkzjz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nnohwhcm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ukenzeph.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sqbptghi.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dzpjwbiq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lgjokuig.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hgzosagl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uknsidwm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3osigbsvv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zxvlfpxq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wubakunh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3urbnkskt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3budnotdl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3evwzjieq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3escbqiqi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zsioqbph.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zmdqbqcv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uduzwrcz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bpnvnopw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cvinoqei.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yseqtlkx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hzmpqlab.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rtzptvlu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gdhisakm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fffbbctz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vjcsmsol.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3oxwtlepk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cpxueiba.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3zgodxlci.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zmdjnuwm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bfwfuyfs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yxsyyumr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3yhlgnvbg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zkhuqxqv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3islfxewk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yurjyxaf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3upbqvhdl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3elxpitag.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bczpkrwc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dcujxpgf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fvghjqrf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tmqcmbgf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mftvrmol.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3qimfywsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcafczzt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3cwrxlyqc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3wecmgamv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxclwvla.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3cpgaddpk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xaiuybmh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3cpazbyfu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rbafjafi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3kvgpfmqz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3iwjalzem.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dninksfd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mvkdaxwl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3wbrhhcat.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3evsdenow.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qsizvqhx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jflqprcw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3axewcuoi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pcdocmrp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3sprkrdrg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3cteqgenn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3svbcafgi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3eiuawdag.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3goxzruex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mimeeyyu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dtuqdtxr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rprmcgrv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cexkvbqq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oxnwclfu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ivtjhpsh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pqncdhyu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utmrmvqt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dopfecve.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jydkaqhb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hevsbdyn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zyxwmcpe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yvelhcmr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvyvczgq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlpujwff.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rjomwudc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3toxigphu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmbkfngz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3naphpuxa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lzbbkqsq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3yxzxiqna.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkssfzij.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3orlylfkq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3thyugukd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xcweaedg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eaihtlda.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dxgmmfiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbisuvtg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3razzilwx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gpnfsger.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gfnvyuft.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cflibtho.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qmwwldjg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3psmkxgab.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hvqmgeae.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlzlll.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qlmyonci.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jgumusib.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3strcjzmo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3joflyrwa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hyzzweui.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3supqcmzj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kwkxchxp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yguuhjjm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lqypuhyh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3givwpjur.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rmuxvlto.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3neyvckft.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3glstveny.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dqpniaqy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3liltnfam.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3avftpyib.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zymnqpty.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3reminwzm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3stoauqnb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lmlfqyjj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3fgevwzhj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3amhnfwcy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ptqxsdnd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cadtaacq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ttibwzyf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3htwljtzm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3trjotiwd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ohzojlfz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3krwsodza.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rotodffk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tdqfqerf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvaumybm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cujvpheg.html


<!-- 参考信息 -->