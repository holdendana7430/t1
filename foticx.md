代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://hz.ivvv.top/gtlttnrfdw.html

@contextlib.contextmanager
来源：http://hz.iojbl.cn/gtwsykcsyi.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtmsyghspr.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtcgbwgmod.html

[U23] Py：分块读取大文件
来源：http://hz.zycfv.cn/gtziuedbof.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.iojbl.cn/gtepolsyjj.html

[U24] Py：路径操作
来源：http://hz.jlsjyb.cn/gtusavnsnd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtjdnvssfl.html

[U25] Py：CSV 按字典读
来源：http://hz.ywan-chungtsiang.top/gtbxxgqmxd.html

csv.DictReader(f)
来源：http://hz.vqdsnc.cn/gtcvrhlrah.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtssnievex.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.c1oappe.top/gtdgcsppld.html

[U27] Py：异步 HTTP
来源：http://hz.hongshengwenyu.top/gtuuyjqvnk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cheryme.top/gttazzyiwa.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtgmnvhtrr.html

UserId = int
来源：http://hz.svipenyu.cn/gtoaivrjfp.html

[U29] Py：属性校验
来源：http://hz.nanxinkj.top/gtsuhcxrbl.html

@property 与 @x.setter 配合
来源：http://hz.wangdashe.top/gtanvyxijo.html

[U30] Py：数据类
来源：http://hz.c1oappe.top/gtjsqxazua.html

@dataclass(slots=True)
来源：http://hz.zhoulong.xyz/gtwmvsyfym.html

[U31] Py：单测
来源：http://hz.feifeiyinyue.top/gtqkdlmehb.html

python -m pytest -q
来源：http://hz.zycfv.cn/gtipetxxsu.html

[U32] Py：代码格式化
来源：http://hz.nanxuanxn.top/gtowdgjoqd.html

ruff format . && ruff check --fix .
来源：http://hz.yonumen.top/gtoysyoqgo.html

[U33] Py：打包发布
来源：http://hz.ehwqpu.com/gtfowfsrve.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.guowangkeji.top/gtzfudlqrx.html

[U34] Py：判断编码
来源：http://hz.havefunace.top/gtilvtiqfy.html

chardet.detect(raw)
来源：http://hz.yj20258888.top/gtesaqvuom.html

[U35] Py：发送邮件
来源：http://hz.haohaochexian.top/gtmrzbpeks.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinqigufen.top/gtwpvwbgqp.html

[U36] Py：定时任务
来源：http://hz.bjfxy.top/gtkezqzuiq.html

schedule.every(10).minutes.do(job)
来源：http://hz.yueranfly.top/gtbdmyzpjc.html

[U37] Py：读写 Excel
来源：http://hz.jqgfzy.top/gtwzxwxmek.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigfzy.top/gtncbxsiaa.html

[U38] Py：获取脚本所在目录
来源：http://hz.hywenlv.cn/gtmnepxtwj.html

Path(__file__).resolve().parent
来源：http://hz.zhongyouzk.top/gtrvgmpmpf.html

[U39] Py：判断是否在交互环境
来源：http://hz.ybcxt.top/gtxfpbhplv.html

sys.stdout.isatty()
来源：http://hz.jinqigfzy.top/gtgzstautg.html

[U40] Py：打印到标准错误
来源：http://hz.pengpengdd.cyou/gtuinyfzsd.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtytqgmbeg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.9152youxi.cn/gtysjyuiea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhiwuduotai.top/gtkzdxsaki.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.9152youxi.cn/gtyjplkgzv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj202588.top/gtviysdpkv.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gthkoixlve.html

namespace App\Http;
来源：http://hz.yangfankeji.com/gtijxddhoy.html

[U44] PHP：开启严格类型
来源：http://hz.sysykeji.top/gtvvdmlrmz.html

declare(strict_types=1);
来源：http://hz.chenlongwang.top/gtviogtior.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zdqjudy.top/gtdbtrdykh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtwovkxtfy.html

[U46] PHP：可空类型
来源：http://hz.sysykeji.top/gtqxxhucjy.html

?string $name = null
来源：http://hz.gaohongyu789.top/gtiwbtnypo.html

[U47] PHP：联合类型
来源：http://hz.guowangkeji.top/gtfambuacz.html

int|string $id
来源：http://hz.cucudq.cn/gtpfyablas.html

[U48] PHP：纯枚举
来源：http://hz.iojbl.cn/gteekxslka.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cashguo.top/gtnwjsntlj.html

[U49] PHP：只读属性
来源：http://hz.yuanzhike.top/gtmzlawoih.html

public readonly string $name
来源：http://hz.chenzaomai.com/gtztntghpz.html

[U50] PHP：构造器属性提升
来源：http://hz.dianchejie.cn/gtbkmhbbnx.html

public function __construct(private int $id) {}
来源：http://hz.xylfe.cn/gtcnzwzlub.html

[U51] PHP：数组解构
来源：http://hz.mhx1999.top/gtowdytfnx.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtdlkxvafd.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtbvafzsjr.html

$double = fn($x) => $x * 2;
来源：http://hz.vqdsnc.cn/gtffemapdu.html

[U53] PHP：空合并运算符
来源：http://hz.tanke756.top/gtlvhilbpg.html

$v = $a ?? $b ?? "default";
来源：http://hz.bjfxy.top/gtypyiirpt.html

[U54] PHP：空安全调用
来源：http://hz.fengsongda.top/gtcszuviqq.html

$obj?->method()
来源：http://hz.yongpay.top/gtjcfldnde.html

[U55] PHP：match 表达式
来源：http://hz.sweek.top/gtrjzlikcs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jianghu66.top/gtctlaessh.html

[U56] PHP：命名参数
来源：http://hz.kuanghao11.cn/gtxgfwdrdu.html

f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtxlrgegyj.html

[U57] PHP：字符串插值
来源：http://hz.cqqwz.cn/gtymtsacsy.html

"值: {$a}"
来源：http://hz.dashuyun.cn/gtsngodhxf.html

[U58] PHP：数组三件套
来源：http://hz.yj20258888.top/gtannftfnc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hongshengwenyu.top/gtjycteqxf.html

[U59] PHP：自定义排序
来源：http://hz.vqdsnc.cn/gtewlaqzso.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhijiandao.cn/gtrflryddx.html

[U60] PHP：JSON 编解码
来源：http://hz.yongpay.top/gtiobktakj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.daxiang520.top/gtpqbygrrf.html

[U61] PHP：正则
来源：http://hz.hywenlv.cn/gtpxxprnse.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtzqfpsole.html

[U62] PHP：日期对象
来源：http://hz.52xcode.cn/gtjonrgwla.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj20258888.top/gtctsvkghj.html

[U63] PHP：文件读写
来源：http://hz.ydzc1.top/gtxgkfufze.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenjidiqi.icu/gtrdjtpttc.html

[U64] PHP：目录遍历
来源：http://hz.chenlongwang.top/gtamisfllr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangdashe.top/gtvcjyaeqq.html

[U65] PHP：会话
来源：http://hz.sufxvd.cn/gtfmpazjfp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ppjwa.cn/gtmnvbymku.html

[U66] PHP：设置 Cookie
来源：http://hz.ehwqpu.com/gtjiilradb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.kuanghao11.cn/gtenumsgef.html

[U67] PHP：处理文件上传
来源：http://hz.cheryme.top/gtmezbmdxm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ehwqpu.com/gtbfakqsqa.html

[U68] PHP：PDO 连接
来源：http://hz.gogol.net.cn/gtvcprfylm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ydzc1.top/gtyzlqpyev.html

[U69] PHP：PDO 预处理
来源：http://hz.zdqjudy.top/gtxmubzdxf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ydzc1.top/gtqhqmpwqy.html

[U70] PHP：PDO 事务
来源：http://hz.ppjwa.cn/gtrdsuvpvk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.aibaodan.cn/gtjncuszrz.html

[U71] PHP：抛出异常
来源：http://hz.yueranfly.top/gtigifumjr.html

throw new RuntimeException("失败", 500);
来源：http://hz.guannengcc.top/gtvnbmudez.html

[U72] PHP：写错误日志
来源：http://hz.jiagoushi.top/gthqdrlpcf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yuanzhike.top/gtcbrlzska.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhijiandao.cn/gtikryfdss.html

parse_ini_file("config.ini", true)
来源：http://hz.hnxiangtu.top/gtemhrxvqo.html

[U74] PHP：读取环境变量
来源：http://hz.jyoumei.cn/gtcmqwxhhu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.svipenyu.cn/gthrlicvwk.html

[U75] PHP：依赖注入
来源：http://hz.hysaishi.cn/gttmencssc.html

composer require psr/container
来源：http://hz.feifeiyinyue.top/gtfyzdniho.html

[U76] PHP：简单路由
来源：http://hz.hongshengwenyu.top/gtjvtbvohf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yuxming.cn/gtoynjggqh.html

[U77] PHP：模板渲染
来源：http://hz.shanyushiyangkeji.top/gturjnmqce.html

composer require twig/twig
来源：http://hz.xuanzx.com/gtdktqgxus.html

[U78] PHP：单元测试
来源：http://hz.haohaochexian.top/gtxswksylc.html

composer require --dev phpunit/phpunit
来源：http://hz.gaohongyu789.top/gtgeabkmka.html

[U79] PHP：静态分析
来源：http://hz.birdmap.top/gtnjlaperv.html

composer require --dev phpstan/phpstan
来源：http://hz.zycfv.cn/gtzzdguyfr.html

[U80] PHP：代码规范修复
来源：http://hz.pycfn.com/gtfcvbwaxs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yueranfly.top/gtbvdhhyta.html

[U81] JS：初始化项目
来源：http://hz.aizwys.cn/gtlbwxrudh.html

npm init -y;  npm i express
来源：http://hz.zdqjudy.top/gtfhrqjneu.html

[U82] JS：package.json 脚本
来源：http://hz.fengsongda.top/gtlsftwuow.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shzxlz.cn/gtqgkjnnei.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhoulong.xyz/gtvjodnlic.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtslliftcp.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gtxxpdksrh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nwbrower.top/gtpggztqvp.html

[U85] JS：可选链
来源：http://hz.jiagoushi.top/gttimfccaf.html

a?.b?.c
来源：http://hz.daxiang520.top/gtohoubpmx.html

[U86] JS：空值合并
来源：http://hz.snrcjt.cn/gtzagjdrbh.html

a ?? b
来源：http://hz.zhongyouzk.top/gtfdzgoxqy.html

[U87] JS：解构默认值
来源：http://hz.guannengcc.top/gtswfdfxle.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gaohongyu789.top/gthesrdyfs.html

[U88] JS：对象展开合并
来源：http://hz.xuetiantiany.cn/gtjqmoehqt.html

{ ...a, ...b }
来源：http://hz.kuanghao11.cn/gtdfvtxewr.html

[U89] JS：数组去重
来源：http://hz.zhijiandao.cn/gtxyteawau.html

[...new Set(arr)]
来源：http://hz.yj202588.top/gtidrlxznd.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtxbykbylq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtidrslooo.html

[U91] JS：对象键值遍历
来源：http://hz.guannengcc.top/gtffrkizqs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yanxiufei.cn/gtdgdnpjpu.html

[U92] JS：深拷贝
来源：http://hz.jqgufenzy.top/gtumzzfpot.html

structuredClone(obj)
来源：http://hz.cashguo.top/gtzynjuzwh.html

[U93] JS：模板字符串
来源：http://hz.sysykeji.top/gtceviqnvh.html

`共 ${n} 条`
来源：http://hz.9152youxi.cn/gteytcteul.html

[U94] JS：箭头函数
来源：http://hz.yvedp.cn/gtxolzlevc.html

const double = x => x * 2;
来源：http://hz.52xcode.cn/gtsejybnqx.html

[U95] JS：Promise 包装
来源：http://hz.tanke756.top/gtuftiawjs.html

new Promise((resolve, reject) => {})
来源：http://hz.nwbrower.top/gtofoaqwpt.html

[U96] JS：async/await 与异常
来源：http://hz.yanxiufei.cn/gtynnghjvh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtkslxmygq.html

[U97] JS：并发请求
来源：http://hz.haohaochexian.top/gtafrkocta.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtlggkmras.html

[U98] JS：fetch 带 JSON
来源：http://hz.nanxuanxn.top/gtcrgecfvc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zdqjudy.top/gtujlyqvys.html

[U99] JS：事件监听
来源：http://hz.xylfe.cn/gtzzkeyrkn.html

el.addEventListener("click", e => {})
来源：http://hz.jqgufenzy.top/gtmjniphda.html

[U100] JS：DOM 查询
来源：http://hz.wangshuangyany.cn/gtqlugnxjc.html

document.querySelector(".item")
来源：http://hz.andypj.xyz/gtjnvucvez.html

[U101] JS：classList 操作
来源：http://hz.pycfn.com/gtvuhqholb.html

el.classList.toggle("active")
来源：http://hz.svipenyu.cn/gtxnwjeupu.html

[U102] JS：本地存储
来源：http://hz.nanxuanxn.top/gtpfuacdxs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuxming.cn/gtkkjmgsbe.html

[U103] JS：定时器
来源：http://hz.smart0.xyz/gtgktyhzww.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gtaqtqetng.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtynihsvne.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtedgadysu.html

[U105] JS：节流
来源：http://hz.cdnleiting.top/gtzmgfgiqg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nwbrower.top/gtivhzfsal.html

[U106] JS：日期格式化
来源：http://hz.yonumen.top/gttcfjhzxe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yongpay.top/gtbfejfhfs.html

[U107] JS：数字千分位
来源：http://hz.yuanzhike.top/gtemmmjsoo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.fzhhl.top/gtuljltvgk.html

[U108] JS：随机整数
来源：http://hz.yuanzhike.top/gtflqzjpuh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hnqzz.top/gtriqfampf.html

[U109] JS：数组分组
来源：http://hz.zhijiandao.cn/gtczffmhqu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtgilzjhbd.html

[U110] JS：数组分块
来源：http://hz.mhx1999.top/gtxqpesolh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xinyue.icu/gtzcgprhvi.html

[U111] JS：对象转 Map
来源：http://hz.nanxinkj.top/gtndphhxrj.html

new Map(Object.entries(obj))
来源：http://hz.jianghu66.top/gtkncwikej.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangtech.top/gtddtrqaov.html

"7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtrnniuykh.html

[U113] JS：正则替换全部
来源：http://hz.mhx1999.top/gtdxolpotj.html

s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtziqyhduy.html

[U114] JS：JSON 深比较
来源：http://hz.haohaochexian.top/gtvseruawa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cheryme.top/gtoznodzim.html

[U115] JS：生成 UUID
来源：http://hz.jinqigufen.top/gtompzjllg.html

crypto.randomUUID()
来源：http://hz.zhixingplan.top/gtiupreipj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jqgfzy.top/gtvqdcthvs.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dashuyun.cn/gtfujhwfhb.html

[U117] JS：单元测试
来源：http://hz.zdqjudy.top/gtgohnijqq.html

npm i -D vitest;  npx vitest
来源：http://hz.jinqigfzy.top/gtqzookmps.html

[U118] JS：开发服务器
来源：http://hz.andypj.xyz/gtlybbvpku.html

npm i -D vite;  npx vite
来源：http://hz.chenlongwang.top/gtvjucfhge.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtturxxvpj.html

npx vite build
来源：http://hz.zycfv.cn/gtqijxiqow.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinghuilouyu.cn/gtwdebfggq.html

import.meta.env.VITE_API_URL
来源：http://hz.sysykeji.top/gtvoimiwvb.html

================================================================================
来源：http://hz.yj20258.top/gtjzrxsbiu.html

统计汇总
来源：http://hz.ppjwa.cn/gtdlgvpbvm.html

================================================================================
来源：http://hz.yj202588.top/gtnsedgeou.html

按语言统计（条）：
来源：http://hz.vqdsnc.cn/gtlueyxhrk.html

Python ......... 252
来源：http://hz.shangyingyoupin.top/gtprqihcjp.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtcrriikmn.html

JavaScript ..... 252
来源：http://hz.tian-w.cn/gtperhqnoj.html

TypeScript ..... 212
来源：http://hz.yj202588.top/gteubnfmvm.html

Java ........... 212
来源：http://hz.yongpay.top/gthxycuezi.html

Go ............. 212
来源：http://hz.cucudq.cn/gtiyzxxfak.html

Ruby ........... 212
来源：http://hz.ydzc1.top/gtflxxrvpb.html

C# ............. 212
来源：http://hz.9152youxi.cn/gtievsspnn.html

C .............. 30
来源：http://hz.quarkkingdee.top/gtksqpblgv.html

C++ ............ 30
来源：http://hz.zhiwuduotai.top/gtramwpxfc.html

SQL ............ 90
来源：http://hz.fengsongda.top/gtmdrcbdui.html

Bash ........... 80
来源：http://hz.aizwys.cn/gtjsixmlup.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtkksxccqj.html

Swift .......... 15
来源：http://hz.yonumen.top/gtltzxmgpl.html

Lua ............ 10
来源：http://hz.pengpengdd.cyou/gtuivckhkf.html

Perl ........... 10
来源：http://hz.yuanzhike.top/gtxaqayobl.html

Scala .......... 10
来源：http://hz.redwolf501.top/gtttwkbuic.html

------------------------------------
来源：http://hz.ydjk.org.cn/gtsdhubewk.html

合计 ........... 2106 条
来源：http://hz.mhx1999.top/gtihoxbeoa.html

按章节统计：
来源：http://hz.gotoacloud.top/gtrbrwcwic.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtqpwaykua.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangkeji.top/gtlbrovqia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtgfqjtuyd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtstxgrzch.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yvedp.cn/gtyptwecza.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhongyouzk.top/gtnaaihgup.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtuauhsuce.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtnrfmcmga.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtyencmsif.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhoulong.xyz/gtddublfby.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtlnmhffpa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtcktjplgl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtpqezuddu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xingfuxueyuan.xyz/gtpiaaagdb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhiwuduotai.top/gtizswhsjg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtxtnsqpiu.html

Q SQL 专题                              90
来源：http://hz.yvedp.cn/gtkcrqymbd.html

R Bash 专题                             80
来源：http://hz.316326.xyz/gtdrmyuror.html

S C / C++ 专题                          60
来源：http://hz.pycfn.com/gtmtiumjbi.html

T 其他语言补充                          60
来源：http://hz.wangshuangyany.cn/gtrbsqowmv.html

U 高频实用片段                         120
来源：http://hz.0kj1m.cn/gtqtgygrqb.html

------------------------------------
来源：http://hz.sufxvd.cn/gtrjunzewk.html

合计                                  2106 条
来源：http://hz.nanxuanxn.top/gteqqjuyyg.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtokhknwhz.html

使用提醒
来源：http://hz.xylfe.cn/gtrioongdu.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtwnaeymds.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.dashuyun.cn/gtgyygditc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ehwqpu.com/gtqrxbzbqs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sufxvd.cn/gtfnyqidiq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.guannengcc.top/gtgasvldck.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.9152youxi.cn/gtexbcnqxb.html

—— 文件结束 ——
来源：http://hz.birdmap.top/gtqsvbjcls.html

================================================================================
来源：http://hz.9152youxi.cn/gtfskvgcfu.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jqgufenzy.top/gtlsfjusyh.html

Common Programming Examples Cheat Book
来源：http://hz.chenlongwang.top/gtknltlpyc.html

================================================================================
来源：http://hz.meibo888.top/gtcsvyxarp.html

【收录内容】
来源：http://hz.smart0.xyz/gtsjcamviy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinqigufen.top/gtkqjnoolc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.52xcode.cn/gtjpabcfuk.html

SQL · Bash · C · C++
来源：http://hz.zhaomingkeji.xyz/gtwjinvwij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ehwqpu.com/gtpyyjglof.html

【使用说明】
来源：http://hz.9152youxi.cn/gttvjptlxc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.meibo888.top/gthnjfaleo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhaomingkeji.xyz/gtvjvhrqgr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hfpthk.cn/gthgvqaric.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shanyushiyangtech.top/gtxhdzmgdu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gogol.net.cn/gtvfqacstd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hongshengwenyu.top/gtxdpvpbyv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinghuilouyu.cn/gtrgrxbgat.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.sysykeji.top/gtpybutfdn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.dianchejie.cn/gttuzgolpk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tanke756.top/gtrmgrbbby.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nwbrower.top/gtbmhdiqml.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shzxlz.cn/gtgggldvur.html

【文件统计】
来源：http://hz.xingfuxueyuan.xyz/gtpqjpxxxg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pycfn.com/gtlujygyxl.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtkeftuksd.html

目  录
来源：http://hz.ehwqpu.com/gtmhcbzupu.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtrqgsicqi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ydjk.org.cn/gthykyfgbp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hnxiangtu.top/gtoaicfkeh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtwczukqpb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hysaishi.cn/gtlrzeyepi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgufenzy.top/gtkkvcafcr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtysgjsmpw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtaamwgxyc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jqgufenzy.top/gtmcnpbfzw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtqhwxgnhe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtfkxiqriz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtpdbgqgjp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtrnspaafe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtctubcivh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gtnrxmvdni.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sysykeji.top/gtjmylafji.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtezxfgbvt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jinqigufen.top/gtxrjqslfr.html


<!-- 参考信息 -->