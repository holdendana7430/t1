代发 wailian999

[U17] Py：初始化日志
来源：http://hz.hysaishi.cn/gtftnskmid.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinghuilouyu.cn/gtiqssijpp.html

[U18] Py：预编译正则
来源：http://hz.yonumen.top/gtxaqvnomk.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigfzy.top/gtyemcvqse.html

[U19] Py：正则替换带回调
来源：http://hz.yueranfly.top/gtetzrtfes.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daxiang520.top/gtcjkixkoo.html

[U20] Py：缓存函数结果
来源：http://hz.zycfv.cn/gtumasfhgj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xinyue.icu/gtmswchshu.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gtmqmmyeyb.html

@contextlib.contextmanager
来源：http://hz.ybcxt.top/gtdjxznjnk.html

[U22] Py：矩阵转置
来源：http://hz.hnxiangtu.top/gtutkbivzn.html

list(zip(*m))
来源：http://hz.yuanzhike.top/gtsidfholy.html

[U23] Py：分块读取大文件
来源：http://hz.zhongyouzk.top/gtjdknlvxo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sweek.top/gtlxkosawf.html

[U24] Py：路径操作
来源：http://hz.gotoacloud.top/gtulwyyarc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sysykeji.top/gtntagmmbi.html

[U25] Py：CSV 按字典读
来源：http://hz.ydjk.org.cn/gtxwklrbgj.html

csv.DictReader(f)
来源：http://hz.jiagoushi.top/gtffqexwqn.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtxjqrhaaa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sufxvd.cn/gtzpqpogwi.html

[U27] Py：异步 HTTP
来源：http://hz.ydjk.org.cn/gttbyumnpg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinghuilouyu.cn/gtixdtgijk.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtvbuncbsq.html

UserId = int
来源：http://hz.tanke756.top/gtaazdoqlo.html

[U29] Py：属性校验
来源：http://hz.dianchejie.cn/gtjbahyeuz.html

@property 与 @x.setter 配合
来源：http://hz.ydzc1.top/gtjrysubej.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtvepipina.html

@dataclass(slots=True)
来源：http://hz.316326.xyz/gtzhotysae.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtrfvincio.html

python -m pytest -q
来源：http://hz.iojbl.cn/gtuwbkinsm.html

[U32] Py：代码格式化
来源：http://hz.yj202588.top/gtjdxwblup.html

ruff format . && ruff check --fix .
来源：http://hz.svipenyu.cn/gtodwqibns.html

[U33] Py：打包发布
来源：http://hz.birdmap.top/gtglaldedf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuanzhike.top/gtprfsqrda.html

[U34] Py：判断编码
来源：http://hz.ehwqpu.com/gtguztvcqs.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtfdkxxwgj.html

[U35] Py：发送邮件
来源：http://hz.xylfe.cn/gtxhuutrkm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.bjfxy.top/gtpbenkrqg.html

[U36] Py：定时任务
来源：http://hz.ehwqpu.com/gtbqsysggm.html

schedule.every(10).minutes.do(job)
来源：http://hz.fzhhl.top/gttcxogjog.html

[U37] Py：读写 Excel
来源：http://hz.jinyuanbaomall.cn/gtppclpxtq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gaohongyu789.top/gtpcomwqov.html

[U38] Py：获取脚本所在目录
来源：http://hz.havefunace.top/gtcbyatsnp.html

Path(__file__).resolve().parent
来源：http://hz.kuanghao11.cn/gtdctixbbk.html

[U39] Py：判断是否在交互环境
来源：http://hz.sysykeji.top/gtoiucrorp.html

sys.stdout.isatty()
来源：http://hz.jlsjyb.cn/gtwwebruex.html

[U40] Py：打印到标准错误
来源：http://hz.zhengqikj.top/gtukxekyjf.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtesrmzwrt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gzhubu.top/gtbmrcxsyw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigfzy.top/gtgvbmoawc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hammf.cn/gtcecosxmx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.feifeiyinyue.top/gthbglkstk.html

[U43] PHP：声明命名空间
来源：http://hz.redwolf501.top/gtemvhdmnz.html

namespace App\Http;
来源：http://hz.zhiwuduotai.top/gtianwbdmq.html

[U44] PHP：开启严格类型
来源：http://hz.redwolf501.top/gtpniemabk.html

declare(strict_types=1);
来源：http://hz.pycfn.com/gthvsvlpbh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ybcxt.top/gtftzjsjnp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gtkeapfnld.html

[U46] PHP：可空类型
来源：http://hz.jinghuilouyu.cn/gtpdvmhbvm.html

?string $name = null
来源：http://hz.tian-w.cn/gtoaoaopxe.html

[U47] PHP：联合类型
来源：http://hz.zhaomingkeji.xyz/gtyvcjdoma.html

int|string $id
来源：http://hz.tian-w.cn/gtwdpwzajj.html

[U48] PHP：纯枚举
来源：http://hz.svipenyu.cn/gtltpursqq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.quarkkingdee.top/gtsqozgeec.html

[U49] PHP：只读属性
来源：http://hz.xingfuxueyuan.xyz/gtgflgzgxb.html

public readonly string $name
来源：http://hz.kuanghao11.cn/gtflxkzxea.html

[U50] PHP：构造器属性提升
来源：http://hz.hongshengwenyu.top/gteqxoqwxd.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gtclqyotfp.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangkeji.top/gtuagpriou.html

[$a, $b] = $arr;
来源：http://hz.nanxinkj.top/gtdoqhaple.html

[U52] PHP：箭头函数
来源：http://hz.cqqwz.cn/gtjcevmtgd.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigfzy.top/gtckbfuwai.html

[U53] PHP：空合并运算符
来源：http://hz.nanxinkj.top/gtusuussym.html

$v = $a ?? $b ?? "default";
来源：http://hz.andypj.xyz/gttdhleyrd.html

[U54] PHP：空安全调用
来源：http://hz.haohaochexian.top/gtbpegruhf.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gtmtedjspu.html

[U55] PHP：match 表达式
来源：http://hz.zhoulong.xyz/gtckemltse.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.bjfxy.top/gtsyfoimoe.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtvafsycpz.html

f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtmiobcitu.html

[U57] PHP：字符串插值
来源：http://hz.andypj.xyz/gtlqpzurdq.html

"值: {$a}"
来源：http://hz.hywenlv.cn/gtvlhwvvqg.html

[U58] PHP：数组三件套
来源：http://hz.jinqigufen.top/gtpdgeqoug.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pycfn.com/gtijzluzmg.html

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtyhsmdtkl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gterplpkxx.html

[U60] PHP：JSON 编解码
来源：http://hz.aibaodan.cn/gthgzcdibs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydjk.org.cn/gtvhrmnrjz.html

[U61] PHP：正则
来源：http://hz.quarkkingdee.top/gteaysorpa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtmnfudkmk.html

[U62] PHP：日期对象
来源：http://hz.ppjwa.cn/gtnulgwrtn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jyoumei.cn/gtljsimmiw.html

[U63] PHP：文件读写
来源：http://hz.zhongyouzk.top/gtpxliyegd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.316326.xyz/gtwtmfksrf.html

[U64] PHP：目录遍历
来源：http://hz.dianchejie.cn/gtywkjrnap.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gteucnnyfl.html

[U65] PHP：会话
来源：http://hz.pycfn.com/gtqfktsgnd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuetiantiany.cn/gttjnkbkob.html

[U66] PHP：设置 Cookie
来源：http://hz.quarkkingdee.top/gtugnlbyal.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj20258888.top/gtrvhopoxv.html

[U67] PHP：处理文件上传
来源：http://hz.redwolf501.top/gtdrfbnabw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hfpthk.cn/gtgkptpyvw.html

[U68] PHP：PDO 连接
来源：http://hz.cashguo.top/gtkwfiqosv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.vqdsnc.cn/gtgahicbjx.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtyfazhsqm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuanzhike.top/gtqtiguduh.html

[U70] PHP：PDO 事务
来源：http://hz.cucudq.cn/gtfcxfbrfu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.c1oappe.top/gttpvhfyqy.html

[U71] PHP：抛出异常
来源：http://hz.daria6918.cn/gtryfkxhyj.html

throw new RuntimeException("失败", 500);
来源：http://hz.hnqzz.top/gtjkbsyrja.html

[U72] PHP：写错误日志
来源：http://hz.ywan-chungtsiang.top/gtznakjoii.html

error_log("失败: " . $e->getMessage());
来源：http://hz.iojbl.cn/gtykhainyz.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenzaomai.com/gtxbllsqbh.html

parse_ini_file("config.ini", true)
来源：http://hz.hywenlv.cn/gtdtttzopi.html

[U74] PHP：读取环境变量
来源：http://hz.havefunace.top/gtrrqymsud.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258888.top/gtopsdyzqk.html

[U75] PHP：依赖注入
来源：http://hz.havefunace.top/gtstoiuumb.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtdygnrmex.html

[U76] PHP：简单路由
来源：http://hz.jianghu66.top/gtyvkpyudv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dianchejie.cn/gtchiaohke.html

[U77] PHP：模板渲染
来源：http://hz.shanyushiyangtech.top/gttumpjteo.html

composer require twig/twig
来源：http://hz.zhoulong.xyz/gtsfsrwiao.html

[U78] PHP：单元测试
来源：http://hz.316326.xyz/gtkpqhvlrs.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtmzpogbct.html

[U79] PHP：静态分析
来源：http://hz.gzhubu.top/gtmfgnzcak.html

composer require --dev phpstan/phpstan
来源：http://hz.sysykeji.top/gthrhpntxa.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangkeji.top/gtfytkuzzc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinyuanbaomall.cn/gtikzvjjnf.html

[U81] JS：初始化项目
来源：http://hz.shangyingyoupin.top/gtvnhbpaao.html

npm init -y;  npm i express
来源：http://hz.zhixingplan.top/gtkkumqthv.html

[U82] JS：package.json 脚本
来源：http://hz.nanxuanxn.top/gtcilwygkn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sxryk.cn/gtyjmggqyr.html

[U83] JS：ES Module 导入导出
来源：http://hz.meibo888.top/gtbckduoka.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.snrcjt.cn/gtqvczfmad.html

[U84] JS：CommonJS 写法
来源：http://hz.ybcxt.top/gtguiecdvb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hfpthk.cn/gtsmgmzmml.html

[U85] JS：可选链
来源：http://hz.birdmap.top/gtdfrojgvn.html

a?.b?.c
来源：http://hz.feifeiyinyue.top/gtbfqedyae.html

[U86] JS：空值合并
来源：http://hz.0kj1m.cn/gtlngwehhb.html

a ?? b
来源：http://hz.hongshengwenyu.top/gtutrlqowd.html

[U87] JS：解构默认值
来源：http://hz.pengpengdd.cyou/gtwrqoratg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daria6918.cn/gtwdlejkik.html

[U88] JS：对象展开合并
来源：http://hz.hnqzz.top/gtrbacdmlq.html

{ ...a, ...b }
来源：http://hz.9152youxi.cn/gtsrthrmli.html

[U89] JS：数组去重
来源：http://hz.tanke756.top/gtopzjqdbm.html

[...new Set(arr)]
来源：http://hz.chenlongwang.top/gthvutrgie.html

[U90] JS：数字数组排序
来源：http://hz.chenzaomai.com/gtgbmaeczo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gttvgqwnqs.html

[U91] JS：对象键值遍历
来源：http://hz.ydzc1.top/gtqyuiylqs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtrbqpjcxw.html

[U92] JS：深拷贝
来源：http://hz.zhoulong.xyz/gtpmoqdjrs.html

structuredClone(obj)
来源：http://hz.316326.xyz/gtauhmtvod.html

[U93] JS：模板字符串
来源：http://hz.gaohongyu789.top/gtouaapopr.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gthcwuycxu.html

[U94] JS：箭头函数
来源：http://hz.iojbl.cn/gthknqekfb.html

const double = x => x * 2;
来源：http://hz.tianlin.xyz/gtcupphfcp.html

[U95] JS：Promise 包装
来源：http://hz.dianchejie.cn/gtccnunfeo.html

new Promise((resolve, reject) => {})
来源：http://hz.smart0.xyz/gtfinrtvls.html

[U96] JS：async/await 与异常
来源：http://hz.redwolf501.top/gtybjbvccc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtykxduasu.html

[U97] JS：并发请求
来源：http://hz.jianghu66.top/gtfpqgcrvh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtwxkcjguv.html

[U98] JS：fetch 带 JSON
来源：http://hz.ywan-chungtsiang.top/gthuvvvlts.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnxiangtu.top/gtwcboytbl.html

[U99] JS：事件监听
来源：http://hz.shangyingyoupin.top/gthvfyteqm.html

el.addEventListener("click", e => {})
来源：http://hz.cqqwz.cn/gtcqgogmcm.html

[U100] JS：DOM 查询
来源：http://hz.chenlongwang.top/gtwdwcsnrk.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gtvbbgmwvi.html

[U101] JS：classList 操作
来源：http://hz.snrcjt.cn/gtqbvpxjgx.html

el.classList.toggle("active")
来源：http://hz.yj20258888.top/gtvsseogfz.html

[U102] JS：本地存储
来源：http://hz.yueranfly.top/gtcmihnrzb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jlsjyb.cn/gtzunlfnaj.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gtcpvongwb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhoulong.xyz/gtwihvmnsu.html

[U104] JS：防抖
来源：http://hz.yj202588.top/gtihqfcmuv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gttuqybpqj.html

[U105] JS：节流
来源：http://hz.quarkkingdee.top/gtlxrqivel.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hongshengwenyu.top/gtdjlvtcec.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gttosbhsxo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zycfv.cn/gtmxododnj.html

[U107] JS：数字千分位
来源：http://hz.andypj.xyz/gthxcxiukz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ppjwa.cn/gtbsrehddq.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtjfycqjlf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aibaodan.cn/gtojdvhavt.html

[U109] JS：数组分组
来源：http://hz.yueranfly.top/gtflinlbec.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtmmcnnwhz.html

[U110] JS：数组分块
来源：http://hz.zhijiandao.cn/gtnsnjkemc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.birdmap.top/gtwsgvmzfa.html

[U111] JS：对象转 Map
来源：http://hz.wangdashe.top/gtozowaivf.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtqhijpihb.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangkeji.top/gtrbthknqh.html

"7".padStart(3, "0")
来源：http://hz.yongpay.top/gtfemvfdnv.html

[U113] JS：正则替换全部
来源：http://hz.daria6918.cn/gtyanmvfnr.html

s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtjfbgbdqj.html

[U114] JS：JSON 深比较
来源：http://hz.aibaodan.cn/gtisrdgrhv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gtidyworzz.html

[U115] JS：生成 UUID
来源：http://hz.nwbrower.top/gtthvxqlis.html

crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtijsgcjkc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.dianchejie.cn/gtoazxbeoh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yanxiufei.cn/gtykvxsuwh.html

[U117] JS：单元测试
来源：http://hz.ydzc1.top/gtnbmrjjmc.html

npm i -D vitest;  npx vitest
来源：http://hz.guowangkeji.top/gthywondco.html

[U118] JS：开发服务器
来源：http://hz.zycfv.cn/gtizhltjse.html

npm i -D vite;  npx vite
来源：http://hz.jqgfzy.top/gtkglqqfsx.html

[U119] JS：生产构建
来源：http://hz.yanxiufei.cn/gtuxfqkwjy.html

npx vite build
来源：http://hz.hongshengwenyu.top/gtpmtvrcav.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jianghu66.top/gtaydycbtx.html

import.meta.env.VITE_API_URL
来源：http://hz.tian-w.cn/gtmugievqo.html

================================================================================
来源：http://hz.chenlongwang.top/gtupexmkio.html

统计汇总
来源：http://hz.xinyue.icu/gtsfsuzwhf.html

================================================================================
来源：http://hz.snrcjt.cn/gtdndvkfpz.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtnxiplnmx.html

Python ......... 252
来源：http://hz.cucudq.cn/gtmxdylvhw.html

PHP ............ 252
来源：http://hz.xylfe.cn/gtwonifmly.html

JavaScript ..... 252
来源：http://hz.mhx1999.top/gtamdmydmo.html

TypeScript ..... 212
来源：http://hz.ybcxt.top/gtnalevbju.html

Java ........... 212
来源：http://hz.sysykeji.top/gtosyaxayh.html

Go ............. 212
来源：http://hz.hysaishi.cn/gtrezlbspl.html

Ruby ........... 212
来源：http://hz.cheryme.top/gtxompqrtx.html

C# ............. 212
来源：http://hz.zhengqikj.top/gtzzffurxd.html

C .............. 30
来源：http://hz.yj202588.top/gtcacvybya.html

C++ ............ 30
来源：http://hz.cucudq.cn/gtuudxwapy.html

SQL ............ 90
来源：http://hz.nwbrower.top/gtaoyywgdv.html

Bash ........... 80
来源：http://hz.jlsjyb.cn/gtxhklqpua.html

Kotlin ......... 15
来源：http://hz.wangdashe.top/gtwchhgrea.html

Swift .......... 15
来源：http://hz.shuidangran.top/gtkcftiszc.html

Lua ............ 10
来源：http://hz.hammf.cn/gtxupbtiqp.html

Perl ........... 10
来源：http://hz.ivvv.top/gtnwucpthu.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtirsqapcu.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtrclvxhpv.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gtzkacmfcm.html

按章节统计：
来源：http://hz.shanyushiyangtech.top/gtwknmxhlb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shanyushiyangkeji.top/gtpvuzzryz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtgdtuxoqz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shuidangran.top/gtmiuqioku.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gtftwidjuq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhaomingkeji.xyz/gtktghhzmt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gtxzounvel.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtwqdhbica.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtslulukqh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtyndejlys.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cheryme.top/gtfiuwlzsr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gterghmrwf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtcataahip.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtghxseogn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtxqdqcwan.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgufenzy.top/gtqglfmdop.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtsrwzaqnj.html

Q SQL 专题                              90
来源：http://hz.yj202588.top/gtehlblyfh.html

R Bash 专题                             80
来源：http://hz.yanxiufei.cn/gtvmckrsnq.html

S C / C++ 专题                          60
来源：http://hz.ivvv.top/gtklzyayrq.html

T 其他语言补充                          60
来源：http://hz.gogol.net.cn/gteydiulqx.html

U 高频实用片段                         120
来源：http://hz.yj20258888.top/gtdghygkeo.html

------------------------------------
来源：http://hz.chenzaomai.com/gtcbhgnhmq.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtgbkqhhhb.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtjkmfqogj.html

使用提醒
来源：http://hz.zhaomingkeji.xyz/gtfkwspgqv.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtjqvbdvvn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtlbasgpal.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangtech.top/gtxxjhjcfr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuanzx.com/gtnvjkiddg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gaohongyu789.top/gtlvtjqvci.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhijiandao.cn/gtionkttaj.html

—— 文件结束 ——
来源：http://hz.jianghu66.top/gtjsmafqeo.html

================================================================================
来源：http://hz.jqgfzy.top/gtpgnydaqb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtylvybmfq.html

Common Programming Examples Cheat Book
来源：http://hz.cucudq.cn/gtrgjpqvkk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtudpotbol.html

【收录内容】
来源：http://hz.pycfn.com/gtwslxhnxs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtkeqfekyw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yanxiufei.cn/gtxsupziah.html

SQL · Bash · C · C++
来源：http://hz.smart0.xyz/gtyzzlfeit.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtsejgnwtl.html

【使用说明】
来源：http://hz.yueranfly.top/gtsnpgfawe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhiwuduotai.top/gtfrwckose.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ybcxt.top/gtfutfebcs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ivvv.top/gtiuvlympi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hfpthk.cn/gtovmjavlr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.meibo888.top/gtyeqrnpnf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtgkmqactu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hongshengwenyu.top/gtetmppmkd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xingfuxueyuan.xyz/gtgpmdzpai.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shanyushiyangkeji.top/gtslbnlsmv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.nanxuanxn.top/gtxzhrepai.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.fengsongda.top/gtvqbftxdj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xingfuxueyuan.xyz/gtikhypoxa.html

【文件统计】
来源：http://hz.jqgufenzy.top/gtmzwwafnf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.iojbl.cn/gtujtezpba.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtrsudadno.html

目  录
来源：http://hz.xingfuxueyuan.xyz/gtteepcptn.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtgyrebnye.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.dianchejie.cn/gtybtsndtz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gtwjidzegp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtbximbrvn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangkeji.top/gtiochyybm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sufxvd.cn/gtggxedgby.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cucudq.cn/gtbwdwcboi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gthicogrjn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtdbtxupjo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtrmzjnnoc.html


<!-- 参考信息 -->