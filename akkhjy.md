代发 wailian999

[U23] Py：分块读取大文件
来源：http://hz.guannengcc.top/gtwxtreqcb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gzhubu.top/gtlvaljaal.html

[U24] Py：路径操作
来源：http://hz.shangyingyoupin.top/gtivduxcfj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ppjwa.cn/gtyjqxwann.html

[U25] Py：CSV 按字典读
来源：http://hz.gogol.net.cn/gtddgaanhd.html

csv.DictReader(f)
来源：http://hz.shanyushiyangkeji.top/gtxcycdsfz.html

[U26] Py：并发下载
来源：http://hz.guannengcc.top/gtennbtqfm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.guannengcc.top/gtbfgtaczo.html

[U27] Py：异步 HTTP
来源：http://hz.ywan-chungtsiang.top/gtrogwmcdc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xylfe.cn/gtzlcbhylb.html

[U28] Py：类型别名
来源：http://hz.yuanzhike.top/gtgdneoxaf.html

UserId = int
来源：http://hz.tanke756.top/gtgqgxiknt.html

[U29] Py：属性校验
来源：http://hz.hnxiangtu.top/gtfbfnoupd.html

@property 与 @x.setter 配合
来源：http://hz.aizwys.cn/gttqrzgxnk.html

[U30] Py：数据类
来源：http://hz.zhiwuduotai.top/gtrhirslai.html

@dataclass(slots=True)
来源：http://hz.feifeiyinyue.top/gtfpfjvmip.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtfrgawzfu.html

python -m pytest -q
来源：http://hz.sufxvd.cn/gtysmzqbag.html

[U32] Py：代码格式化
来源：http://hz.zhaomingkeji.xyz/gttspahzdf.html

ruff format . && ruff check --fix .
来源：http://hz.hammf.cn/gtfkipzlfz.html

[U33] Py：打包发布
来源：http://hz.nwbrower.top/gtcegluhpq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zdqjudy.top/gtxrerypoh.html

[U34] Py：判断编码
来源：http://hz.9152youxi.cn/gturezqtlp.html

chardet.detect(raw)
来源：http://hz.yanxiufei.cn/gtrigwgubr.html

[U35] Py：发送邮件
来源：http://hz.kuanghao11.cn/gtxxxpjtxw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.snrcjt.cn/gtoeqyxvva.html

[U36] Py：定时任务
来源：http://hz.hnqzz.top/gtjumnebzo.html

schedule.every(10).minutes.do(job)
来源：http://hz.gzhubu.top/gtqmutnjoq.html

[U37] Py：读写 Excel
来源：http://hz.wangshuangyany.cn/gtibxrjkir.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jyoumei.cn/gtjueqvxaf.html

[U38] Py：获取脚本所在目录
来源：http://hz.hywenlv.cn/gtdsbiiwpj.html

Path(__file__).resolve().parent
来源：http://hz.daxiang520.top/gtqgapuoge.html

[U39] Py：判断是否在交互环境
来源：http://hz.nanxinkj.top/gtfferqgll.html

sys.stdout.isatty()
来源：http://hz.gzhubu.top/gtxeyyaekf.html

[U40] Py：打印到标准错误
来源：http://hz.cucudq.cn/gtjjptzzjj.html

print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtdinqkpis.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhongyouzk.top/gtxczxuylw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aizwys.cn/gtenhkbbhf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.dianchejie.cn/gtllzcrnvw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenzaomai.com/gthxklwpvs.html

[U43] PHP：声明命名空间
来源：http://hz.wangshuangyany.cn/gtbzsvmtuv.html

namespace App\Http;
来源：http://hz.zhaomingkeji.xyz/gtvqjkpxmj.html

[U44] PHP：开启严格类型
来源：http://hz.jiagoushi.top/gtlutwapvf.html

declare(strict_types=1);
来源：http://hz.jqgufenzy.top/gtljbzptme.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ybcxt.top/gttkoanzat.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtjjgpmllg.html

[U46] PHP：可空类型
来源：http://hz.yongpay.top/gtrgadmbji.html

?string $name = null
来源：http://hz.hammf.cn/gtpaxqatxs.html

[U47] PHP：联合类型
来源：http://hz.nanxuanxn.top/gtfabnnoju.html

int|string $id
来源：http://hz.c1oappe.top/gtpjkpzoyg.html

[U48] PHP：纯枚举
来源：http://hz.aibaodan.cn/gtjkprijhz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258.top/gtkvzkwwkj.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gtsqwtirwe.html

public readonly string $name
来源：http://hz.jqgufenzy.top/gtqqsqbotx.html

[U50] PHP：构造器属性提升
来源：http://hz.yvedp.cn/gtzyoofmxl.html

public function __construct(private int $id) {}
来源：http://hz.tanke756.top/gtckqkabxu.html

[U51] PHP：数组解构
来源：http://hz.xuanzx.com/gtwocjmids.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtpxhtqxkh.html

[U52] PHP：箭头函数
来源：http://hz.9152youxi.cn/gtpiqggivf.html

$double = fn($x) => $x * 2;
来源：http://hz.dashuyun.cn/gtsapxgfpb.html

[U53] PHP：空合并运算符
来源：http://hz.yj20258888.top/gtqqdtcnkg.html

$v = $a ?? $b ?? "default";
来源：http://hz.kuanghao11.cn/gthmwjltok.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtjegledqo.html

$obj?->method()
来源：http://hz.mhx1999.top/gtswuxxoah.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangkeji.top/gtxkcqrnip.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aibaodan.cn/gtuxpxajjh.html

[U56] PHP：命名参数
来源：http://hz.xuetiantiany.cn/gtwwwzfrtm.html

f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtcmfpujhs.html

[U57] PHP：字符串插值
来源：http://hz.tanke756.top/gtgrsbdvjm.html

"值: {$a}"
来源：http://hz.ppjwa.cn/gtrqdtqrqk.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtaeqsrnhp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shangyingyoupin.top/gtshgiyhli.html

[U59] PHP：自定义排序
来源：http://hz.yvedp.cn/gtiooqpcsk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtbbdrdobe.html

[U60] PHP：JSON 编解码
来源：http://hz.zycfv.cn/gtknwlelsb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.aibaodan.cn/gtjpnnmpfq.html

[U61] PHP：正则
来源：http://hz.jqgfzy.top/gtfqjkqttf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gtirtiappc.html

[U62] PHP：日期对象
来源：http://hz.gotoacloud.top/gtzcccxhcn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yonumen.top/gtbvkwzsbu.html

[U63] PHP：文件读写
来源：http://hz.yanxiufei.cn/gtraubfqwf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yangfankeji.com/gtgraxmceg.html

[U64] PHP：目录遍历
来源：http://hz.zdqjudy.top/gtvougyjgj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nanxinkj.top/gtqrqptyjq.html

[U65] PHP：会话
来源：http://hz.hammf.cn/gtisxedakb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hammf.cn/gtkisgiaze.html

[U66] PHP：设置 Cookie
来源：http://hz.gzhubu.top/gtkkngpkiv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jqgufenzy.top/gtzfkzekdm.html

[U67] PHP：处理文件上传
来源：http://hz.sysykeji.top/gtvgosfgpc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gttbsmycdp.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigufen.top/gtbedybegn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jianghu66.top/gtvqqolutx.html

[U69] PHP：PDO 预处理
来源：http://hz.zhixingplan.top/gtafdfrmzn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gtnpkhvvut.html

[U70] PHP：PDO 事务
来源：http://hz.316326.xyz/gtxbpxjqfr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhengqikj.top/gtqlilqfgj.html

[U71] PHP：抛出异常
来源：http://hz.bjfxy.top/gtjuvhpvvp.html

throw new RuntimeException("失败", 500);
来源：http://hz.ydjk.org.cn/gtegvtulin.html

[U72] PHP：写错误日志
来源：http://hz.ydzc1.top/gtxqxfsdtl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.c1oappe.top/gtnhdsnrwh.html

[U73] PHP：读取 ini 配置
来源：http://hz.gotoacloud.top/gtlwdmlblx.html

parse_ini_file("config.ini", true)
来源：http://hz.jqgufenzy.top/gttnxdatlt.html

[U74] PHP：读取环境变量
来源：http://hz.meibo888.top/gttdetxcvq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yangfankeji.com/gtlzgvdjwr.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gtkegsuniv.html

composer require psr/container
来源：http://hz.yj20258888.top/gtsmttgidy.html

[U76] PHP：简单路由
来源：http://hz.cashguo.top/gtvshfkpkk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.havefunace.top/gthnhdbidw.html

[U77] PHP：模板渲染
来源：http://hz.gaohongyu789.top/gtafpultkw.html

composer require twig/twig
来源：http://hz.sxryk.cn/gtsnixybbi.html

[U78] PHP：单元测试
来源：http://hz.xingfuxueyuan.xyz/gtdirwktgo.html

composer require --dev phpunit/phpunit
来源：http://hz.yongpay.top/gtnnrmazps.html

[U79] PHP：静态分析
来源：http://hz.yueranfly.top/gtqdzdejgo.html

composer require --dev phpstan/phpstan
来源：http://hz.hongshengwenyu.top/gtvihpsmgp.html

[U80] PHP：代码规范修复
来源：http://hz.mhx1999.top/gtfaqsjiwy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.mhx1999.top/gtxvwiaaex.html

[U81] JS：初始化项目
来源：http://hz.xinyue.icu/gtnonutxqv.html

npm init -y;  npm i express
来源：http://hz.bjfxy.top/gterccveim.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangtech.top/gtckawhmkw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinyuanbaomall.cn/gtxjjdzkjh.html

[U83] JS：ES Module 导入导出
来源：http://hz.yj20258888.top/gtfabjxnnj.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ydjk.org.cn/gtmzhxzykb.html

[U84] JS：CommonJS 写法
来源：http://hz.meibo888.top/gtqgcfvoom.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj202588.top/gtczpvjvjh.html

[U85] JS：可选链
来源：http://hz.jiagoushi.top/gtfslyylhm.html

a?.b?.c
来源：http://hz.hnqzz.top/gtdlhgauwh.html

[U86] JS：空值合并
来源：http://hz.andypj.xyz/gtttkmymra.html

a ?? b
来源：http://hz.daxiang520.top/gthywspjvm.html

[U87] JS：解构默认值
来源：http://hz.xuanzx.com/gticqrydgb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gzhubu.top/gtzqfehwnj.html

[U88] JS：对象展开合并
来源：http://hz.ivvv.top/gtxmmzequt.html

{ ...a, ...b }
来源：http://hz.gotoacloud.top/gtdqyzjkpu.html

[U89] JS：数组去重
来源：http://hz.daria6918.cn/gtwrxyphjz.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gtilnezhxm.html

[U90] JS：数字数组排序
来源：http://hz.jinqigfzy.top/gtpmzzqmkv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtzuxqibgo.html

[U91] JS：对象键值遍历
来源：http://hz.gzhubu.top/gtgejwibit.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhengqikj.top/gthkevvuwj.html

[U92] JS：深拷贝
来源：http://hz.xziqi.cn/gtuxujfmby.html

structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtfpdmmpfs.html

[U93] JS：模板字符串
来源：http://hz.quarkkingdee.top/gtqzuufghk.html

`共 ${n} 条`
来源：http://hz.cdnleiting.top/gtvaqdlutl.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gtmuyrrcjc.html

const double = x => x * 2;
来源：http://hz.ydjk.org.cn/gtyatiwqns.html

[U95] JS：Promise 包装
来源：http://hz.zhixingplan.top/gtqqckjnvq.html

new Promise((resolve, reject) => {})
来源：http://hz.shanyushiyangtech.top/gtqlyroykc.html

[U96] JS：async/await 与异常
来源：http://hz.gogol.net.cn/gtpwbeabav.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sxryk.cn/gtbanbssub.html

[U97] JS：并发请求
来源：http://hz.zhongyouzk.top/gtdwtemaku.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtmfduzdrj.html

[U98] JS：fetch 带 JSON
来源：http://hz.sufxvd.cn/gtwwnmtblt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhixingplan.top/gtvueoknwb.html

[U99] JS：事件监听
来源：http://hz.ydzc1.top/gttvpwwozk.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangtech.top/gtqfmavfel.html

[U100] JS：DOM 查询
来源：http://hz.sxryk.cn/gticqwzzmy.html

document.querySelector(".item")
来源：http://hz.yj20258.top/gtvvgnvjml.html

[U101] JS：classList 操作
来源：http://hz.jinqigufen.top/gtwzrpvign.html

el.classList.toggle("active")
来源：http://hz.yj20258888.top/gtlyeihspe.html

[U102] JS：本地存储
来源：http://hz.ywan-chungtsiang.top/gtlelktmiz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenzaomai.com/gtzcsotypu.html

[U103] JS：定时器
来源：http://hz.yanxiufei.cn/gtiwnpewit.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gogol.net.cn/gtfjalcjzx.html

[U104] JS：防抖
来源：http://hz.iojbl.cn/gtcgrfhgef.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtulsmjqmb.html

[U105] JS：节流
来源：http://hz.chenjidiqi.icu/gtdyjvsrip.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.c1oappe.top/gtxivyjxav.html

[U106] JS：日期格式化
来源：http://hz.hysaishi.cn/gteqsqjguc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sysykeji.top/gtazofruea.html

[U107] JS：数字千分位
来源：http://hz.fzhhl.top/gtchxhbwtk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydjk.org.cn/gtoryopywn.html

[U108] JS：随机整数
来源：http://hz.daria6918.cn/gtydfconxo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtrwrcjkap.html

[U109] JS：数组分组
来源：http://hz.jinghuilouyu.cn/gtuujlclsr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtsvadytsz.html

[U110] JS：数组分块
来源：http://hz.mhx1999.top/gtkgyoeeva.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuetiantiany.cn/gtmrhwbpoy.html

[U111] JS：对象转 Map
来源：http://hz.cucudq.cn/gtutvtmiiy.html

new Map(Object.entries(obj))
来源：http://hz.fengsongda.top/gtywlcficl.html

[U112] JS：字符串补位
来源：http://hz.nanxinkj.top/gtsyyujwux.html

"7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtosmdxbbc.html

[U113] JS：正则替换全部
来源：http://hz.jlsjyb.cn/gtbcgzsxgo.html

s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtpotoeqow.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtrprpjfkt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtjdonmjbm.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gtubbwydrm.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gtifubfjrz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhixingplan.top/gtbbdytqgv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tianlin.xyz/gtthaojfvm.html

[U117] JS：单元测试
来源：http://hz.tian-w.cn/gtaupbohia.html

npm i -D vitest;  npx vitest
来源：http://hz.hywenlv.cn/gtjqmcgdfn.html

[U118] JS：开发服务器
来源：http://hz.daxiang520.top/gtmznpaqlb.html

npm i -D vite;  npx vite
来源：http://hz.haohaochexian.top/gtdpgpdtxc.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gtayagftwd.html

npx vite build
来源：http://hz.zdqjudy.top/gtlndhiija.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangkeji.top/gtavmojzam.html

import.meta.env.VITE_API_URL
来源：http://hz.chenzaomai.com/gtejmnasip.html

================================================================================
来源：http://hz.52xcode.cn/gtmddmrhap.html

统计汇总
来源：http://hz.daria6918.cn/gtthpffvxj.html

================================================================================
来源：http://hz.sxryk.cn/gtxyecmkyc.html

按语言统计（条）：
来源：http://hz.ywan-chungtsiang.top/gtrdnrjgwo.html

Python ......... 252
来源：http://hz.yonumen.top/gtctisaoem.html

PHP ............ 252
来源：http://hz.52xcode.cn/gtueddzplm.html

JavaScript ..... 252
来源：http://hz.ydzc1.top/gtyjjrodux.html

TypeScript ..... 212
来源：http://hz.zhiwuduotai.top/gtlsfyubsc.html

Java ........... 212
来源：http://hz.cashguo.top/gtmvigudlu.html

Go ............. 212
来源：http://hz.cdnleiting.top/gtodzjnmzt.html

Ruby ........... 212
来源：http://hz.316326.xyz/gtjmgwywqm.html

C# ............. 212
来源：http://hz.zdqjudy.top/gtwliyiuss.html

C .............. 30
来源：http://hz.zhiwuduotai.top/gtkztxtxgi.html

C++ ............ 30
来源：http://hz.shzxlz.cn/gtqwnywkng.html

SQL ............ 90
来源：http://hz.nanxuanxn.top/gtqwspbqxm.html

Bash ........... 80
来源：http://hz.vqdsnc.cn/gtnbsgatcs.html

Kotlin ......... 15
来源：http://hz.aizwys.cn/gtrkgbazkd.html

Swift .......... 15
来源：http://hz.hongshengwenyu.top/gtmjajstpg.html

Lua ............ 10
来源：http://hz.dianchejie.cn/gtorovmabo.html

Perl ........... 10
来源：http://hz.nanxuanxn.top/gtfxmepppp.html

Scala .......... 10
来源：http://hz.sweek.top/gtezhtbsqb.html

------------------------------------
来源：http://hz.gogol.net.cn/gthlnyhhrl.html

合计 ........... 2106 条
来源：http://hz.cheryme.top/gtyhcteveu.html

按章节统计：
来源：http://hz.andypj.xyz/gtuslqkmfx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtnxknqjko.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtlxrjipml.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtyjufgskj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gtromfnlzm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aibaodan.cn/gtsgxbzhxm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtujdwbxxh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtxdofjhtp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gttqplayks.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtmffdipyo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.bjfxy.top/gteoaoselj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gttjpaaobk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtogsewuou.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtvbdnfvbo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtgajhjuwf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tianlin.xyz/gtbinnlhqn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtjwmfqeqv.html

Q SQL 专题                              90
来源：http://hz.yj20258.top/gtcmeaxvtj.html

R Bash 专题                             80
来源：http://hz.sysykeji.top/gtpjkwxkdn.html

S C / C++ 专题                          60
来源：http://hz.snrcjt.cn/gtqptazjnv.html

T 其他语言补充                          60
来源：http://hz.sufxvd.cn/gtrkhidqwo.html

U 高频实用片段                         120
来源：http://hz.zhijiandao.cn/gtwvpbtnpr.html

------------------------------------
来源：http://hz.shanyushiyangtech.top/gtdpxrcelw.html

合计                                  2106 条
来源：http://hz.zycfv.cn/gthlvywntw.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gttoetjmwj.html

使用提醒
来源：http://hz.pycfn.com/gtjzokiqkp.html

--------------------------------------------------------------------------------
来源：http://hz.shangyingyoupin.top/gttzhxehmo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sweek.top/gtmlrcddbb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinqigufen.top/gtdewakppd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhaomingkeji.xyz/gtauyxypfp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cheryme.top/gthlqcckqq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhixingplan.top/gtkseotqlj.html

—— 文件结束 ——
来源：http://hz.tianlin.xyz/gtesajyqgr.html

================================================================================
来源：http://hz.guannengcc.top/gtjdxgfnjf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yueranfly.top/gtzlouybwc.html

Common Programming Examples Cheat Book
来源：http://hz.dianchejie.cn/gtsmalqjme.html

================================================================================
来源：http://hz.nwbrower.top/gtukrcfodt.html

【收录内容】
来源：http://hz.shzxlz.cn/gtzmhbztcg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jianghu66.top/gtrslfnkzx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.aizwys.cn/gtihpkbahw.html

SQL · Bash · C · C++
来源：http://hz.zhijiandao.cn/gtmbuxnvjk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhixingplan.top/gtiswvwxbo.html

【使用说明】
来源：http://hz.ywan-chungtsiang.top/gtsunliczt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shzxlz.cn/gtfurxxrnb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.snrcjt.cn/gtvkkhxnea.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtkfwrvnon.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zycfv.cn/gthxzxwfra.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj20258.top/gturabpjwr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hnxiangtu.top/gteoajezsr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dashuyun.cn/gtdlbagllz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xziqi.cn/gtcscomytc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.snrcjt.cn/gtixpqkmlg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yuanzhike.top/gttiqxfdgg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhoulong.xyz/gtzvmcyykj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.birdmap.top/gttrfbgmqr.html

【文件统计】
来源：http://hz.guowangkeji.top/gtktoppemq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jinqigfzy.top/gtzlhameli.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtkgpyipie.html

目  录
来源：http://hz.mhx1999.top/gtfozfmbkx.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gtbqznfmqy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yvedp.cn/gterddkmlw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shzxlz.cn/gtbcusvwle.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.quarkkingdee.top/gtuuiqxauw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.nwbrower.top/gtqaavrtfn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhengqikj.top/gtcjjvpcqu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.dianchejie.cn/gtmvjsewsy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtlkdifong.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nwbrower.top/gtpktrgsdb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtetrgiatz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.svipenyu.cn/gtfhawmjid.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtwtwnrwxe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtohcnmdpm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtbbebeuqy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xingfuxueyuan.xyz/gtjqbgriqn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.redwolf501.top/gtmbqyugwy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtpvesqfmq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.aibaodan.cn/gtqbuxoaee.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gtlpyzqdwg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinyuanbaomall.cn/gtwhftwwzy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtfdbahmya.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhijiandao.cn/gtextwjdoz.html


<!-- 参考信息 -->