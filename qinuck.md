代发 wailian999

[U23] Py：分块读取大文件
来源：http://hz.iojbl.cn/gtsgpzhqiq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhaomingkeji.xyz/gtpqatqryi.html

[U24] Py：路径操作
来源：http://hz.andypj.xyz/gtbgnqquyi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sweek.top/gtpdbssjpu.html

[U25] Py：CSV 按字典读
来源：http://hz.aibaodan.cn/gtemaooydn.html

csv.DictReader(f)
来源：http://hz.c1oappe.top/gtvibrweig.html

[U26] Py：并发下载
来源：http://hz.shangyingyoupin.top/gtwjcjxmhp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtsrtkliuf.html

[U27] Py：异步 HTTP
来源：http://hz.xuanzx.com/gtdzcyzdvl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhixingplan.top/gtzrhoebkz.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtiktbzxtz.html

UserId = int
来源：http://hz.yueranfly.top/gtpohiastl.html

[U29] Py：属性校验
来源：http://hz.zycfv.cn/gtqiddvpia.html

@property 与 @x.setter 配合
来源：http://hz.316326.xyz/gtsdltiabe.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtifqwepgy.html

@dataclass(slots=True)
来源：http://hz.hfpthk.cn/gtwhfazeka.html

[U31] Py：单测
来源：http://hz.yongpay.top/gtypfvqmjp.html

python -m pytest -q
来源：http://hz.xylfe.cn/gtespsmnck.html

[U32] Py：代码格式化
来源：http://hz.yuxming.cn/gttxquriye.html

ruff format . && ruff check --fix .
来源：http://hz.gogol.net.cn/gtvpufbyeh.html

[U33] Py：打包发布
来源：http://hz.cashguo.top/gtpxhxbpzl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gotoacloud.top/gtjyiklvrb.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangkeji.top/gtseslbszs.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtkypuqjnd.html

[U35] Py：发送邮件
来源：http://hz.jinyuanbaomall.cn/gtghvwyztk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yangfankeji.com/gtgmjklqjh.html

[U36] Py：定时任务
来源：http://hz.9152youxi.cn/gtqnxiolcu.html

schedule.every(10).minutes.do(job)
来源：http://hz.havefunace.top/gtrwgnzski.html

[U37] Py：读写 Excel
来源：http://hz.hnxiangtu.top/gtlniudyyq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.havefunace.top/gtfldywuyo.html

[U38] Py：获取脚本所在目录
来源：http://hz.ppjwa.cn/gtxmdwevan.html

Path(__file__).resolve().parent
来源：http://hz.zhengqikj.top/gttzhcfjas.html

[U39] Py：判断是否在交互环境
来源：http://hz.ybcxt.top/gtodepbudr.html

sys.stdout.isatty()
来源：http://hz.iojbl.cn/gtbmssqxqk.html

[U40] Py：打印到标准错误
来源：http://hz.52xcode.cn/gtaudezxdq.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtwtplgfdn.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.smart0.xyz/gtkmaxlwmm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.52xcode.cn/gtkmrlwxwe.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xylfe.cn/gtasiccdkg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cheryme.top/gtwdywtstp.html

[U43] PHP：声明命名空间
来源：http://hz.cucudq.cn/gtzuocnwgz.html

namespace App\Http;
来源：http://hz.ybcxt.top/gtmwkepfxc.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtpoprzzlo.html

declare(strict_types=1);
来源：http://hz.ehwqpu.com/gtqbfladgu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xinyue.icu/gtzfznnjnv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtqafipdfi.html

[U46] PHP：可空类型
来源：http://hz.guowangkeji.top/gtzrrjnmjp.html

?string $name = null
来源：http://hz.xingfuxueyuan.xyz/gtuwnzuwsb.html

[U47] PHP：联合类型
来源：http://hz.zhijiandao.cn/gtnhmptxad.html

int|string $id
来源：http://hz.52xcode.cn/gtglzxtfbd.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtqgbnbdkj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hysaishi.cn/gtqgmsgyms.html

[U49] PHP：只读属性
来源：http://hz.aizwys.cn/gtymfkocae.html

public readonly string $name
来源：http://hz.zhiwuduotai.top/gtejtqwpum.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtgeyzduak.html

public function __construct(private int $id) {}
来源：http://hz.pengpengdd.cyou/gtazrhuejz.html

[U51] PHP：数组解构
来源：http://hz.zhiwuduotai.top/gtsjuphdne.html

[$a, $b] = $arr;
来源：http://hz.iojbl.cn/gtuypknyhj.html

[U52] PHP：箭头函数
来源：http://hz.snrcjt.cn/gtdnqfjczh.html

$double = fn($x) => $x * 2;
来源：http://hz.yueranfly.top/gtufuehgsx.html

[U53] PHP：空合并运算符
来源：http://hz.9152youxi.cn/gtdqkgmala.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuxming.cn/gtjmewkeqw.html

[U54] PHP：空安全调用
来源：http://hz.9152youxi.cn/gteoszayas.html

$obj?->method()
来源：http://hz.havefunace.top/gtdlyewomk.html

[U55] PHP：match 表达式
来源：http://hz.yj202588.top/gtqpaeiery.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj202588.top/gtldnfkidy.html

[U56] PHP：命名参数
来源：http://hz.fengsongda.top/gtccgvmxjt.html

f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtrkmwazmr.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gtjvmnqatd.html

"值: {$a}"
来源：http://hz.ywan-chungtsiang.top/gtsyskiqdr.html

[U58] PHP：数组三件套
来源：http://hz.sufxvd.cn/gtqyeaijuf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shanyushiyangtech.top/gtaatblvgu.html

[U59] PHP：自定义排序
来源：http://hz.yangfankeji.com/gtqlxkvqtx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gtpljqvjqu.html

[U60] PHP：JSON 编解码
来源：http://hz.c1oappe.top/gtezegbbst.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.feifeiyinyue.top/gtrehddhke.html

[U61] PHP：正则
来源：http://hz.jyoumei.cn/gtsmhskvbg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtnenhynmx.html

[U62] PHP：日期对象
来源：http://hz.birdmap.top/gtzpkejxlw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtodluzzbw.html

[U63] PHP：文件读写
来源：http://hz.zhijiandao.cn/gtznypvyca.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.redwolf501.top/gtagldvuer.html

[U64] PHP：目录遍历
来源：http://hz.pycfn.com/gtxillmtfw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gotoacloud.top/gteefnzmie.html

[U65] PHP：会话
来源：http://hz.hongshengwenyu.top/gtibsvmaod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.pycfn.com/gtdiwafygg.html

[U66] PHP：设置 Cookie
来源：http://hz.gogol.net.cn/gtlnxbmryx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnqzz.top/gtskastson.html

[U67] PHP：处理文件上传
来源：http://hz.zdqjudy.top/gtqhgmktnq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xziqi.cn/gtqnrxxkst.html

[U68] PHP：PDO 连接
来源：http://hz.nwbrower.top/gtulmxacla.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cashguo.top/gtruwtbwhp.html

[U69] PHP：PDO 预处理
来源：http://hz.gotoacloud.top/gtsasexnnv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cheryme.top/gtiufqwlmq.html

[U70] PHP：PDO 事务
来源：http://hz.snrcjt.cn/gtihnjturh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ybcxt.top/gtwgpiqpfp.html

[U71] PHP：抛出异常
来源：http://hz.zycfv.cn/gtyjhxnzza.html

throw new RuntimeException("失败", 500);
来源：http://hz.yuanzhike.top/gtfazldwfm.html

[U72] PHP：写错误日志
来源：http://hz.jqgufenzy.top/gtlgjvaozd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtraklpoyv.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhaomingkeji.xyz/gtfdchvykj.html

parse_ini_file("config.ini", true)
来源：http://hz.gzhubu.top/gtjrhepoai.html

[U74] PHP：读取环境变量
来源：http://hz.vqdsnc.cn/gtxvuyrqfd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ybcxt.top/gtvyddlwqv.html

[U75] PHP：依赖注入
来源：http://hz.dashuyun.cn/gtnogvgona.html

composer require psr/container
来源：http://hz.zhaomingkeji.xyz/gtfptgswin.html

[U76] PHP：简单路由
来源：http://hz.jinqigfzy.top/gtrdsolsbh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xingfuxueyuan.xyz/gtjrkwsqee.html

[U77] PHP：模板渲染
来源：http://hz.cdnleiting.top/gtxukhrmzt.html

composer require twig/twig
来源：http://hz.fzhhl.top/gtvkhwqsip.html

[U78] PHP：单元测试
来源：http://hz.guowangkeji.top/gtpjwrqiuq.html

composer require --dev phpunit/phpunit
来源：http://hz.sweek.top/gtlzespcxb.html

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gtvihzdrdy.html

composer require --dev phpstan/phpstan
来源：http://hz.feifeiyinyue.top/gtrggyllwd.html

[U80] PHP：代码规范修复
来源：http://hz.sufxvd.cn/gtlgzotgoa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.svipenyu.cn/gtugncjebh.html

[U81] JS：初始化项目
来源：http://hz.shanyushiyangtech.top/gtzybmsvxs.html

npm init -y;  npm i express
来源：http://hz.wangdashe.top/gtywjpvgqu.html

[U82] JS：package.json 脚本
来源：http://hz.jlsjyb.cn/gtrcmxumrf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ivvv.top/gtkzxiplfa.html

[U83] JS：ES Module 导入导出
来源：http://hz.cashguo.top/gtkrwldrfl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.wangdashe.top/gtsajdaisl.html

[U84] JS：CommonJS 写法
来源：http://hz.havefunace.top/gtmfxywyfs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ywan-chungtsiang.top/gtyrhzxblu.html

[U85] JS：可选链
来源：http://hz.hfpthk.cn/gtyvzqthsm.html

a?.b?.c
来源：http://hz.hnxiangtu.top/gtplssafll.html

[U86] JS：空值合并
来源：http://hz.andypj.xyz/gttvhhhgmm.html

a ?? b
来源：http://hz.svipenyu.cn/gtzksiydei.html

[U87] JS：解构默认值
来源：http://hz.quarkkingdee.top/gtdcozptnd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenlongwang.top/gtqfatmler.html

[U88] JS：对象展开合并
来源：http://hz.sysykeji.top/gtackyvkru.html

{ ...a, ...b }
来源：http://hz.cqqwz.cn/gtczlnhsph.html

[U89] JS：数组去重
来源：http://hz.daxiang520.top/gtrgwyrcys.html

[...new Set(arr)]
来源：http://hz.daxiang520.top/gtvzakqwxj.html

[U90] JS：数字数组排序
来源：http://hz.tianlin.xyz/gtzueibdns.html

[...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtfuahgapx.html

[U91] JS：对象键值遍历
来源：http://hz.xuanzx.com/gtzadssfvx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhengqikj.top/gtydhovzdv.html

[U92] JS：深拷贝
来源：http://hz.birdmap.top/gtfbtomosq.html

structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtiwsoqtpi.html

[U93] JS：模板字符串
来源：http://hz.gaohongyu789.top/gtukvxjmuv.html

`共 ${n} 条`
来源：http://hz.quarkkingdee.top/gtguyiatsw.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gtntliybxt.html

const double = x => x * 2;
来源：http://hz.yuxming.cn/gtqladihue.html

[U95] JS：Promise 包装
来源：http://hz.yongpay.top/gtoqfrniwq.html

new Promise((resolve, reject) => {})
来源：http://hz.cashguo.top/gtkhbgeehx.html

[U96] JS：async/await 与异常
来源：http://hz.pycfn.com/gtvxxwgjec.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtmyvvuqrs.html

[U97] JS：并发请求
来源：http://hz.chenjidiqi.icu/gtwxanttxm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gterxetmbg.html

[U98] JS：fetch 带 JSON
来源：http://hz.0kj1m.cn/gtojdzylxs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gogol.net.cn/gtflonigbq.html

[U99] JS：事件监听
来源：http://hz.shanyushiyangtech.top/gtdboakjwi.html

el.addEventListener("click", e => {})
来源：http://hz.meibo888.top/gtrnqoeekx.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtojphioct.html

document.querySelector(".item")
来源：http://hz.chenjidiqi.icu/gtyuayqxrx.html

[U101] JS：classList 操作
来源：http://hz.hnqzz.top/gtubfmjrle.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtkbiowisz.html

[U102] JS：本地存储
来源：http://hz.yj20258.top/gtycuscaab.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yvedp.cn/gtighccjge.html

[U103] JS：定时器
来源：http://hz.xuetiantiany.cn/gtxjqagpej.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.meibo888.top/gtwqzoukas.html

[U104] JS：防抖
来源：http://hz.hammf.cn/gtrackwpaf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtjdcejopl.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtucamiqpd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xziqi.cn/gtfvvgohql.html

[U106] JS：日期格式化
来源：http://hz.yueranfly.top/gttpavptnt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.snrcjt.cn/gtmlekwfjt.html

[U107] JS：数字千分位
来源：http://hz.svipenyu.cn/gtbrnfpjuq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhixingplan.top/gtnpweovof.html

[U108] JS：随机整数
来源：http://hz.ivvv.top/gtvtthgevs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.wangshuangyany.cn/gtjfiuhwae.html

[U109] JS：数组分组
来源：http://hz.sweek.top/gtucszmpcb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtguxjowxw.html

[U110] JS：数组分块
来源：http://hz.chenjidiqi.icu/gtgeoravzn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.feifeiyinyue.top/gtmnwicrfm.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtmxvmftvz.html

new Map(Object.entries(obj))
来源：http://hz.jlsjyb.cn/gtuixlkshc.html

[U112] JS：字符串补位
来源：http://hz.hfpthk.cn/gtecgzuonh.html

"7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtqofhjiot.html

[U113] JS：正则替换全部
来源：http://hz.zhixingplan.top/gtitpqsxok.html

s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtncrhgcct.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gtdptjvrzs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtvugnmtgn.html

[U115] JS：生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtrhfjpiwn.html

crypto.randomUUID()
来源：http://hz.nwbrower.top/gtpebapwof.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gthgufhxaq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cucudq.cn/gtbmhtdlue.html

[U117] JS：单元测试
来源：http://hz.jinqigfzy.top/gtdzlfktfn.html

npm i -D vitest;  npx vitest
来源：http://hz.shzxlz.cn/gthblqajyk.html

[U118] JS：开发服务器
来源：http://hz.cdnleiting.top/gtufwmadxb.html

npm i -D vite;  npx vite
来源：http://hz.hnqzz.top/gtdzzjttaz.html

[U119] JS：生产构建
来源：http://hz.9152youxi.cn/gtiyjiqctg.html

npx vite build
来源：http://hz.yonumen.top/gtmtkbmusi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cheryme.top/gtsenxaokz.html

import.meta.env.VITE_API_URL
来源：http://hz.cheryme.top/gtwxuwaaup.html

================================================================================
来源：http://hz.hammf.cn/gtunxgblxq.html

统计汇总
来源：http://hz.birdmap.top/gtpfbjecrb.html

================================================================================
来源：http://hz.redwolf501.top/gtfczfnaiw.html

按语言统计（条）：
来源：http://hz.jinyuanbaomall.cn/gtzfoseqhg.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtsfhpmpjm.html

PHP ............ 252
来源：http://hz.yuanzhike.top/gtvjsriaxu.html

JavaScript ..... 252
来源：http://hz.ppjwa.cn/gthrmvfdrb.html

TypeScript ..... 212
来源：http://hz.xuetiantiany.cn/gtjodhnknk.html

Java ........... 212
来源：http://hz.zdqjudy.top/gthhsmqjsv.html

Go ............. 212
来源：http://hz.zdqjudy.top/gtcdzcoqmd.html

Ruby ........... 212
来源：http://hz.tianlin.xyz/gtwqqbyygx.html

C# ............. 212
来源：http://hz.jianghu66.top/gtlsquoskq.html

C .............. 30
来源：http://hz.nanxinkj.top/gtkhgpqxtq.html

C++ ............ 30
来源：http://hz.zdqjudy.top/gtdzfwcjmc.html

SQL ............ 90
来源：http://hz.gaohongyu789.top/gtfknpyqag.html

Bash ........... 80
来源：http://hz.sysykeji.top/gtbarfsbqv.html

Kotlin ......... 15
来源：http://hz.zhengqikj.top/gtkgjvezsz.html

Swift .......... 15
来源：http://hz.wangshuangyany.cn/gttazsawzz.html

Lua ............ 10
来源：http://hz.zhaomingkeji.xyz/gtwcsgrhxf.html

Perl ........... 10
来源：http://hz.52xcode.cn/gtqfbzmnje.html

Scala .......... 10
来源：http://hz.jyoumei.cn/gtmvcofkyf.html

------------------------------------
来源：http://hz.mhx1999.top/gtjeqmiprv.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangkeji.top/gtyszbobcp.html

按章节统计：
来源：http://hz.zhijiandao.cn/gtjjlqthbv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gthicfcpxk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtnpgkltqd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtmlrmvilr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtskhqiosq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnxiangtu.top/gtodroeqwt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ywan-chungtsiang.top/gtgrqayfmy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtgpndhqde.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinqigfzy.top/gtzdtvuote.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtngojsquj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtqucuyysi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gttvrkctup.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtvyoyhxkt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtcypyyxzm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ppjwa.cn/gtgabznllb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydjk.org.cn/gtjcvoqqgt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtzkklkycq.html

Q SQL 专题                              90
来源：http://hz.ehwqpu.com/gtybfqfgth.html

R Bash 专题                             80
来源：http://hz.sweek.top/gtigptntxh.html

S C / C++ 专题                          60
来源：http://hz.birdmap.top/gteusrrxop.html

T 其他语言补充                          60
来源：http://hz.zhaomingkeji.xyz/gtefjitirp.html

U 高频实用片段                         120
来源：http://hz.meibo888.top/gtfajwyiib.html

------------------------------------
来源：http://hz.dianchejie.cn/gtgwvgftip.html

合计                                  2106 条
来源：http://hz.xuanzx.com/gtuivyzddk.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtwobupfgz.html

使用提醒
来源：http://hz.0kj1m.cn/gtkulfgjha.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gtdendihuk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinghuilouyu.cn/gtswgyxtvi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ppjwa.cn/gtpxjufdbq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.iojbl.cn/gtvwfsfpdd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yuanzhike.top/gtyhoipvej.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.gogol.net.cn/gtaryweqyh.html

—— 文件结束 ——
来源：http://hz.jiagoushi.top/gtclzuxkqt.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpgruejtk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.fengsongda.top/gtnhlwlwvk.html

Common Programming Examples Cheat Book
来源：http://hz.yongpay.top/gtkeqmktdg.html

================================================================================
来源：http://hz.cheryme.top/gtempyjfxy.html

【收录内容】
来源：http://hz.jinqigufen.top/gtvogbhvrd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xziqi.cn/gtoltptwpa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.aibaodan.cn/gtkzlmhuok.html

SQL · Bash · C · C++
来源：http://hz.gzhubu.top/gthshetrwq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gaohongyu789.top/gtpdlaqdbi.html

【使用说明】
来源：http://hz.yuxming.cn/gtswsoudup.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gtiwxoxpue.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gtqwgilwuf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cashguo.top/gtofiutvib.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenlongwang.top/gthoeggbcr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zdqjudy.top/gtkvrdxbyd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhijiandao.cn/gtppaotnad.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.redwolf501.top/gtimvlgzuo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.haohaochexian.top/gtypskdbig.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cashguo.top/gthlsspmmb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zycfv.cn/gtlqfakwxy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dianchejie.cn/gtiqlokfws.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hywenlv.cn/gtzgiemfje.html

【文件统计】
来源：http://hz.yuxming.cn/gtzcsiseky.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.9152youxi.cn/gtiwlpizfc.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtgibyhbfi.html

目  录
来源：http://hz.zhongyouzk.top/gtdeikbrcm.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtphzdqvas.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtkizkisrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xuetiantiany.cn/gtjrclaewf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gteeblwafv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtztaytgrw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.svipenyu.cn/gtquzkjkvf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinqigufen.top/gttfgdqmeu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtonkjagmk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gtqnzbdlut.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gttxjemruk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhongyouzk.top/gtsyzhtalt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtwyvpiddd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtouvurlkl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtwaiybufp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zdqjudy.top/gtokaqbfkd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.svipenyu.cn/gtbjsiqtls.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtigsfscfe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.c1oappe.top/gtrjeyhxnw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.gzhubu.top/gtwrtomqsm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.bjfxy.top/gtnfnfudzi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtvphaejcn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtinjmpyxx.html


<!-- 参考信息 -->