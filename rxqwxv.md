代发 wailian999

[U25] Py：CSV 按字典读
来源：http://hz.hysaishi.cn/gtpfwhooar.html

csv.DictReader(f)
来源：http://hz.xuetiantiany.cn/gtuuxivgeu.html

[U26] Py：并发下载
来源：http://hz.chenlongwang.top/gtjvrgspol.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtswkzltbj.html

[U27] Py：异步 HTTP
来源：http://hz.kuanghao11.cn/gtcaydtjkw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zdqjudy.top/gtpdkasknn.html

[U28] Py：类型别名
来源：http://hz.jiagoushi.top/gthtjvarrk.html

UserId = int
来源：http://hz.snrcjt.cn/gtuteesdza.html

[U29] Py：属性校验
来源：http://hz.dianchejie.cn/gtwswvwcrd.html

@property 与 @x.setter 配合
来源：http://hz.zhijiandao.cn/gtrrmrvmof.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtmyrnisor.html

@dataclass(slots=True)
来源：http://hz.iojbl.cn/gtrjbkevhf.html

[U31] Py：单测
来源：http://hz.zycfv.cn/gtcrmnvcqh.html

python -m pytest -q
来源：http://hz.jiagoushi.top/gtaytyfilm.html

[U32] Py：代码格式化
来源：http://hz.quarkkingdee.top/gtwryittgf.html

ruff format . && ruff check --fix .
来源：http://hz.smart0.xyz/gtaexweobe.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtidqjmhdb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tanke756.top/gtsjpetmti.html

[U34] Py：判断编码
来源：http://hz.shuidangran.top/gtyqueonvs.html

chardet.detect(raw)
来源：http://hz.quarkkingdee.top/gtfzmcbjwp.html

[U35] Py：发送邮件
来源：http://hz.shzxlz.cn/gtucttuklz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgfzy.top/gtrkicvnjb.html

[U36] Py：定时任务
来源：http://hz.yj20258.top/gtuarjbydo.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj202588.top/gtoilviszz.html

[U37] Py：读写 Excel
来源：http://hz.daria6918.cn/gtfzjbilrb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtnlmrfxgd.html

[U38] Py：获取脚本所在目录
来源：http://hz.guannengcc.top/gtvojhtesu.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtavhlwfic.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gttqnigxrb.html

sys.stdout.isatty()
来源：http://hz.bjfxy.top/gtjeaqmspn.html

[U40] Py：打印到标准错误
来源：http://hz.ywan-chungtsiang.top/gtbmmckavh.html

print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtkwqlumsi.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xuetiantiany.cn/gtjfzauwpt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xingfuxueyuan.xyz/gtfzekoxhw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.smart0.xyz/gtluhaxneb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tianlin.xyz/gtjdvxjvxz.html

[U43] PHP：声明命名空间
来源：http://hz.dashuyun.cn/gtvlzowypv.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtjgypqahu.html

[U44] PHP：开启严格类型
来源：http://hz.sysykeji.top/gthwixdtip.html

declare(strict_types=1);
来源：http://hz.nanxinkj.top/gtcgdfjyfr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sufxvd.cn/gtdvowxmuw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gttjkbhvpx.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtxkglygnq.html

?string $name = null
来源：http://hz.cashguo.top/gtbequlvgh.html

[U47] PHP：联合类型
来源：http://hz.jinqigfzy.top/gtmgddueuc.html

int|string $id
来源：http://hz.nanxinkj.top/gtfeosxqgp.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtsnmhvvsf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ybcxt.top/gtkacrasau.html

[U49] PHP：只读属性
来源：http://hz.yuxming.cn/gtgynszbxc.html

public readonly string $name
来源：http://hz.kuanghao11.cn/gtyqriocpc.html

[U50] PHP：构造器属性提升
来源：http://hz.yuxming.cn/gtcezyghsh.html

public function __construct(private int $id) {}
来源：http://hz.zdqjudy.top/gtjpzezpcd.html

[U51] PHP：数组解构
来源：http://hz.hnqzz.top/gtavchjpvh.html

[$a, $b] = $arr;
来源：http://hz.iojbl.cn/gtbhifuhlq.html

[U52] PHP：箭头函数
来源：http://hz.feifeiyinyue.top/gtbafkfzjo.html

$double = fn($x) => $x * 2;
来源：http://hz.snrcjt.cn/gtkjglnsdo.html

[U53] PHP：空合并运算符
来源：http://hz.vqdsnc.cn/gtmwvhoxfc.html

$v = $a ?? $b ?? "default";
来源：http://hz.xinyue.icu/gtyjulxibp.html

[U54] PHP：空安全调用
来源：http://hz.daxiang520.top/gtjsbsdtgw.html

$obj?->method()
来源：http://hz.yj20258888.top/gtzroiqpaj.html

[U55] PHP：match 表达式
来源：http://hz.tianlin.xyz/gtvogntmfs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.pycfn.com/gtedothfyf.html

[U56] PHP：命名参数
来源：http://hz.birdmap.top/gtldqaeztr.html

f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtboqyfobs.html

[U57] PHP：字符串插值
来源：http://hz.chenjidiqi.icu/gtvptamkxg.html

"值: {$a}"
来源：http://hz.52xcode.cn/gtashrxbws.html

[U58] PHP：数组三件套
来源：http://hz.nwbrower.top/gtjoljdsye.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gaohongyu789.top/gtfsxhymdr.html

[U59] PHP：自定义排序
来源：http://hz.fengsongda.top/gtdbcjcnch.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtarmphlow.html

[U60] PHP：JSON 编解码
来源：http://hz.sxryk.cn/gtgrblvyej.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tianlin.xyz/gtaaksrdyc.html

[U61] PHP：正则
来源：http://hz.shzxlz.cn/gtfogcbvmc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtatwyhlph.html

[U62] PHP：日期对象
来源：http://hz.zhixingplan.top/gtiljivbzo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ydjk.org.cn/gteqcgrtrd.html

[U63] PHP：文件读写
来源：http://hz.ybcxt.top/gtvcikvhnt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuetiantiany.cn/gtrkrldxkl.html

[U64] PHP：目录遍历
来源：http://hz.redwolf501.top/gtradmtzjm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yueranfly.top/gtqveygyts.html

[U65] PHP：会话
来源：http://hz.yueranfly.top/gtuawomkjk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtbiqscthp.html

[U66] PHP：设置 Cookie
来源：http://hz.zhiwuduotai.top/gtadjjqssl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.c1oappe.top/gtjwuzjbbc.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigfzy.top/gthxwqadlf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.dashuyun.cn/gtcspfsaqu.html

[U68] PHP：PDO 连接
来源：http://hz.jianghu66.top/gtrkigdyqy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ppjwa.cn/gtwhkpuwqd.html

[U69] PHP：PDO 预处理
来源：http://hz.yanxiufei.cn/gtpuqdptcc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.daria6918.cn/gtugyrdahc.html

[U70] PHP：PDO 事务
来源：http://hz.ivvv.top/gtamxxwlol.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yuanzhike.top/gtiybypruk.html

[U71] PHP：抛出异常
来源：http://hz.daxiang520.top/gttrqqkcwb.html

throw new RuntimeException("失败", 500);
来源：http://hz.daxiang520.top/gtirrqpmzk.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gtdtqgmvwy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.316326.xyz/gttkvqvqvp.html

[U73] PHP：读取 ini 配置
来源：http://hz.hywenlv.cn/gtfisxtrmg.html

parse_ini_file("config.ini", true)
来源：http://hz.yuanzhike.top/gtuzmdpxov.html

[U74] PHP：读取环境变量
来源：http://hz.zhixingplan.top/gtddadmmys.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jyoumei.cn/gtphkuttoc.html

[U75] PHP：依赖注入
来源：http://hz.dianchejie.cn/gtzzlhmojj.html

composer require psr/container
来源：http://hz.quarkkingdee.top/gteipiclcl.html

[U76] PHP：简单路由
来源：http://hz.jinghuilouyu.cn/gtzdffrfzd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangkeji.top/gtzpgodqlq.html

[U77] PHP：模板渲染
来源：http://hz.yueranfly.top/gtatjtvomq.html

composer require twig/twig
来源：http://hz.pycfn.com/gtenljxshf.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtfufdlgqj.html

composer require --dev phpunit/phpunit
来源：http://hz.hfpthk.cn/gtvkgcbixe.html

[U79] PHP：静态分析
来源：http://hz.dianchejie.cn/gtnkceerwr.html

composer require --dev phpstan/phpstan
来源：http://hz.haohaochexian.top/gteyyehxzz.html

[U80] PHP：代码规范修复
来源：http://hz.xuetiantiany.cn/gtwrlrbtca.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yanxiufei.cn/gtknokqxxt.html

[U81] JS：初始化项目
来源：http://hz.zhaomingkeji.xyz/gtgkxelvmf.html

npm init -y;  npm i express
来源：http://hz.shuidangran.top/gtzkrzvbrf.html

[U82] JS：package.json 脚本
来源：http://hz.cdnleiting.top/gtetmfodhu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ywan-chungtsiang.top/gtlkrszfnx.html

[U83] JS：ES Module 导入导出
来源：http://hz.jianghu66.top/gtdtrhjeuq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhongyouzk.top/gtrbgppjmb.html

[U84] JS：CommonJS 写法
来源：http://hz.yj20258888.top/gtuadgynnj.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydzc1.top/gthfuhobvu.html

[U85] JS：可选链
来源：http://hz.pengpengdd.cyou/gtdkvitpfh.html

a?.b?.c
来源：http://hz.sweek.top/gtygdknuhk.html

[U86] JS：空值合并
来源：http://hz.cdnleiting.top/gturveabjv.html

a ?? b
来源：http://hz.cashguo.top/gtfvdxiovc.html

[U87] JS：解构默认值
来源：http://hz.shanyushiyangtech.top/gtznljraxi.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuxming.cn/gtwdxvphsf.html

[U88] JS：对象展开合并
来源：http://hz.hongshengwenyu.top/gtfsljspqp.html

{ ...a, ...b }
来源：http://hz.tianlin.xyz/gtzpctswlj.html

[U89] JS：数组去重
来源：http://hz.tanke756.top/gtqxxixthj.html

[...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtyajdcpbn.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtvygemsyj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtcoufxmki.html

[U91] JS：对象键值遍历
来源：http://hz.gzhubu.top/gtwabqlsaw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gaohongyu789.top/gtfpzaqswl.html

[U92] JS：深拷贝
来源：http://hz.dashuyun.cn/gteuyvgyte.html

structuredClone(obj)
来源：http://hz.chenzaomai.com/gtugoysrgb.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtnxmowaby.html

`共 ${n} 条`
来源：http://hz.jinghuilouyu.cn/gtkuoaiakg.html

[U94] JS：箭头函数
来源：http://hz.havefunace.top/gtdrvexpuh.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtlizefxfp.html

[U95] JS：Promise 包装
来源：http://hz.haohaochexian.top/gtlpxlaqql.html

new Promise((resolve, reject) => {})
来源：http://hz.jinghuilouyu.cn/gtyyhsxetg.html

[U96] JS：async/await 与异常
来源：http://hz.zhijiandao.cn/gtlqeinqvj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtwldxoonr.html

[U97] JS：并发请求
来源：http://hz.snrcjt.cn/gtxeqxqruk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtzmsccixr.html

[U98] JS：fetch 带 JSON
来源：http://hz.yonumen.top/gtyqonrgxi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuanzx.com/gtoxwilteb.html

[U99] JS：事件监听
来源：http://hz.cdnleiting.top/gteobhyotb.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtipcylfzv.html

[U100] JS：DOM 查询
来源：http://hz.ybcxt.top/gtlbpupefx.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtcsfrgltg.html

[U101] JS：classList 操作
来源：http://hz.xuetiantiany.cn/gtmodwozjk.html

el.classList.toggle("active")
来源：http://hz.wangshuangyany.cn/gtwqrxbrxk.html

[U102] JS：本地存储
来源：http://hz.mhx1999.top/gttzbjsmgc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hysaishi.cn/gtsxvqqsta.html

[U103] JS：定时器
来源：http://hz.xuetiantiany.cn/gtvsgvryyg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.nanxinkj.top/gtxzcbppnt.html

[U104] JS：防抖
来源：http://hz.aizwys.cn/gtkraafkog.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtawqhnhso.html

[U105] JS：节流
来源：http://hz.mhx1999.top/gtkzqtujys.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.mhx1999.top/gtgbtmtbex.html

[U106] JS：日期格式化
来源：http://hz.kuanghao11.cn/gtlmonzakv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangtech.top/gtrxfxjfhj.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gtcczirjos.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydzc1.top/gtrgvnvtau.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtadsfbrls.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.quarkkingdee.top/gtmtbblxnc.html

[U109] JS：数组分组
来源：http://hz.jqgufenzy.top/gtfuuhjlgi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.aibaodan.cn/gtpubktppa.html

[U110] JS：数组分块
来源：http://hz.dianchejie.cn/gtxmrvheyk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sweek.top/gtdaxnsugu.html

[U111] JS：对象转 Map
来源：http://hz.shangyingyoupin.top/gtxltgxsyx.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtqbaqbwbp.html

[U112] JS：字符串补位
来源：http://hz.shzxlz.cn/gtbzhvbiju.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtfcufpxvx.html

[U113] JS：正则替换全部
来源：http://hz.cheryme.top/gtjibjpnuq.html

s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtszlsplcp.html

[U114] JS：JSON 深比较
来源：http://hz.zycfv.cn/gtnbojhbdy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gturlzcogc.html

[U115] JS：生成 UUID
来源：http://hz.dianchejie.cn/gteqdjybfj.html

crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtikplpydw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jiagoushi.top/gtoefbajct.html

/** @param {string} name */ function f(name) {}
来源：http://hz.haohaochexian.top/gtiyghkoqw.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtgiuizddr.html

npm i -D vitest;  npx vitest
来源：http://hz.xuanzx.com/gtnpnoegbg.html

[U118] JS：开发服务器
来源：http://hz.wangdashe.top/gtazivaakz.html

npm i -D vite;  npx vite
来源：http://hz.daria6918.cn/gtdfzzwiiy.html

[U119] JS：生产构建
来源：http://hz.ywan-chungtsiang.top/gtwmqnzaoi.html

npx vite build
来源：http://hz.hnxiangtu.top/gtimnrkdgi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sysykeji.top/gthrovrjox.html

import.meta.env.VITE_API_URL
来源：http://hz.andypj.xyz/gttdimnfzu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtoecjtluz.html

统计汇总
来源：http://hz.zhoulong.xyz/gtzbzqozhx.html

================================================================================
来源：http://hz.zdqjudy.top/gtmxzxoikc.html

按语言统计（条）：
来源：http://hz.nanxinkj.top/gtvouxbedh.html

Python ......... 252
来源：http://hz.hnxiangtu.top/gtrfcuyrze.html

PHP ............ 252
来源：http://hz.xinyue.icu/gtuwizwkkf.html

JavaScript ..... 252
来源：http://hz.pengpengdd.cyou/gtyepxjnum.html

TypeScript ..... 212
来源：http://hz.xuetiantiany.cn/gtqheottjz.html

Java ........... 212
来源：http://hz.shangyingyoupin.top/gtmxufldku.html

Go ............. 212
来源：http://hz.nanxinkj.top/gtgybdicxh.html

Ruby ........... 212
来源：http://hz.gaohongyu789.top/gtsyajnnwq.html

C# ............. 212
来源：http://hz.ppjwa.cn/gtlxiigfpw.html

C .............. 30
来源：http://hz.hysaishi.cn/gtnqzomuxo.html

C++ ............ 30
来源：http://hz.zhengqikj.top/gtgsktohpb.html

SQL ............ 90
来源：http://hz.nanxinkj.top/gtrmbsrity.html

Bash ........... 80
来源：http://hz.nanxuanxn.top/gtiboqzaqz.html

Kotlin ......... 15
来源：http://hz.gogol.net.cn/gtbbaxpmby.html

Swift .......... 15
来源：http://hz.zhiwuduotai.top/gtnyiwrelp.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtmzniddno.html

Perl ........... 10
来源：http://hz.mhx1999.top/gtnrhnlmpu.html

Scala .......... 10
来源：http://hz.guowangkeji.top/gtygpnxbhd.html

------------------------------------
来源：http://hz.quarkkingdee.top/gthflqthkc.html

合计 ........... 2106 条
来源：http://hz.cqqwz.cn/gtmlooxsmp.html

按章节统计：
来源：http://hz.yj20258888.top/gtsjqlxfwr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gtnrkhleyy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtdybghycg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtnfuuquhx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gaohongyu789.top/gtijhjyfii.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenlongwang.top/gtenxclmnl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hfpthk.cn/gtltxptfvx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtldgqbgyg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.daxiang520.top/gtfortufhn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtfsuxzriw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinghuilouyu.cn/gtlhrmjkkc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtyxkyidqr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtybityrtv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtuhrnlfwb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.redwolf501.top/gtvcwqulcn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.aibaodan.cn/gtqkijltjv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtqcksmboi.html

Q SQL 专题                              90
来源：http://hz.iojbl.cn/gtguazuymz.html

R Bash 专题                             80
来源：http://hz.dashuyun.cn/gtxevtmwha.html

S C / C++ 专题                          60
来源：http://hz.jinqigfzy.top/gtaseekqee.html

T 其他语言补充                          60
来源：http://hz.nanxinkj.top/gtmhtvhwnu.html

U 高频实用片段                         120
来源：http://hz.52xcode.cn/gttkekaeaj.html

------------------------------------
来源：http://hz.daria6918.cn/gtrgbrzvnl.html

合计                                  2106 条
来源：http://hz.zhengqikj.top/gtpnhgrpov.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtuuklqajm.html

使用提醒
来源：http://hz.iojbl.cn/gtimgxdlvp.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtiovmulkl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cheryme.top/gtffeawquc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yueranfly.top/gtgzkzghna.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cqqwz.cn/gtyqhvzqic.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xuetiantiany.cn/gtyfxrvaxl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jianghu66.top/gtikvqlngr.html

—— 文件结束 ——
来源：http://hz.zdqjudy.top/gtbandlrmu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlgiaggfg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nanxuanxn.top/gtoovcjohw.html

Common Programming Examples Cheat Book
来源：http://hz.yuxming.cn/gtllgsrprn.html

================================================================================
来源：http://hz.haohaochexian.top/gtztvkakch.html

【收录内容】
来源：http://hz.birdmap.top/gtjatteisp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.9152youxi.cn/gtmgedxluz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nanxinkj.top/gtplrdabmi.html

SQL · Bash · C · C++
来源：http://hz.aibaodan.cn/gtmnbhvgfh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hysaishi.cn/gtceijpqrf.html

【使用说明】
来源：http://hz.aizwys.cn/gtocnhkvkf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shuidangran.top/gtqvcwmlpu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xingfuxueyuan.xyz/gtflbttgzs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258888.top/gtyaoydcsl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hammf.cn/gtljtswoyu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.pengpengdd.cyou/gtqkjhfxhn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nanxinkj.top/gtwrvimzwx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jyoumei.cn/gtfolqvaif.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.quarkkingdee.top/gtbyaueabh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gzhubu.top/gtmxjwtett.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ehwqpu.com/gtexsjyznw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.aibaodan.cn/gthlpmybmm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.havefunace.top/gtcvtslwtb.html

【文件统计】
来源：http://hz.pengpengdd.cyou/gtnmwmzzct.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sysykeji.top/gtawkrnzdx.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtyrkigfxb.html

目  录
来源：http://hz.dianchejie.cn/gticqewaay.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtfyrdlyau.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenzaomai.com/gtcqbyrmox.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtxrdtsxzb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xuetiantiany.cn/gtdodkzkfz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtyrfnvqzb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.daria6918.cn/gtwbhzmzpg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jianghu66.top/gtxneeelsm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtasbluzcb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gtptqepjhw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtbqgoxexv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jlsjyb.cn/gtzwmxcule.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtjpwihwbh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtcfsecucf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtntuqqhnf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.nanxuanxn.top/gtotoncnym.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinqigufen.top/gtvgsxhfhg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtqowvijgv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.bjfxy.top/gtqyghzrlb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ppjwa.cn/gtqujqtvwu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.9152youxi.cn/gtfmkoxrap.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtitlizpvu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ehwqpu.com/gtojfuunws.html

================================================================================
来源：http://hz.aizwys.cn/gtfvtwwcpo.html

A. 基础语法与类型
来源：http://hz.cucudq.cn/gtqfprafaw.html

================================================================================
来源：http://hz.yvedp.cn/gtkacyrzxt.html

[A01] Hello World
来源：http://hz.pycfn.com/gtrvvouvrf.html


<!-- 参考信息 -->