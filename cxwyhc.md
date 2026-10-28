代发 wailian999

[U31] Py：单测
来源：http://hz.zhongyouzk.top/gtohnyshlq.html

python -m pytest -q
来源：http://hz.yongpay.top/gtfsswcicj.html

[U32] Py：代码格式化
来源：http://hz.zycfv.cn/gttoozmpns.html

ruff format . && ruff check --fix .
来源：http://hz.nwbrower.top/gtubycypru.html

[U33] Py：打包发布
来源：http://hz.smart0.xyz/gtudfuenol.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yvedp.cn/gtocdxbsxv.html

[U34] Py：判断编码
来源：http://hz.svipenyu.cn/gtzvwzquor.html

chardet.detect(raw)
来源：http://hz.jianghu66.top/gtyxdjmiyd.html

[U35] Py：发送邮件
来源：http://hz.mhx1999.top/gtmtlnxald.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.feifeiyinyue.top/gtrgqjzggx.html

[U36] Py：定时任务
来源：http://hz.wangdashe.top/gtynsrijav.html

schedule.every(10).minutes.do(job)
来源：http://hz.feifeiyinyue.top/gtzvitttwr.html

[U37] Py：读写 Excel
来源：http://hz.zhongyouzk.top/gtpvclqjsy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.iojbl.cn/gtwbvswskf.html

[U38] Py：获取脚本所在目录
来源：http://hz.dashuyun.cn/gthstccafv.html

Path(__file__).resolve().parent
来源：http://hz.zhixingplan.top/gtqfgducyx.html

[U39] Py：判断是否在交互环境
来源：http://hz.iojbl.cn/gtgdfnqjal.html

sys.stdout.isatty()
来源：http://hz.tianlin.xyz/gtycjfztwp.html

[U40] Py：打印到标准错误
来源：http://hz.fengsongda.top/gtgvzyonaq.html

print("err", file=sys.stderr)
来源：http://hz.zycfv.cn/gtsjietwbz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhijiandao.cn/gttyettgjt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yvedp.cn/gtcwralcpm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.mhx1999.top/gtpbazxqqi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.svipenyu.cn/gtivarmdji.html

[U43] PHP：声明命名空间
来源：http://hz.chenlongwang.top/gtqigvcccu.html

namespace App\Http;
来源：http://hz.zhijiandao.cn/gtrropqdmf.html

[U44] PHP：开启严格类型
来源：http://hz.guowangkeji.top/gtvjbsutrb.html

declare(strict_types=1);
来源：http://hz.cucudq.cn/gtvyoglidd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.52xcode.cn/gtmqnoszii.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtkxbhneza.html

[U46] PHP：可空类型
来源：http://hz.yj20258888.top/gtciqqgrbq.html

?string $name = null
来源：http://hz.yanxiufei.cn/gtlksvtuqr.html

[U47] PHP：联合类型
来源：http://hz.nanxinkj.top/gtazxvjyil.html

int|string $id
来源：http://hz.iojbl.cn/gtsyeotzur.html

[U48] PHP：纯枚举
来源：http://hz.ydjk.org.cn/gtyrqlamsf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cheryme.top/gtjfyerrag.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gtnbbryaas.html

public readonly string $name
来源：http://hz.zhongyouzk.top/gtqyrfrghj.html

[U50] PHP：构造器属性提升
来源：http://hz.sxryk.cn/gtwxsxlaom.html

public function __construct(private int $id) {}
来源：http://hz.iojbl.cn/gtdfoqkpme.html

[U51] PHP：数组解构
来源：http://hz.aibaodan.cn/gtwnjiqpjy.html

[$a, $b] = $arr;
来源：http://hz.nanxuanxn.top/gtvwdhfutu.html

[U52] PHP：箭头函数
来源：http://hz.jlsjyb.cn/gtqcmthtie.html

$double = fn($x) => $x * 2;
来源：http://hz.smart0.xyz/gtxdjxedez.html

[U53] PHP：空合并运算符
来源：http://hz.ydzc1.top/gtyminzife.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangtech.top/gtvfvicjel.html

[U54] PHP：空安全调用
来源：http://hz.guannengcc.top/gtpqhcopbv.html

$obj?->method()
来源：http://hz.shangyingyoupin.top/gtwttcmucl.html

[U55] PHP：match 表达式
来源：http://hz.yonumen.top/gtnynnfsxy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sweek.top/gtujpaycts.html

[U56] PHP：命名参数
来源：http://hz.smart0.xyz/gtgilszhpn.html

f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtjqxvmvay.html

[U57] PHP：字符串插值
来源：http://hz.yonumen.top/gttaqqptbk.html

"值: {$a}"
来源：http://hz.zhiwuduotai.top/gtlnakaeam.html

[U58] PHP：数组三件套
来源：http://hz.yonumen.top/gtnxaecsgz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jianghu66.top/gthfilyoje.html

[U59] PHP：自定义排序
来源：http://hz.yonumen.top/gtosihmkxt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tian-w.cn/gtrrzvsscw.html

[U60] PHP：JSON 编解码
来源：http://hz.gotoacloud.top/gtxutvctvo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.kuanghao11.cn/gtamalidct.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gtwgemuaiq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gterugbjxy.html

[U62] PHP：日期对象
来源：http://hz.wangshuangyany.cn/gtauyhhlpx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.kuanghao11.cn/gtsvbjsazg.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtcmnlfryw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jlsjyb.cn/gtryeymqsp.html

[U64] PHP：目录遍历
来源：http://hz.ppjwa.cn/gtjcaqbaly.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.andypj.xyz/gtovdwzyou.html

[U65] PHP：会话
来源：http://hz.ppjwa.cn/gtpjkfphwi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xylfe.cn/gtcixivvub.html

[U66] PHP：设置 Cookie
来源：http://hz.xziqi.cn/gtflhfoffr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.kuanghao11.cn/gtncdeshld.html

[U67] PHP：处理文件上传
来源：http://hz.tianlin.xyz/gtkloxykqj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.svipenyu.cn/gthviqirxg.html

[U68] PHP：PDO 连接
来源：http://hz.yangfankeji.com/gtrfjepxty.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tanke756.top/gtsijwatic.html

[U69] PHP：PDO 预处理
来源：http://hz.hnxiangtu.top/gthqblvnqm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jiagoushi.top/gtzjyaazpk.html

[U70] PHP：PDO 事务
来源：http://hz.zhoulong.xyz/gtpfnyevkx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guowangkeji.top/gtwbnbzlqc.html

[U71] PHP：抛出异常
来源：http://hz.jqgfzy.top/gtaxlvxlxq.html

throw new RuntimeException("失败", 500);
来源：http://hz.xylfe.cn/gtwkpxyjsn.html

[U72] PHP：写错误日志
来源：http://hz.jqgufenzy.top/gtqtgseenu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yvedp.cn/gteavkzuxp.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenlongwang.top/gttxpmteds.html

parse_ini_file("config.ini", true)
来源：http://hz.jqgufenzy.top/gtgpwrhdsm.html

[U74] PHP：读取环境变量
来源：http://hz.fzhhl.top/gtifbbijra.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gotoacloud.top/gttsoovnnl.html

[U75] PHP：依赖注入
来源：http://hz.fengsongda.top/gtlitdbyax.html

composer require psr/container
来源：http://hz.yj20258888.top/gtrnsigjzy.html

[U76] PHP：简单路由
来源：http://hz.vqdsnc.cn/gtilvghavn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtgmvgwqtn.html

[U77] PHP：模板渲染
来源：http://hz.cashguo.top/gtjdsrurxi.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gtuccujuhw.html

[U78] PHP：单元测试
来源：http://hz.zhixingplan.top/gtlwnsidkn.html

composer require --dev phpunit/phpunit
来源：http://hz.hnxiangtu.top/gttttpofvb.html

[U79] PHP：静态分析
来源：http://hz.tian-w.cn/gtynxqczes.html

composer require --dev phpstan/phpstan
来源：http://hz.quarkkingdee.top/gtshrqdzst.html

[U80] PHP：代码规范修复
来源：http://hz.quarkkingdee.top/gtemfbrxsq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuanzx.com/gtquqkbmau.html

[U81] JS：初始化项目
来源：http://hz.mhx1999.top/gtwqlelmzg.html

npm init -y;  npm i express
来源：http://hz.9152youxi.cn/gtvrkgvhew.html

[U82] JS：package.json 脚本
来源：http://hz.dianchejie.cn/gtvacamqvr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxinkj.top/gtbwsheaah.html

[U83] JS：ES Module 导入导出
来源：http://hz.smart0.xyz/gtbgbkszyx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shzxlz.cn/gtkzurpkih.html

[U84] JS：CommonJS 写法
来源：http://hz.sysykeji.top/gtjvmmiluq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.havefunace.top/gtuziwnitw.html

[U85] JS：可选链
来源：http://hz.316326.xyz/gtysiirovh.html

a?.b?.c
来源：http://hz.aizwys.cn/gtckswbrwy.html

[U86] JS：空值合并
来源：http://hz.xuetiantiany.cn/gtemtnbekt.html

a ?? b
来源：http://hz.fzhhl.top/gtehcaioxy.html

[U87] JS：解构默认值
来源：http://hz.nanxinkj.top/gtzixnpgqw.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnxiangtu.top/gtliwnkmqp.html

[U88] JS：对象展开合并
来源：http://hz.yvedp.cn/gtrjdruzde.html

{ ...a, ...b }
来源：http://hz.smart0.xyz/gtjxgmbfmb.html

[U89] JS：数组去重
来源：http://hz.meibo888.top/gtyiibdcah.html

[...new Set(arr)]
来源：http://hz.zdqjudy.top/gtlrsbadvu.html

[U90] JS：数字数组排序
来源：http://hz.yvedp.cn/gtsbgqmkcc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtnirgzkug.html

[U91] JS：对象键值遍历
来源：http://hz.jqgfzy.top/gtyplkywcc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.iojbl.cn/gtlgvescsr.html

[U92] JS：深拷贝
来源：http://hz.tian-w.cn/gtyfjxiidf.html

structuredClone(obj)
来源：http://hz.yj20258888.top/gtpmhpjakb.html

[U93] JS：模板字符串
来源：http://hz.pengpengdd.cyou/gteiuglxdl.html

`共 ${n} 条`
来源：http://hz.ppjwa.cn/gtuqfyvkzq.html

[U94] JS：箭头函数
来源：http://hz.cashguo.top/gthtxhllop.html

const double = x => x * 2;
来源：http://hz.cqqwz.cn/gtslyugcbt.html

[U95] JS：Promise 包装
来源：http://hz.smart0.xyz/gtenpirwwf.html

new Promise((resolve, reject) => {})
来源：http://hz.pycfn.com/gttswzthtx.html

[U96] JS：async/await 与异常
来源：http://hz.zhoulong.xyz/gtwlodchxf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtfofjyhvo.html

[U97] JS：并发请求
来源：http://hz.sweek.top/gtnspnhuiv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtqwfwdrpj.html

[U98] JS：fetch 带 JSON
来源：http://hz.sufxvd.cn/gtophtbyan.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.svipenyu.cn/gtivoytrod.html

[U99] JS：事件监听
来源：http://hz.cashguo.top/gtmgztudmc.html

el.addEventListener("click", e => {})
来源：http://hz.jinqigfzy.top/gtpowtimqx.html

[U100] JS：DOM 查询
来源：http://hz.c1oappe.top/gtwnflntxp.html

document.querySelector(".item")
来源：http://hz.jianghu66.top/gtgrhfmubf.html

[U101] JS：classList 操作
来源：http://hz.shanyushiyangtech.top/gtkfxqlrei.html

el.classList.toggle("active")
来源：http://hz.ydzc1.top/gtnvryvoai.html

[U102] JS：本地存储
来源：http://hz.cheryme.top/gtnmdpmbfd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sufxvd.cn/gtskgkhplg.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtyyezahya.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gzhubu.top/gtkbcqnfbq.html

[U104] JS：防抖
来源：http://hz.jinqigfzy.top/gtucvnwatv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtiiocvfxc.html

[U105] JS：节流
来源：http://hz.jinyuanbaomall.cn/gtxfkhjlxu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gttzdlbqwe.html

[U106] JS：日期格式化
来源：http://hz.zhoulong.xyz/gtggheacsn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.smart0.xyz/gtwvwmqhed.html

[U107] JS：数字千分位
来源：http://hz.hysaishi.cn/gtgidxiznu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.havefunace.top/gthscelnle.html

[U108] JS：随机整数
来源：http://hz.sufxvd.cn/gttvsdqljg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gzhubu.top/gtcovcchaf.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtaxxmdapp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gttmdwfsad.html

[U110] JS：数组分块
来源：http://hz.yanxiufei.cn/gtxhxardzl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.pycfn.com/gtfomtkiel.html

[U111] JS：对象转 Map
来源：http://hz.iojbl.cn/gtpetzhaqj.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gtshrkzvny.html

[U112] JS：字符串补位
来源：http://hz.zhengqikj.top/gtrbdwbkaw.html

"7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtwyppybyt.html

[U113] JS：正则替换全部
来源：http://hz.zycfv.cn/gthfwavcfi.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtdokahvyt.html

[U114] JS：JSON 深比较
来源：http://hz.gotoacloud.top/gtoioknswb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtsbfsyeyl.html

[U115] JS：生成 UUID
来源：http://hz.yueranfly.top/gtsbikkcjd.html

crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gttmpsrmik.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gogol.net.cn/gtzrhkjlqu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cqqwz.cn/gtfkdsbkjo.html

[U117] JS：单元测试
来源：http://hz.shangyingyoupin.top/gtbgdjddlb.html

npm i -D vitest;  npx vitest
来源：http://hz.hnxiangtu.top/gtcbytkqnf.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtasrqeqia.html

npm i -D vite;  npx vite
来源：http://hz.quarkkingdee.top/gtwjrlebbk.html

[U119] JS：生产构建
来源：http://hz.jianghu66.top/gtfmfawitx.html

npx vite build
来源：http://hz.ivvv.top/gtbxyiabds.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinghuilouyu.cn/gtbgfxovsp.html

import.meta.env.VITE_API_URL
来源：http://hz.chenjidiqi.icu/gtwkqfceyc.html

================================================================================
来源：http://hz.daria6918.cn/gtqkkvdnax.html

统计汇总
来源：http://hz.9152youxi.cn/gtawvcwfar.html

================================================================================
来源：http://hz.9152youxi.cn/gtquvscywk.html

按语言统计（条）：
来源：http://hz.nanxinkj.top/gtwvzguvbb.html

Python ......... 252
来源：http://hz.svipenyu.cn/gttgpzxxkl.html

PHP ............ 252
来源：http://hz.hammf.cn/gtqrqeqkch.html

JavaScript ..... 252
来源：http://hz.yvedp.cn/gtbgiljozy.html

TypeScript ..... 212
来源：http://hz.cucudq.cn/gtikpaozrz.html

Java ........... 212
来源：http://hz.guowangkeji.top/gthcpkiwft.html

Go ............. 212
来源：http://hz.yangfankeji.com/gtqbrdkdkd.html

Ruby ........... 212
来源：http://hz.zhaomingkeji.xyz/gtihiygbqp.html

C# ............. 212
来源：http://hz.nanxinkj.top/gtugvxcdpo.html

C .............. 30
来源：http://hz.redwolf501.top/gtqnocgoel.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtochfqeug.html

SQL ............ 90
来源：http://hz.quarkkingdee.top/gtrpmamfgy.html

Bash ........... 80
来源：http://hz.zhongyouzk.top/gtvjgypwjq.html

Kotlin ......... 15
来源：http://hz.dashuyun.cn/gtosmelkzd.html

Swift .......... 15
来源：http://hz.hnxiangtu.top/gttwkniark.html

Lua ............ 10
来源：http://hz.chenlongwang.top/gtdcoynaes.html

Perl ........... 10
来源：http://hz.pycfn.com/gtltiztqdw.html

Scala .......... 10
来源：http://hz.dianchejie.cn/gtpbdaubom.html

------------------------------------
来源：http://hz.haohaochexian.top/gtzhrbhzij.html

合计 ........... 2106 条
来源：http://hz.zhoulong.xyz/gtsgdnljsy.html

按章节统计：
来源：http://hz.cdnleiting.top/gtjabkowke.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtamcqrzbq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.guowangkeji.top/gthlxztfud.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtvuxllkok.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtxrwagpen.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hammf.cn/gtzgyjrbie.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgfzy.top/gtnbuoutuo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtzwaljuqh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gtqqqnpcpa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtamtrznea.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhoulong.xyz/gtsiitwxkj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gttstmgjhk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtzejvisjb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtqsjxhlgl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtszfoxmic.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ywan-chungtsiang.top/gtzwmuzufz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtosvhkprn.html

Q SQL 专题                              90
来源：http://hz.yanxiufei.cn/gtnboptxid.html

R Bash 专题                             80
来源：http://hz.fzhhl.top/gteuwfbvns.html

S C / C++ 专题                          60
来源：http://hz.redwolf501.top/gtnvgbgfjc.html

T 其他语言补充                          60
来源：http://hz.fengsongda.top/gtzbhwqtpo.html

U 高频实用片段                         120
来源：http://hz.feifeiyinyue.top/gtxnzqztst.html

------------------------------------
来源：http://hz.cucudq.cn/gtgpjnvzlm.html

合计                                  2106 条
来源：http://hz.yuanzhike.top/gtdyoxoayx.html

--------------------------------------------------------------------------------
来源：http://hz.yvedp.cn/gtfsvgiehn.html

使用提醒
来源：http://hz.zhiwuduotai.top/gtdvktrwbe.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtchjyzzke.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.wangshuangyany.cn/gtmpbsifdc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shzxlz.cn/gtrjsxyedk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hammf.cn/gtasnqfkkw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtnfugoupe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jianghu66.top/gtofqtbszj.html

—— 文件结束 ——
来源：http://hz.yangfankeji.com/gtzhwsefwj.html

================================================================================
来源：http://hz.yonumen.top/gtynradtvk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtzvaqdiku.html

Common Programming Examples Cheat Book
来源：http://hz.cdnleiting.top/gttnnymgth.html

================================================================================
来源：http://hz.ehwqpu.com/gtuzqtfmfw.html

【收录内容】
来源：http://hz.xylfe.cn/gtcpnmdtlw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhijiandao.cn/gtayzhhgsw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shangyingyoupin.top/gtzwdbkhjk.html

SQL · Bash · C · C++
来源：http://hz.jyoumei.cn/gtnlortkuf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj202588.top/gtpwgpvypt.html

【使用说明】
来源：http://hz.havefunace.top/gtzkivsmnx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangkeji.top/gtypxsmhua.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgufenzy.top/gtjdsfxecv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.bjfxy.top/gtndjcsojj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cucudq.cn/gthxbiaosp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xylfe.cn/gtetpocxic.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gtzrczbhxr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yvedp.cn/gtegtxvrgf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.316326.xyz/gtsfpnoarn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yueranfly.top/gtauytdpiz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.wangdashe.top/gtnsesrtxq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.mhx1999.top/gtwcpfzlqg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shanyushiyangkeji.top/gtjrndawpr.html

【文件统计】
来源：http://hz.yj20258.top/gtugsksigt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.316326.xyz/gtnumnyxcm.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtdddstvxy.html

目  录
来源：http://hz.gogol.net.cn/gtfmffekjv.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtrqibzwkm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinyuanbaomall.cn/gttkdaofty.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtemzmkzci.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gtvfbzdvbx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinqigufen.top/gtcdxjqenz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hongshengwenyu.top/gtxumsyroc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xinyue.icu/gtvjavgbal.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtdvsurrxf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnxiangtu.top/gtcbncwgce.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gttfnuppwt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xziqi.cn/gtiybxoqlx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtbenwmgnu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gthvblqlyu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtcrrtdyve.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.meibo888.top/gtlizigeab.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.iojbl.cn/gtrejkznxs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtnceaekbc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cheryme.top/gtqzsmeqkf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fengsongda.top/gtqczpgmdt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cucudq.cn/gtjeqrwsws.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtsizuxfhh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtlsjaxqin.html

================================================================================
来源：http://hz.cheryme.top/gtblhweoxr.html

A. 基础语法与类型
来源：http://hz.aizwys.cn/gtoevjhedp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtgvsqacct.html

[A01] Hello World
来源：http://hz.sxryk.cn/gtlnzfxzza.html

Py:   print("Hello, World!")
来源：http://hz.jinqigufen.top/gtmfzlpbmr.html

PHP:  echo "Hello, World!";
来源：http://hz.sweek.top/gtgovymcex.html

JS:   console.log("Hello, World!");
来源：http://hz.yonumen.top/gtbfuglkvm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhengqikj.top/gtbnmktcpb.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhoulong.xyz/gtatodqlds.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.meibo888.top/gtkvokgnbu.html

Ruby: puts "Hello, World!"
来源：http://hz.shzxlz.cn/gtbuamgrec.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cdnleiting.top/gtnooswekr.html

[A02] 变量声明与赋值
来源：http://hz.shuidangran.top/gtfbckibmc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.chenzaomai.com/gtqzwsnttw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.chenlongwang.top/gtkwlsztei.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zycfv.cn/gtkzsqjhyn.html


<!-- 参考信息 -->