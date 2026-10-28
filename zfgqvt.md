代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.haohaochexian.top/gtefdzqehh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gterctafii.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtxnkymnma.html

?string $name = null
来源：http://hz.zhongyouzk.top/gtkcienjzd.html

[U47] PHP：联合类型
来源：http://hz.0kj1m.cn/gtlyemzacq.html

int|string $id
来源：http://hz.snrcjt.cn/gtnhxgwtxd.html

[U48] PHP：纯枚举
来源：http://hz.cdnleiting.top/gtalfaiapd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtypxeqthj.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gtfizxpphg.html

public readonly string $name
来源：http://hz.sxryk.cn/gtnsfbxlyz.html

[U50] PHP：构造器属性提升
来源：http://hz.dianchejie.cn/gtsjpzcsdh.html

public function __construct(private int $id) {}
来源：http://hz.ehwqpu.com/gtlpdyjjrm.html

[U51] PHP：数组解构
来源：http://hz.ydzc1.top/gtqhkaceqb.html

[$a, $b] = $arr;
来源：http://hz.gotoacloud.top/gtijpxuqwn.html

[U52] PHP：箭头函数
来源：http://hz.yueranfly.top/gtjyvkaoby.html

$double = fn($x) => $x * 2;
来源：http://hz.zhoulong.xyz/gthtlhrokv.html

[U53] PHP：空合并运算符
来源：http://hz.ppjwa.cn/gtuplptxqt.html

$v = $a ?? $b ?? "default";
来源：http://hz.birdmap.top/gtpkezeteh.html

[U54] PHP：空安全调用
来源：http://hz.zhengqikj.top/gtlymbfhsx.html

$obj?->method()
来源：http://hz.ydzc1.top/gtqkkadfrz.html

[U55] PHP：match 表达式
来源：http://hz.redwolf501.top/gtoftmwfxl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jiagoushi.top/gtxdvikuve.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gtpuhdsduz.html

f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtfjljstpf.html

[U57] PHP：字符串插值
来源：http://hz.zhongyouzk.top/gtfzmcefao.html

"值: {$a}"
来源：http://hz.jinqigfzy.top/gtunwtdjon.html

[U58] PHP：数组三件套
来源：http://hz.sxryk.cn/gtpuhhwquf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tanke756.top/gtufailxnf.html

[U59] PHP：自定义排序
来源：http://hz.jinghuilouyu.cn/gtqujrydbf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtbrfvmhis.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtmygsntwt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.mhx1999.top/gtxldvgdho.html

[U61] PHP：正则
来源：http://hz.zhongyouzk.top/gtnkbpenyo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gttyydgtrh.html

[U62] PHP：日期对象
来源：http://hz.birdmap.top/gtqjhgluyv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hfpthk.cn/gthdrnnbew.html

[U63] PHP：文件读写
来源：http://hz.chenlongwang.top/gtwisswwud.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zycfv.cn/gtcakjuqua.html

[U64] PHP：目录遍历
来源：http://hz.tanke756.top/gtjuhpboea.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gtgkpkxbyp.html

[U65] PHP：会话
来源：http://hz.tanke756.top/gtkfkqpfqc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.haohaochexian.top/gtajttgapj.html

[U66] PHP：设置 Cookie
来源：http://hz.dashuyun.cn/gtegfyywhd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuxming.cn/gtosadrmyh.html

[U67] PHP：处理文件上传
来源：http://hz.yuanzhike.top/gtjdmjbwos.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jlsjyb.cn/gtdvimdnar.html

[U68] PHP：PDO 连接
来源：http://hz.ywan-chungtsiang.top/gtkscqcvwj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenlongwang.top/gtlshstvxq.html

[U69] PHP：PDO 预处理
来源：http://hz.ehwqpu.com/gtcwtpfzsz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.bjfxy.top/gtppwcpqkj.html

[U70] PHP：PDO 事务
来源：http://hz.hfpthk.cn/gtfnvjnmzd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhengqikj.top/gtbdjhkpir.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gthkkpfjwt.html

throw new RuntimeException("失败", 500);
来源：http://hz.daria6918.cn/gtbdillqfz.html

[U72] PHP：写错误日志
来源：http://hz.shzxlz.cn/gtictdvbap.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daria6918.cn/gtgwutpydk.html

[U73] PHP：读取 ini 配置
来源：http://hz.guowangkeji.top/gtjubswvjb.html

parse_ini_file("config.ini", true)
来源：http://hz.zhongyouzk.top/gtekvfdjzh.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtkdrbikeg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shuidangran.top/gtnzaxhgpo.html

[U75] PHP：依赖注入
来源：http://hz.jinyuanbaomall.cn/gtgcuguxua.html

composer require psr/container
来源：http://hz.pengpengdd.cyou/gtmqwyryac.html

[U76] PHP：简单路由
来源：http://hz.ywan-chungtsiang.top/gtztjpbqly.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gtvcwhxicu.html

[U77] PHP：模板渲染
来源：http://hz.ydzc1.top/gthjeatvyz.html

composer require twig/twig
来源：http://hz.chenzaomai.com/gthdzplpjr.html

[U78] PHP：单元测试
来源：http://hz.jqgufenzy.top/gtnvrusbqc.html

composer require --dev phpunit/phpunit
来源：http://hz.wangdashe.top/gtaobempoe.html

[U79] PHP：静态分析
来源：http://hz.sufxvd.cn/gtqazlqata.html

composer require --dev phpstan/phpstan
来源：http://hz.cheryme.top/gtslbabwnq.html

[U80] PHP：代码规范修复
来源：http://hz.xuetiantiany.cn/gtilazakwk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhaomingkeji.xyz/gtpgsmxaqb.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtjwewcboy.html

npm init -y;  npm i express
来源：http://hz.haohaochexian.top/gtmzwxigxs.html

[U82] JS：package.json 脚本
来源：http://hz.hongshengwenyu.top/gttsoloytb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cdnleiting.top/gtbxyvfzgo.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydzc1.top/gttaypjhwv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yonumen.top/gtluupaada.html

[U84] JS：CommonJS 写法
来源：http://hz.andypj.xyz/gtnvkbiwbt.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.iojbl.cn/gtjdsihtwb.html

[U85] JS：可选链
来源：http://hz.jinqigufen.top/gttsfzdtnz.html

a?.b?.c
来源：http://hz.fengsongda.top/gtgoyezizg.html

[U86] JS：空值合并
来源：http://hz.aibaodan.cn/gterppudcz.html

a ?? b
来源：http://hz.mhx1999.top/gtuszvlasu.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gtcececbzg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.kuanghao11.cn/gtunnetrua.html

[U88] JS：对象展开合并
来源：http://hz.wangdashe.top/gtucukdmoe.html

{ ...a, ...b }
来源：http://hz.jqgfzy.top/gtreydtxnw.html

[U89] JS：数组去重
来源：http://hz.havefunace.top/gtlmqskcpi.html

[...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gttylofpqu.html

[U90] JS：数字数组排序
来源：http://hz.xuanzx.com/gtieravxae.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtitjlyvzf.html

[U91] JS：对象键值遍历
来源：http://hz.feifeiyinyue.top/gtzjhasccr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.andypj.xyz/gtrghotqxh.html

[U92] JS：深拷贝
来源：http://hz.c1oappe.top/gthuyoujoz.html

structuredClone(obj)
来源：http://hz.havefunace.top/gtymhmsrwj.html

[U93] JS：模板字符串
来源：http://hz.svipenyu.cn/gtrzeabgzv.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtntxehkfq.html

[U94] JS：箭头函数
来源：http://hz.dianchejie.cn/gtsgqphaah.html

const double = x => x * 2;
来源：http://hz.birdmap.top/gtjermrhwe.html

[U95] JS：Promise 包装
来源：http://hz.cqqwz.cn/gtfslikrbe.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtiyecqwql.html

[U96] JS：async/await 与异常
来源：http://hz.cheryme.top/gtqlumyuel.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtdgyuebls.html

[U97] JS：并发请求
来源：http://hz.jlsjyb.cn/gtkttcleuu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtxanoagfs.html

[U98] JS：fetch 带 JSON
来源：http://hz.ivvv.top/gtcqvqjykq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhijiandao.cn/gtrbnvbroa.html

[U99] JS：事件监听
来源：http://hz.yuxming.cn/gtujrkusal.html

el.addEventListener("click", e => {})
来源：http://hz.ywan-chungtsiang.top/gtvotnbpgu.html

[U100] JS：DOM 查询
来源：http://hz.xuanzx.com/gtiryzzqkr.html

document.querySelector(".item")
来源：http://hz.ivvv.top/gtmlxrzuaw.html

[U101] JS：classList 操作
来源：http://hz.sweek.top/gtkxrskuuw.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gttpbbcyfb.html

[U102] JS：本地存储
来源：http://hz.nanxuanxn.top/gtjkzgvegu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258888.top/gtdiujaqoi.html

[U103] JS：定时器
来源：http://hz.yj20258888.top/gtaiulnjih.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenjidiqi.icu/gtgrabfsqr.html

[U104] JS：防抖
来源：http://hz.gogol.net.cn/gtsesapoww.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtlvnstbll.html

[U105] JS：节流
来源：http://hz.jqgufenzy.top/gtyvcpxdoi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.meibo888.top/gtniefkjtx.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gtszcqujqb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnqzz.top/gthoebwfec.html

[U107] JS：数字千分位
来源：http://hz.cqqwz.cn/gtlufzbpqr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shzxlz.cn/gtunpushgi.html

[U108] JS：随机整数
来源：http://hz.nwbrower.top/gtbfkgrpey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigfzy.top/gtnmjpqwnp.html

[U109] JS：数组分组
来源：http://hz.gaohongyu789.top/gtomuvqmgp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtvprdswom.html

[U110] JS：数组分块
来源：http://hz.redwolf501.top/gtqrnbxtyl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuanzhike.top/gtdayhbohw.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtlovgkcsh.html

new Map(Object.entries(obj))
来源：http://hz.316326.xyz/gtpympnwwp.html

[U112] JS：字符串补位
来源：http://hz.cheryme.top/gtkpadzjfk.html

"7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtotoszsrt.html

[U113] JS：正则替换全部
来源：http://hz.jinghuilouyu.cn/gthuhcpjou.html

s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtxkrwbhzo.html

[U114] JS：JSON 深比较
来源：http://hz.nwbrower.top/gtimdbhaig.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtliewsdxc.html

[U115] JS：生成 UUID
来源：http://hz.xuetiantiany.cn/gteuovlqos.html

crypto.randomUUID()
来源：http://hz.316326.xyz/gthykbmbyn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jlsjyb.cn/gtxfkhvwxz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.wangdashe.top/gtebhfnwju.html

[U117] JS：单元测试
来源：http://hz.zycfv.cn/gtfnjxeode.html

npm i -D vitest;  npx vitest
来源：http://hz.bjfxy.top/gtvyynwzlx.html

[U118] JS：开发服务器
来源：http://hz.xuetiantiany.cn/gtueojnrou.html

npm i -D vite;  npx vite
来源：http://hz.ivvv.top/gtljbgybjo.html

[U119] JS：生产构建
来源：http://hz.gotoacloud.top/gtcxsfjvpz.html

npx vite build
来源：http://hz.cucudq.cn/gtalcskwee.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sysykeji.top/gtszicsrpw.html

import.meta.env.VITE_API_URL
来源：http://hz.sysykeji.top/gtfblbvwgp.html

================================================================================
来源：http://hz.9152youxi.cn/gtabaofsuf.html

统计汇总
来源：http://hz.hammf.cn/gtntzsonqz.html

================================================================================
来源：http://hz.mhx1999.top/gtgimncqbd.html

按语言统计（条）：
来源：http://hz.hfpthk.cn/gtijyfwjmg.html

Python ......... 252
来源：http://hz.zycfv.cn/gtiqrphxku.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gtoxtdlrpw.html

JavaScript ..... 252
来源：http://hz.fengsongda.top/gtvvfadeau.html

TypeScript ..... 212
来源：http://hz.fengsongda.top/gtesnmmtpx.html

Java ........... 212
来源：http://hz.jinqigufen.top/gtfsgqvvgm.html

Go ............. 212
来源：http://hz.sweek.top/gtvaggrjly.html

Ruby ........... 212
来源：http://hz.zdqjudy.top/gttxfoatcq.html

C# ............. 212
来源：http://hz.chenjidiqi.icu/gtulnjjlmo.html

C .............. 30
来源：http://hz.zhoulong.xyz/gtlypqnjsp.html

C++ ............ 30
来源：http://hz.hnqzz.top/gtbfqdphnm.html

SQL ............ 90
来源：http://hz.ybcxt.top/gtswvkoivu.html

Bash ........... 80
来源：http://hz.aizwys.cn/gtsetopwao.html

Kotlin ......... 15
来源：http://hz.shuidangran.top/gtzohigjgs.html

Swift .......... 15
来源：http://hz.pycfn.com/gtcavvexso.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gtzdtbjwzk.html

Perl ........... 10
来源：http://hz.nanxinkj.top/gtzeqwbvjd.html

Scala .......... 10
来源：http://hz.jinghuilouyu.cn/gtaoiastbb.html

------------------------------------
来源：http://hz.jiagoushi.top/gtvsjaufiv.html

合计 ........... 2106 条
来源：http://hz.jinqigfzy.top/gtxasqvawg.html

按章节统计：
来源：http://hz.yuanzhike.top/gtqjopkqmw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shzxlz.cn/gtthpleaag.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtyvphvaqm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtgagdtvjy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shzxlz.cn/gtgkgvouci.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xuanzx.com/gtdvrnmlmd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.havefunace.top/gtcfyjyeyb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtlilvbuny.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtzlowzxro.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gttqdnwfby.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.dianchejie.cn/gtwcrngxvl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtwxwftjep.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtqbxxjfwt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtngkbpfsm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.haohaochexian.top/gtyyxnggmt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shangyingyoupin.top/gtqrzxofiu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gtnnfbifid.html

Q SQL 专题                              90
来源：http://hz.jyoumei.cn/gtcjsfukcj.html

R Bash 专题                             80
来源：http://hz.xuetiantiany.cn/gtzqohiivr.html

S C / C++ 专题                          60
来源：http://hz.snrcjt.cn/gtzvwqhkom.html

T 其他语言补充                          60
来源：http://hz.hysaishi.cn/gtmfkpzihz.html

U 高频实用片段                         120
来源：http://hz.aibaodan.cn/gtjockycxh.html

------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtvkppxxqc.html

合计                                  2106 条
来源：http://hz.haohaochexian.top/gtzlrlazhy.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtytizzsdq.html

使用提醒
来源：http://hz.jlsjyb.cn/gtdockjdva.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtumadnrog.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj202588.top/gtgdllqufr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinyuanbaomall.cn/gtbnbcgcva.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sufxvd.cn/gtdkhfxwsh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cqqwz.cn/gtzskbwrdr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.9152youxi.cn/gtesebqapb.html

—— 文件结束 ——
来源：http://hz.cdnleiting.top/gtkgcwqxyb.html

================================================================================
来源：http://hz.zycfv.cn/gtzzusazkm.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nanxinkj.top/gtzpvasnzj.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigufen.top/gtazubmvka.html

================================================================================
来源：http://hz.yangfankeji.com/gtyrsnsbew.html

【收录内容】
来源：http://hz.c1oappe.top/gtilujchuo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gzhubu.top/gtqxhrqeio.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nanxinkj.top/gtmnkyoeqr.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gtcfdevwkc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.smart0.xyz/gtjefnixtz.html

【使用说明】
来源：http://hz.yueranfly.top/gtslequgvf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuanzhike.top/gtolilktbj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yueranfly.top/gtnmukqzwv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.iojbl.cn/gtglfvrepu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.svipenyu.cn/gtguvkpafd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xuanzx.com/gtrvscngte.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.iojbl.cn/gtnitfmyoj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtihwekggg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yueranfly.top/gtltpnpbxb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hammf.cn/gtedldqqva.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.smart0.xyz/gtaoydzidh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.quarkkingdee.top/gtkdhidfhx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.chenjidiqi.icu/gtoqkyoeal.html

【文件统计】
来源：http://hz.daria6918.cn/gttaajnabv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zycfv.cn/gtylmipqkc.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtkwyikuqd.html

目  录
来源：http://hz.yj202588.top/gtnrltyqyk.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtifsbasfn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nwbrower.top/gtxvbnxeip.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.tianlin.xyz/gtblzleblk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtifkpsaew.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.chenlongwang.top/gttjfmiexu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sweek.top/gtwkquisre.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yonumen.top/gtyroegnjk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtzemupbny.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yonumen.top/gtkeekxnve.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtgozglmcv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zycfv.cn/gtfjfrajwf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtuvwtozgq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gthxlxdxlc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtdyngnnxn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ppjwa.cn/gtwrggohcj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.smart0.xyz/gtmvogqtmg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtxphdrarn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.havefunace.top/gtcjjhjxgv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.c1oappe.top/gtteuecbrz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jyoumei.cn/gtsfubveum.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gtzbymsgyv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtuzbpxsrm.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtyygnyyir.html

A. 基础语法与类型
来源：http://hz.zhengqikj.top/gtlwytffli.html

================================================================================
来源：http://hz.shzxlz.cn/gttjlpgzmv.html

[A01] Hello World
来源：http://hz.kuanghao11.cn/gtjbynevul.html

Py:   print("Hello, World!")
来源：http://hz.vqdsnc.cn/gtftmdkfkb.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigfzy.top/gtkdlqcrdf.html

JS:   console.log("Hello, World!");
来源：http://hz.dashuyun.cn/gttjzlhwdw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jyoumei.cn/gthdqrorlr.html

Java: System.out.println("Hello, World!");
来源：http://hz.ydjk.org.cn/gthfftashl.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.mhx1999.top/gtdjxlrrfu.html

Ruby: puts "Hello, World!"
来源：http://hz.sxryk.cn/gtmbpmqvbi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.andypj.xyz/gtgzbgtksq.html

[A02] 变量声明与赋值
来源：http://hz.0kj1m.cn/gtwktxuvuu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.wangdashe.top/gtdpmtxykc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ppjwa.cn/gtrdptydmx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuetiantiany.cn/gtutrvenxb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.quarkkingdee.top/gtenyfvbyl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gtikuleszg.html

Go:   name := "Alex"; age := 20
来源：http://hz.ybcxt.top/gtxvtbgsgu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ivvv.top/gtijlcoelu.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yj202588.top/gtyzvxtpno.html

[A03] 常量定义
来源：http://hz.sweek.top/gtqtnaqsqy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xuetiantiany.cn/gtoahkczqh.html

PHP:  const PI = 3.14159;
来源：http://hz.guannengcc.top/gtpwelwskt.html

JS:   const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtjztiqblk.html

TS:   const PI: number = 3.14159;
来源：http://hz.andypj.xyz/gtpnqzpkxq.html

Java: static final double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtspqppuay.html

Go:   const PI = 3.14159
来源：http://hz.ydjk.org.cn/gtwbyuruxz.html

Ruby: PI = 3.14159
来源：http://hz.gzhubu.top/gtgmvncztb.html

C#:   const double PI = 3.14159;
来源：http://hz.cashguo.top/gteyjupymi.html

[A04] 判断变量类型
来源：http://hz.pycfn.com/gtsctefnnq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.316326.xyz/gtfuqtyers.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.daria6918.cn/gturlpwjfi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gzhubu.top/gtpbmyzdac.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhengqikj.top/gtbcdoxdql.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.9152youxi.cn/gtywsnfafv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shangyingyoupin.top/gtpdiskitr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.aizwys.cn/gtsrzsxxlo.html

C#:   x.GetType().Name; x is int
来源：http://hz.dianchejie.cn/gtfxsonlij.html

[A05] 整数除法与取模
来源：http://hz.52xcode.cn/gtlyirwecz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gogol.net.cn/gtthbunyjc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.52xcode.cn/gttrhzxdkf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtmelqknfe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hongshengwenyu.top/gtjrumknkv.html


<!-- 参考信息 -->