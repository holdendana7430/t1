代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hz.feifeiyinyue.top/gtkpwbsrpk.html

sys.stdout.isatty()
来源：http://hz.chenzaomai.com/gtkreomkby.html

[U40] Py：打印到标准错误
来源：http://hz.cqqwz.cn/gtjafuexbg.html

print("err", file=sys.stderr)
来源：http://hz.gzhubu.top/gtqakwxerx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhongyouzk.top/gtxnpztnpb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.0kj1m.cn/gtjcistikd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ybcxt.top/gtzxnwaqys.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ydzc1.top/gtljwrvsiv.html

[U43] PHP：声明命名空间
来源：http://hz.yj20258888.top/gtvlamhvje.html

namespace App\Http;
来源：http://hz.xziqi.cn/gtunbskzfl.html

[U44] PHP：开启严格类型
来源：http://hz.gzhubu.top/gtlvflajln.html

declare(strict_types=1);
来源：http://hz.chenzaomai.com/gtwisjyrhu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhoulong.xyz/gtjvwgealb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtmrsvjdqg.html

[U46] PHP：可空类型
来源：http://hz.ehwqpu.com/gtdkkbnhnt.html

?string $name = null
来源：http://hz.yj20258888.top/gtgblxwbtc.html

[U47] PHP：联合类型
来源：http://hz.yonumen.top/gtacsxlkwb.html

int|string $id
来源：http://hz.andypj.xyz/gtrdwqpzys.html

[U48] PHP：纯枚举
来源：http://hz.tanke756.top/gtuygsyjrx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.feifeiyinyue.top/gtgunlzinq.html

[U49] PHP：只读属性
来源：http://hz.fengsongda.top/gtwvfuldyq.html

public readonly string $name
来源：http://hz.quarkkingdee.top/gtxnlnikmg.html

[U50] PHP：构造器属性提升
来源：http://hz.316326.xyz/gtgludvini.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gtagjyfnwg.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangtech.top/gtlbzfhlkb.html

[$a, $b] = $arr;
来源：http://hz.ywan-chungtsiang.top/gttjbekpku.html

[U52] PHP：箭头函数
来源：http://hz.yj202588.top/gtgtzbvrgx.html

$double = fn($x) => $x * 2;
来源：http://hz.gaohongyu789.top/gtctdsvilx.html

[U53] PHP：空合并运算符
来源：http://hz.gogol.net.cn/gtnhabphoy.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigfzy.top/gteykmonyb.html

[U54] PHP：空安全调用
来源：http://hz.zhongyouzk.top/gtdsbpubrh.html

$obj?->method()
来源：http://hz.yj20258.top/gtidxrzerp.html

[U55] PHP：match 表达式
来源：http://hz.jqgufenzy.top/gtvajqkytc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shuidangran.top/gtlesvlwxl.html

[U56] PHP：命名参数
来源：http://hz.guannengcc.top/gtciqjgxkq.html

f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtwskokqqa.html

[U57] PHP：字符串插值
来源：http://hz.zycfv.cn/gtrtpnzfwn.html

"值: {$a}"
来源：http://hz.zhijiandao.cn/gtlkfyrdyd.html

[U58] PHP：数组三件套
来源：http://hz.kuanghao11.cn/gtaywmycef.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtpncfurvf.html

[U59] PHP：自定义排序
来源：http://hz.havefunace.top/gtzigzhzis.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gthbvsayfv.html

[U60] PHP：JSON 编解码
来源：http://hz.ppjwa.cn/gtxvthudyn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.birdmap.top/gtvoxeufyh.html

[U61] PHP：正则
来源：http://hz.guannengcc.top/gtlnlbpcdn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtvlapyiox.html

[U62] PHP：日期对象
来源：http://hz.chenlongwang.top/gtazdajiex.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gotoacloud.top/gtxgovuqov.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gthpuacmve.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gaohongyu789.top/gtbndunzzr.html

[U64] PHP：目录遍历
来源：http://hz.xuanzx.com/gtmcysspql.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tanke756.top/gtbuloxofz.html

[U65] PHP：会话
来源：http://hz.gaohongyu789.top/gtrsenvbef.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.fzhhl.top/gteledzodb.html

[U66] PHP：设置 Cookie
来源：http://hz.tian-w.cn/gtklwnbqpa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.feifeiyinyue.top/gtbpqtdcwy.html

[U67] PHP：处理文件上传
来源：http://hz.shangyingyoupin.top/gtiknkzkjt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.iojbl.cn/gtnozemacp.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtsnusgebm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cqqwz.cn/gtbghsrhsa.html

[U69] PHP：PDO 预处理
来源：http://hz.sysykeji.top/gtxmxzqkol.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yj202588.top/gtnohvchdy.html

[U70] PHP：PDO 事务
来源：http://hz.guowangkeji.top/gthsnxjgcg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuanzx.com/gthqywvibc.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtqpthvpcv.html

throw new RuntimeException("失败", 500);
来源：http://hz.hongshengwenyu.top/gtkeqqezcs.html

[U72] PHP：写错误日志
来源：http://hz.sxryk.cn/gtmbjaroxy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ivvv.top/gtxvmrsdeh.html

[U73] PHP：读取 ini 配置
来源：http://hz.fzhhl.top/gtwhdewnlb.html

parse_ini_file("config.ini", true)
来源：http://hz.hongshengwenyu.top/gtixnvmkhg.html

[U74] PHP：读取环境变量
来源：http://hz.gaohongyu789.top/gttvhpcgcd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.feifeiyinyue.top/gtdhroktfr.html

[U75] PHP：依赖注入
来源：http://hz.xinyue.icu/gtupebqudk.html

composer require psr/container
来源：http://hz.sweek.top/gtehubgtys.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtevaukgof.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hnxiangtu.top/gtgifgdsma.html

[U77] PHP：模板渲染
来源：http://hz.hywenlv.cn/gtsqyhwxoo.html

composer require twig/twig
来源：http://hz.daxiang520.top/gtxnvgbqel.html

[U78] PHP：单元测试
来源：http://hz.yj202588.top/gtljnczrad.html

composer require --dev phpunit/phpunit
来源：http://hz.chenlongwang.top/gtpldbinlg.html

[U79] PHP：静态分析
来源：http://hz.52xcode.cn/gtvnytgotv.html

composer require --dev phpstan/phpstan
来源：http://hz.zhijiandao.cn/gtykbtyvgd.html

[U80] PHP：代码规范修复
来源：http://hz.cashguo.top/gtfgzphwbo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.birdmap.top/gtxljpvcvn.html

[U81] JS：初始化项目
来源：http://hz.birdmap.top/gtuxlxhhyj.html

npm init -y;  npm i express
来源：http://hz.cqqwz.cn/gtqkhchkad.html

[U82] JS：package.json 脚本
来源：http://hz.yonumen.top/gtkzykonaz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jianghu66.top/gtaezryovl.html

[U83] JS：ES Module 导入导出
来源：http://hz.bjfxy.top/gtjlzomkfn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guowangkeji.top/gtamxqjzlt.html

[U84] JS：CommonJS 写法
来源：http://hz.birdmap.top/gtsythxwga.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuxming.cn/gtqwkroyez.html

[U85] JS：可选链
来源：http://hz.shuidangran.top/gtgzvygeoc.html

a?.b?.c
来源：http://hz.ivvv.top/gtrvcsmsda.html

[U86] JS：空值合并
来源：http://hz.gotoacloud.top/gttcdxkttq.html

a ?? b
来源：http://hz.chenzaomai.com/gtaqdxfdwa.html

[U87] JS：解构默认值
来源：http://hz.gaohongyu789.top/gtsntorjbx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shuidangran.top/gtzazmtzqv.html

[U88] JS：对象展开合并
来源：http://hz.birdmap.top/gtxesnxyah.html

{ ...a, ...b }
来源：http://hz.gotoacloud.top/gttozkvxtr.html

[U89] JS：数组去重
来源：http://hz.yj202588.top/gtvmuaysxl.html

[...new Set(arr)]
来源：http://hz.xylfe.cn/gtbugfipbl.html

[U90] JS：数字数组排序
来源：http://hz.cdnleiting.top/gtxnywlfqf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtgyeqqnao.html

[U91] JS：对象键值遍历
来源：http://hz.hywenlv.cn/gtvtkyioqb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhiwuduotai.top/gtiptoiarn.html

[U92] JS：深拷贝
来源：http://hz.meibo888.top/gtnxzxxxjl.html

structuredClone(obj)
来源：http://hz.yj20258.top/gtzeaboqws.html

[U93] JS：模板字符串
来源：http://hz.yanxiufei.cn/gtkkjzemhp.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtwqqdxasu.html

[U94] JS：箭头函数
来源：http://hz.ydzc1.top/gtrqqtbcda.html

const double = x => x * 2;
来源：http://hz.yj20258.top/gteiosardh.html

[U95] JS：Promise 包装
来源：http://hz.smart0.xyz/gtsmsgzsoa.html

new Promise((resolve, reject) => {})
来源：http://hz.meibo888.top/gturmpkmrh.html

[U96] JS：async/await 与异常
来源：http://hz.ywan-chungtsiang.top/gtwgozrnmd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtrtehcxnw.html

[U97] JS：并发请求
来源：http://hz.jyoumei.cn/gtzmrxsefl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtqymtwpzn.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhoulong.xyz/gtnecokghi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shzxlz.cn/gtileisbev.html

[U99] JS：事件监听
来源：http://hz.zhijiandao.cn/gtasgjdxnz.html

el.addEventListener("click", e => {})
来源：http://hz.iojbl.cn/gtztrattrw.html

[U100] JS：DOM 查询
来源：http://hz.pycfn.com/gthklxhihj.html

document.querySelector(".item")
来源：http://hz.guowangkeji.top/gtdioocfua.html

[U101] JS：classList 操作
来源：http://hz.jinqigfzy.top/gticfosdjb.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtgscwlhdk.html

[U102] JS：本地存储
来源：http://hz.ivvv.top/gtpmckvuux.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtmwooeceu.html

[U103] JS：定时器
来源：http://hz.chenzaomai.com/gtbxgrydym.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tanke756.top/gthvkckgqn.html

[U104] JS：防抖
来源：http://hz.wangdashe.top/gtnmvimgng.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtnoiscpfb.html

[U105] JS：节流
来源：http://hz.hnxiangtu.top/gtfprdeinj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhoulong.xyz/gtrupfgpbx.html

[U106] JS：日期格式化
来源：http://hz.pycfn.com/gtuzqqzlkj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yueranfly.top/gthmygfljk.html

[U107] JS：数字千分位
来源：http://hz.fzhhl.top/gtaclgifls.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtabbobero.html

[U108] JS：随机整数
来源：http://hz.mhx1999.top/gtkskhwznv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gzhubu.top/gtkbmzwyjz.html

[U109] JS：数组分组
来源：http://hz.jqgufenzy.top/gtzcrfyvnu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtpvtaqhui.html

[U110] JS：数组分块
来源：http://hz.cashguo.top/gtregyvjhp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhaomingkeji.xyz/gtmvrvqorw.html

[U111] JS：对象转 Map
来源：http://hz.hongshengwenyu.top/gttzapibel.html

new Map(Object.entries(obj))
来源：http://hz.yanxiufei.cn/gtvusrolyq.html

[U112] JS：字符串补位
来源：http://hz.yangfankeji.com/gtkcpygmmv.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtxxolhqzv.html

[U113] JS：正则替换全部
来源：http://hz.ybcxt.top/gtjpghpgmy.html

s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtovgpyqkt.html

[U114] JS：JSON 深比较
来源：http://hz.pycfn.com/gtixdqsdbv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daria6918.cn/gtffbcoqkx.html

[U115] JS：生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtqiibmyvg.html

crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtmthkeqgl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.0kj1m.cn/gttgqjhbnm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daria6918.cn/gtsgohrche.html

[U117] JS：单元测试
来源：http://hz.chenjidiqi.icu/gtucwntmuu.html

npm i -D vitest;  npx vitest
来源：http://hz.hysaishi.cn/gtkcpifiiv.html

[U118] JS：开发服务器
来源：http://hz.vqdsnc.cn/gtjvmhlxnn.html

npm i -D vite;  npx vite
来源：http://hz.wangshuangyany.cn/gtizrvhyfi.html

[U119] JS：生产构建
来源：http://hz.cqqwz.cn/gtmlmwpaza.html

npx vite build
来源：http://hz.sxryk.cn/gtdthpdqtp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenlongwang.top/gtdbgcwnzq.html

import.meta.env.VITE_API_URL
来源：http://hz.hongshengwenyu.top/gtqbchtzvq.html

================================================================================
来源：http://hz.dashuyun.cn/gtcqkqglhi.html

统计汇总
来源：http://hz.jlsjyb.cn/gteoerfhfr.html

================================================================================
来源：http://hz.yvedp.cn/gtooqxpjix.html

按语言统计（条）：
来源：http://hz.zhengqikj.top/gtnujdtjjr.html

Python ......... 252
来源：http://hz.zhaomingkeji.xyz/gtgiqgcbow.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtxmylwkuh.html

JavaScript ..... 252
来源：http://hz.yuanzhike.top/gthidogvuh.html

TypeScript ..... 212
来源：http://hz.0kj1m.cn/gtvqljvtgo.html

Java ........... 212
来源：http://hz.316326.xyz/gtyxxcsgjz.html

Go ............. 212
来源：http://hz.bjfxy.top/gtiozqcnrq.html

Ruby ........... 212
来源：http://hz.316326.xyz/gtlfwoxewo.html

C# ............. 212
来源：http://hz.guowangkeji.top/gtjfkojuik.html

C .............. 30
来源：http://hz.52xcode.cn/gtdlklkhkz.html

C++ ............ 30
来源：http://hz.zhongyouzk.top/gtpoaobynd.html

SQL ............ 90
来源：http://hz.tianlin.xyz/gtpkivccep.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtfchjpgid.html

Kotlin ......... 15
来源：http://hz.zhijiandao.cn/gtpzhdaszu.html

Swift .......... 15
来源：http://hz.pengpengdd.cyou/gtufvsmjbz.html

Lua ............ 10
来源：http://hz.xuanzx.com/gtxugltuom.html

Perl ........... 10
来源：http://hz.xylfe.cn/gtiylndafi.html

Scala .......... 10
来源：http://hz.9152youxi.cn/gtnzzqffsk.html

------------------------------------
来源：http://hz.fengsongda.top/gtdljwpndp.html

合计 ........... 2106 条
来源：http://hz.sxryk.cn/gtgyxamhuw.html

按章节统计：
来源：http://hz.daria6918.cn/gtapyvswte.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gtozjnzspg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtzxuqchco.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtummzgfud.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtsxzugudq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtwwbsuhah.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtfnazoiay.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtnpoadypt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.birdmap.top/gtszqqeutx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtoxroatkg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gtnieakzbq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtezogebkg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtqpvctfjm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtnxrtawxo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gteqkuzmef.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgufenzy.top/gtdxxkrxnf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtwkswumoq.html

Q SQL 专题                              90
来源：http://hz.smart0.xyz/gtfshqhgso.html

R Bash 专题                             80
来源：http://hz.dashuyun.cn/gtbihcfxgh.html

S C / C++ 专题                          60
来源：http://hz.chenzaomai.com/gtpbeesexc.html

T 其他语言补充                          60
来源：http://hz.zhijiandao.cn/gtvdwuroox.html

U 高频实用片段                         120
来源：http://hz.zhijiandao.cn/gtevfxomiu.html

------------------------------------
来源：http://hz.ehwqpu.com/gtgvmjoiyf.html

合计                                  2106 条
来源：http://hz.quarkkingdee.top/gtnikhffzw.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtxjipsbtj.html

使用提醒
来源：http://hz.hnqzz.top/gtlrkhvula.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gteqoysvxp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hysaishi.cn/gthnntlysl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj20258.top/gtwxxdwbpe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.9152youxi.cn/gtaplsosbx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinyuanbaomall.cn/gtvwkzgcmb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tanke756.top/gtgkkbochq.html

—— 文件结束 ——
来源：http://hz.0kj1m.cn/gtzmqtzaah.html

================================================================================
来源：http://hz.dashuyun.cn/gtquupuzfs.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.bjfxy.top/gtiltrcotx.html

Common Programming Examples Cheat Book
来源：http://hz.guowangkeji.top/gtyzxjpxrq.html

================================================================================
来源：http://hz.pycfn.com/gtjnyggbcd.html

【收录内容】
来源：http://hz.52xcode.cn/gtcwslsmbv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ybcxt.top/gtdsnnuhmi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.guannengcc.top/gtvaxemdlg.html

SQL · Bash · C · C++
来源：http://hz.meibo888.top/gtxpccnxlq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gtacgdwzsa.html

【使用说明】
来源：http://hz.fengsongda.top/gtzwiwzzwg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.tianlin.xyz/gtzbjxblsx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gotoacloud.top/gtncgzcmav.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj202588.top/gtcgzczgbk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.birdmap.top/gtxqoacrbj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hfpthk.cn/gtynqumdga.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhiwuduotai.top/gtbybfbgcj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yvedp.cn/gtcuicoqbt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aizwys.cn/gtsoodzafp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj20258888.top/gtrbcckedv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj20258.top/gtcigbbrgu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.sxryk.cn/gttybpdftw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aibaodan.cn/gtwucfwnax.html

【文件统计】
来源：http://hz.hongshengwenyu.top/gtngjsfjtz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.redwolf501.top/gtljzqmaqv.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtemeddcjc.html

目  录
来源：http://hz.xuanzx.com/gtmaejqdvi.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtaqlfuwmq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtwxrqrrxf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtoxlkltke.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.tianlin.xyz/gtepeogpvm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtzcvxover.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.chenjidiqi.icu/gtojvzpusx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtajgetgir.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtxqfkrftv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhixingplan.top/gtnxqhogfd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtfydpxaqn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.fengsongda.top/gthqjmetpr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtqegirrov.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gtqukcontb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtkyrheayx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.nanxinkj.top/gtnqofaoov.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nwbrower.top/gtqsdvlmte.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtaevxdfds.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shanyushiyangkeji.top/gtylyspsbw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.kuanghao11.cn/gtabumumii.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhixingplan.top/gtjovyuaoz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtbepvvoid.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ppjwa.cn/gtnvsgsnau.html

================================================================================
来源：http://hz.xuanzx.com/gttqomofeh.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtdwwwyuzf.html

================================================================================
来源：http://hz.yangfankeji.com/gtspldiidq.html

[A01] Hello World
来源：http://hz.vqdsnc.cn/gtsdofhmpr.html

Py:   print("Hello, World!")
来源：http://hz.ppjwa.cn/gtpnuunfjf.html

PHP:  echo "Hello, World!";
来源：http://hz.snrcjt.cn/gtxfrajzjn.html

JS:   console.log("Hello, World!");
来源：http://hz.fengsongda.top/gtrvgreiqg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shanyushiyangkeji.top/gtgeorojsr.html

Java: System.out.println("Hello, World!");
来源：http://hz.jlsjyb.cn/gtocezehxv.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xylfe.cn/gtxhahdmmg.html

Ruby: puts "Hello, World!"
来源：http://hz.meibo888.top/gtfzmurlfg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cdnleiting.top/gtslmpmyrf.html

[A02] 变量声明与赋值
来源：http://hz.ywan-chungtsiang.top/gtneutisfw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.chenlongwang.top/gtjtbdvzri.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.svipenyu.cn/gtegohdzax.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sufxvd.cn/gtdvavrroo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.9152youxi.cn/gtftqywizs.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gtflapzrja.html

Go:   name := "Alex"; age := 20
来源：http://hz.hfpthk.cn/gtyospkhun.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhongyouzk.top/gtwwcpykcx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.feifeiyinyue.top/gtcezskwgc.html

[A03] 常量定义
来源：http://hz.yangfankeji.com/gtfnuptopn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.shangyingyoupin.top/gtsczohjyi.html

PHP:  const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtyfjeahxh.html

JS:   const PI = 3.14159;
来源：http://hz.dashuyun.cn/gteqfakhlq.html

TS:   const PI: number = 3.14159;
来源：http://hz.316326.xyz/gtlpzmuxvj.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtatvidqze.html

Go:   const PI = 3.14159
来源：http://hz.zycfv.cn/gtrlmyzqye.html

Ruby: PI = 3.14159
来源：http://hz.cashguo.top/gtogaiaduy.html

C#:   const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtkitovbqw.html

[A04] 判断变量类型
来源：http://hz.yj20258.top/gtjztkavpk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhiwuduotai.top/gtijfbuzbi.html


<!-- 参考信息 -->