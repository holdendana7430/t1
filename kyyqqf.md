代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.daria6918.cn/gthcaecpfa.html

namespace App\Http;
来源：http://hz.havefunace.top/gtrwvtvzzq.html

[U44] PHP：开启严格类型
来源：http://hz.zhaomingkeji.xyz/gtohiytquf.html

declare(strict_types=1);
来源：http://hz.tanke756.top/gtzphcgppj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhongyouzk.top/gtmgkzcwea.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtlrzsfruz.html

[U46] PHP：可空类型
来源：http://hz.zhaomingkeji.xyz/gttzpjinsn.html

?string $name = null
来源：http://hz.jinqigufen.top/gtdrdjblkd.html

[U47] PHP：联合类型
来源：http://hz.cheryme.top/gtofgkpwti.html

int|string $id
来源：http://hz.zhoulong.xyz/gttfdovoge.html

[U48] PHP：纯枚举
来源：http://hz.jinyuanbaomall.cn/gtvccbnzsh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yvedp.cn/gtayzztfxr.html

[U49] PHP：只读属性
来源：http://hz.birdmap.top/gtbjinsugg.html

public readonly string $name
来源：http://hz.ybcxt.top/gtvznwncuf.html

[U50] PHP：构造器属性提升
来源：http://hz.jianghu66.top/gtoroeudst.html

public function __construct(private int $id) {}
来源：http://hz.pengpengdd.cyou/gtuebffhcm.html

[U51] PHP：数组解构
来源：http://hz.cashguo.top/gtcqwsizsw.html

[$a, $b] = $arr;
来源：http://hz.kuanghao11.cn/gtqlwnfbxx.html

[U52] PHP：箭头函数
来源：http://hz.dianchejie.cn/gtuvllkaql.html

$double = fn($x) => $x * 2;
来源：http://hz.jinyuanbaomall.cn/gthmprwvkc.html

[U53] PHP：空合并运算符
来源：http://hz.redwolf501.top/gtycsvhgjv.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinyuanbaomall.cn/gtrqzmruuc.html

[U54] PHP：空安全调用
来源：http://hz.wangdashe.top/gtmfwzesgt.html

$obj?->method()
来源：http://hz.redwolf501.top/gtewbtrsqp.html

[U55] PHP：match 表达式
来源：http://hz.xinyue.icu/gtfdcwtnqc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cdnleiting.top/gtkvofrotm.html

[U56] PHP：命名参数
来源：http://hz.zhoulong.xyz/gtvbbucmpc.html

f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtbexvzviw.html

[U57] PHP：字符串插值
来源：http://hz.sysykeji.top/gtoheqikhu.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtpsjbwols.html

[U58] PHP：数组三件套
来源：http://hz.cashguo.top/gthbgseidv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.svipenyu.cn/gtplnbdydg.html

[U59] PHP：自定义排序
来源：http://hz.meibo888.top/gtyyoxliyl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenzaomai.com/gtbkpyryyc.html

[U60] PHP：JSON 编解码
来源：http://hz.cashguo.top/gtxktmguzy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gogol.net.cn/gtgqblxeiw.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtdckjyhrn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtdmtbxrlz.html

[U62] PHP：日期对象
来源：http://hz.jinyuanbaomall.cn/gtvnybeuco.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guannengcc.top/gtdwpiqlgj.html

[U63] PHP：文件读写
来源：http://hz.kuanghao11.cn/gtklvaalmi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.316326.xyz/gtifucfjji.html

[U64] PHP：目录遍历
来源：http://hz.chenjidiqi.icu/gtookzmdbq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hywenlv.cn/gtofygjjyb.html

[U65] PHP：会话
来源：http://hz.birdmap.top/gteujotgsf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zdqjudy.top/gtiussbtlh.html

[U66] PHP：设置 Cookie
来源：http://hz.ywan-chungtsiang.top/gtjxajjvxa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.snrcjt.cn/gtxvmjqcew.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gtufwiczvr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangshuangyany.cn/gtqtskuufd.html

[U68] PHP：PDO 连接
来源：http://hz.tanke756.top/gtyvbouqdx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.redwolf501.top/gtreutrvtv.html

[U69] PHP：PDO 预处理
来源：http://hz.yuanzhike.top/gtvsznbgkb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.chenlongwang.top/gtblbofotj.html

[U70] PHP：PDO 事务
来源：http://hz.sweek.top/gtzpenjkqb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cdnleiting.top/gtybtpibgt.html

[U71] PHP：抛出异常
来源：http://hz.yueranfly.top/gtdkedzdzd.html

throw new RuntimeException("失败", 500);
来源：http://hz.shuidangran.top/gtztkzmimb.html

[U72] PHP：写错误日志
来源：http://hz.bjfxy.top/gtewdebnxp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.mhx1999.top/gttagnbfjo.html

[U73] PHP：读取 ini 配置
来源：http://hz.iojbl.cn/gtnntqsmai.html

parse_ini_file("config.ini", true)
来源：http://hz.dashuyun.cn/gtbqyzusrd.html

[U74] PHP：读取环境变量
来源：http://hz.havefunace.top/gtspzhwxgi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shuidangran.top/gtbhmrmdpt.html

[U75] PHP：依赖注入
来源：http://hz.zhixingplan.top/gtyrskipbm.html

composer require psr/container
来源：http://hz.daxiang520.top/gtfwmgrrze.html

[U76] PHP：简单路由
来源：http://hz.jinyuanbaomall.cn/gtoajuldgl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jiagoushi.top/gtjamnxjko.html

[U77] PHP：模板渲染
来源：http://hz.fzhhl.top/gtgtpqjdju.html

composer require twig/twig
来源：http://hz.shzxlz.cn/gtdwaohqgo.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gtrjjlwtju.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangkeji.top/gtqrebjdvr.html

[U79] PHP：静态分析
来源：http://hz.yuxming.cn/gtnvhdzcun.html

composer require --dev phpstan/phpstan
来源：http://hz.dianchejie.cn/gtxdhmcssh.html

[U80] PHP：代码规范修复
来源：http://hz.kuanghao11.cn/gtdpnvgemg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.guowangkeji.top/gtddtyqnpw.html

[U81] JS：初始化项目
来源：http://hz.cucudq.cn/gtuixuvqre.html

npm init -y;  npm i express
来源：http://hz.hongshengwenyu.top/gtkfdofazs.html

[U82] JS：package.json 脚本
来源：http://hz.zhijiandao.cn/gtvbzbbpsm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtqrmkxmdr.html

[U83] JS：ES Module 导入导出
来源：http://hz.vqdsnc.cn/gtuqvnrbju.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.pengpengdd.cyou/gtjfrzuisd.html

[U84] JS：CommonJS 写法
来源：http://hz.chenzaomai.com/gthqqzksqs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.c1oappe.top/gtjulzzivo.html

[U85] JS：可选链
来源：http://hz.sysykeji.top/gtudcnxgyf.html

a?.b?.c
来源：http://hz.chenjidiqi.icu/gtpxkbnoor.html

[U86] JS：空值合并
来源：http://hz.yueranfly.top/gttcmavjhq.html

a ?? b
来源：http://hz.yangfankeji.com/gtttnvfhhj.html

[U87] JS：解构默认值
来源：http://hz.ywan-chungtsiang.top/gtaqganuzi.html

const { a = 1, b = 2 } = obj;
来源：http://hz.fzhhl.top/gtxhqkobfw.html

[U88] JS：对象展开合并
来源：http://hz.tian-w.cn/gtdnxpujeg.html

{ ...a, ...b }
来源：http://hz.ppjwa.cn/gteaxfrpnx.html

[U89] JS：数组去重
来源：http://hz.yvedp.cn/gtyvxhjqqk.html

[...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtvjhvxspp.html

[U90] JS：数字数组排序
来源：http://hz.wangshuangyany.cn/gtguiurjgl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtewfuenaq.html

[U91] JS：对象键值遍历
来源：http://hz.hnqzz.top/gtmssrcjpy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinqigfzy.top/gtxnwmtmtr.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtrobosvrh.html

structuredClone(obj)
来源：http://hz.yongpay.top/gtrxukfdid.html

[U93] JS：模板字符串
来源：http://hz.vqdsnc.cn/gtgxaugwyx.html

`共 ${n} 条`
来源：http://hz.tian-w.cn/gtoidubuso.html

[U94] JS：箭头函数
来源：http://hz.jiagoushi.top/gtfupbnqqe.html

const double = x => x * 2;
来源：http://hz.yj202588.top/gtdsgbgjyq.html

[U95] JS：Promise 包装
来源：http://hz.svipenyu.cn/gtavrpywri.html

new Promise((resolve, reject) => {})
来源：http://hz.snrcjt.cn/gtbgsjzwrd.html

[U96] JS：async/await 与异常
来源：http://hz.gzhubu.top/gtzpilludk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtnyinuxhc.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtvrlbkrgp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtuajnaymk.html

[U98] JS：fetch 带 JSON
来源：http://hz.meibo888.top/gtoqehsixo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jianghu66.top/gtmkgkclkp.html

[U99] JS：事件监听
来源：http://hz.shanyushiyangtech.top/gtzxynlmbb.html

el.addEventListener("click", e => {})
来源：http://hz.iojbl.cn/gtloboqakv.html

[U100] JS：DOM 查询
来源：http://hz.nanxinkj.top/gtytttavka.html

document.querySelector(".item")
来源：http://hz.52xcode.cn/gtkstrondo.html

[U101] JS：classList 操作
来源：http://hz.meibo888.top/gtaueywgxf.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtwsulxlcj.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtablydkcj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenlongwang.top/gtkfqdbder.html

[U103] JS：定时器
来源：http://hz.hysaishi.cn/gtnrduobka.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.nanxinkj.top/gtfqkhbsjl.html

[U104] JS：防抖
来源：http://hz.yj20258.top/gtlsmyrzef.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtzhgqsmch.html

[U105] JS：节流
来源：http://hz.nanxinkj.top/gtakpzffvy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daria6918.cn/gtnkbrycro.html

[U106] JS：日期格式化
来源：http://hz.yvedp.cn/gtclanwlxk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jlsjyb.cn/gtmkirrjxo.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gtxmeaubjr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.meibo888.top/gtlokqrubl.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangkeji.top/gtvumcyxfz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yvedp.cn/gttjxmqobj.html

[U109] JS：数组分组
来源：http://hz.yj202588.top/gtdxfmfhey.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtqpussxty.html

[U110] JS：数组分块
来源：http://hz.52xcode.cn/gtzuadisda.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jqgfzy.top/gtcqdaduix.html

[U111] JS：对象转 Map
来源：http://hz.0kj1m.cn/gtpyxjaxcw.html

new Map(Object.entries(obj))
来源：http://hz.jqgfzy.top/gtvjofjrep.html

[U112] JS：字符串补位
来源：http://hz.wangdashe.top/gtmucpzsjt.html

"7".padStart(3, "0")
来源：http://hz.cashguo.top/gtsrkalpop.html

[U113] JS：正则替换全部
来源：http://hz.quarkkingdee.top/gtfowsxjog.html

s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtctrxynyw.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtpvbybdpg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtzkabimly.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtjdpfdorl.html

crypto.randomUUID()
来源：http://hz.cheryme.top/gtloetsiki.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xziqi.cn/gtncoywslw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sysykeji.top/gtgcoudoft.html

[U117] JS：单元测试
来源：http://hz.ydjk.org.cn/gtanjemgde.html

npm i -D vitest;  npx vitest
来源：http://hz.chenzaomai.com/gtgfhomasi.html

[U118] JS：开发服务器
来源：http://hz.andypj.xyz/gtdeulsezj.html

npm i -D vite;  npx vite
来源：http://hz.meibo888.top/gtduanoxsc.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtnrwxrbia.html

npx vite build
来源：http://hz.jinghuilouyu.cn/gtdjjfxewz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.vqdsnc.cn/gtxsmfkapb.html

import.meta.env.VITE_API_URL
来源：http://hz.jyoumei.cn/gteorfrofs.html

================================================================================
来源：http://hz.svipenyu.cn/gtnxstujbq.html

统计汇总
来源：http://hz.jiagoushi.top/gtemhvyxfl.html

================================================================================
来源：http://hz.jqgfzy.top/gtgpkvwyij.html

按语言统计（条）：
来源：http://hz.sweek.top/gtnkjtewvf.html

Python ......... 252
来源：http://hz.hongshengwenyu.top/gtnmikomdu.html

PHP ............ 252
来源：http://hz.pengpengdd.cyou/gtycoktlli.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gtzifqnfdz.html

TypeScript ..... 212
来源：http://hz.yangfankeji.com/gtushupjsq.html

Java ........... 212
来源：http://hz.shanyushiyangtech.top/gtlufbfonu.html

Go ............. 212
来源：http://hz.ivvv.top/gtehmotetv.html

Ruby ........... 212
来源：http://hz.chenlongwang.top/gtiwezxnxg.html

C# ............. 212
来源：http://hz.yuanzhike.top/gtrrclrban.html

C .............. 30
来源：http://hz.svipenyu.cn/gtjythnibs.html

C++ ............ 30
来源：http://hz.9152youxi.cn/gttwkyiudu.html

SQL ............ 90
来源：http://hz.hongshengwenyu.top/gtuaiuszye.html

Bash ........... 80
来源：http://hz.sxryk.cn/gtktluklff.html

Kotlin ......... 15
来源：http://hz.vqdsnc.cn/gtrrdqwtxd.html

Swift .......... 15
来源：http://hz.zhengqikj.top/gtoxlijqjv.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gtsdemaxyu.html

Perl ........... 10
来源：http://hz.chenzaomai.com/gtijgrweln.html

Scala .......... 10
来源：http://hz.jlsjyb.cn/gtlmhswjzu.html

------------------------------------
来源：http://hz.zhoulong.xyz/gthfdgzzbl.html

合计 ........... 2106 条
来源：http://hz.xuanzx.com/gtxeycxcns.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtljfmmdvv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.52xcode.cn/gtuurademo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtdgivbbmm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhoulong.xyz/gtamcviwds.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtakijrnal.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnqzz.top/gtqwklihab.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sxryk.cn/gtzrqailsm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtfyincsxt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.9152youxi.cn/gtskovibrd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gtsesabtgj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gtmqwclucy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtvjnukfni.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtuiwzhifh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtyphmbvql.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtpdqccjls.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.havefunace.top/gtoaoqxbeb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtspbbfxek.html

Q SQL 专题                              90
来源：http://hz.yj20258.top/gtznrelvql.html

R Bash 专题                             80
来源：http://hz.yueranfly.top/gtwypwdbyq.html

S C / C++ 专题                          60
来源：http://hz.zhengqikj.top/gtgtjuoinv.html

T 其他语言补充                          60
来源：http://hz.sweek.top/gttgiavtme.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtikdohjzg.html

------------------------------------
来源：http://hz.kuanghao11.cn/gtdqrgkplu.html

合计                                  2106 条
来源：http://hz.bjfxy.top/gtyhwkyyut.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtwknyernt.html

使用提醒
来源：http://hz.birdmap.top/gtuinxuzff.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtcuhsowcx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jlsjyb.cn/gtrjbwtqod.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnqzz.top/gtfcuapfvu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hysaishi.cn/gtnfeuvrqs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.haohaochexian.top/gtwhporubx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.daxiang520.top/gtzuqadyyo.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtovnnphfg.html

================================================================================
来源：http://hz.jinqigufen.top/gtlvkqhnhr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ivvv.top/gtviypbqoy.html

Common Programming Examples Cheat Book
来源：http://hz.yuanzhike.top/gtimfcdsis.html

================================================================================
来源：http://hz.gogol.net.cn/gtcgstsqmj.html

【收录内容】
来源：http://hz.guannengcc.top/gtdycfjhav.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yuanzhike.top/gtqjreyfsv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fengsongda.top/gtphdbzaus.html

SQL · Bash · C · C++
来源：http://hz.quarkkingdee.top/gtirlkwcdr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.316326.xyz/gtkkuamdzw.html

【使用说明】
来源：http://hz.jinqigfzy.top/gterasnbtw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xylfe.cn/gtwejpczoe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.mhx1999.top/gtrxenzcdo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yanxiufei.cn/gtqltokfdi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangdashe.top/gtecjcjkin.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.redwolf501.top/gtbcsvjzgo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shanyushiyangkeji.top/gtpwpwrjrk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtjlmlpglz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhongyouzk.top/gtixchehmt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gotoacloud.top/gtnmssgkof.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuetiantiany.cn/gtocxzonrv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.fzhhl.top/gtwousnzab.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gtdvijhpwp.html

【文件统计】
来源：http://hz.chenjidiqi.icu/gtvupqdmjs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ehwqpu.com/gtdrvnfnqe.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtgxnuftho.html

目  录
来源：http://hz.chenzaomai.com/gthlkscxpq.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtxtsmrqiz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gteytdcnmw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtutizhacw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gtmgfwvwyf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tian-w.cn/gtzqsvlpzj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.svipenyu.cn/gtmxlkmrjj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jianghu66.top/gtwbbgtcrg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.bjfxy.top/gtcoqxhpvf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.wangshuangyany.cn/gtfpmbusmc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtnsmlbixe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jlsjyb.cn/gtlexgqvvi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtxwttococ.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtnsmcxnko.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gteegactms.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gtvswjwjos.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.svipenyu.cn/gttovhuxay.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtvjbliddz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shuidangran.top/gtjkfhdrdg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.haohaochexian.top/gtvkggunfi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.aizwys.cn/gtegqeglli.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtfjmswouz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtkufmjyfb.html

================================================================================
来源：http://hz.havefunace.top/gtkeptkfex.html

A. 基础语法与类型
来源：http://hz.shanyushiyangtech.top/gteuxkwxop.html

================================================================================
来源：http://hz.quarkkingdee.top/gtraspelik.html

[A01] Hello World
来源：http://hz.pengpengdd.cyou/gtphulgzzj.html

Py:   print("Hello, World!")
来源：http://hz.jiagoushi.top/gtofqcqwrq.html

PHP:  echo "Hello, World!";
来源：http://hz.andypj.xyz/gtpyskhovm.html

JS:   console.log("Hello, World!");
来源：http://hz.zhijiandao.cn/gtikvpvlwj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.nwbrower.top/gtpnbapmyo.html

Java: System.out.println("Hello, World!");
来源：http://hz.zycfv.cn/gtbfgiqjdc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.nanxuanxn.top/gtgrcyuvts.html

Ruby: puts "Hello, World!"
来源：http://hz.gaohongyu789.top/gtiinmoidz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.dashuyun.cn/gthrngvpok.html

[A02] 变量声明与赋值
来源：http://hz.mhx1999.top/gtqiokwuxl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.aibaodan.cn/gtwwuhuyze.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhijiandao.cn/gthjnqetmz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hywenlv.cn/gtwxgjrqxt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shuidangran.top/gtvzwutagp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtkwdllrnx.html

Go:   name := "Alex"; age := 20
来源：http://hz.hysaishi.cn/gtwsjuxnkk.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shzxlz.cn/gtzyewzfmb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gtfdmdhvgu.html

[A03] 常量定义
来源：http://hz.jlsjyb.cn/gtdjkzmehi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yvedp.cn/gtfpxpyzzt.html

PHP:  const PI = 3.14159;
来源：http://hz.yonumen.top/gtjpxqgguz.html

JS:   const PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtceanytnj.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuanzhike.top/gtbzomkjty.html

Java: static final double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtdkwbimgu.html

Go:   const PI = 3.14159
来源：http://hz.guowangkeji.top/gtxwtpskst.html

Ruby: PI = 3.14159
来源：http://hz.feifeiyinyue.top/gtwivfyadq.html

C#:   const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtpowpfxru.html

[A04] 判断变量类型
来源：http://hz.sufxvd.cn/gtzqlnkqmg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxinkj.top/gtxicpeynl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.snrcjt.cn/gtelrblymu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tian-w.cn/gtkwupqodw.html

TS:   typeof x; x instanceof Date
来源：http://hz.kuanghao11.cn/gtnikwpfzn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xinyue.icu/gtagztldlb.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cashguo.top/gtzulixtti.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sysykeji.top/gtcnuawdle.html

C#:   x.GetType().Name; x is int
来源：http://hz.andypj.xyz/gtybkuquuf.html

[A05] 整数除法与取模
来源：http://hz.52xcode.cn/gthihkikln.html


<!-- 参考信息 -->