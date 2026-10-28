代发 wailian999

[U15] Py：高精度计时
来源：http://hz.tian-w.cn/gtkcycjueh.html

t = time.perf_counter()
来源：http://hz.gotoacloud.top/gtjdcqrsyd.html

[U16] Py：命令行参数解析
来源：http://hz.fzhhl.top/gtbxlectty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.iojbl.cn/gtdftmxhwj.html

[U17] Py：初始化日志
来源：http://hz.yongpay.top/gtzdrpkxym.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtseyzhurl.html

[U18] Py：预编译正则
来源：http://hz.gzhubu.top/gtzolffsos.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtlajzihlp.html

[U19] Py：正则替换带回调
来源：http://hz.hnqzz.top/gtwywnstbl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yuanzhike.top/gteyqjfare.html

[U20] Py：缓存函数结果
来源：http://hz.jinyuanbaomall.cn/gtjebusgkn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtdgbnshrv.html

[U21] Py：自定义上下文管理器
来源：http://hz.ppjwa.cn/gtoodvlutk.html

@contextlib.contextmanager
来源：http://hz.fengsongda.top/gtdzfqwknp.html

[U22] Py：矩阵转置
来源：http://hz.nanxuanxn.top/gtcbdolwxr.html

list(zip(*m))
来源：http://hz.jinyuanbaomall.cn/gtumsgdlmo.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtgekybvlw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuxming.cn/gtrdnrxumc.html

[U24] Py：路径操作
来源：http://hz.redwolf501.top/gtnfssogiy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtudmywkjn.html

[U25] Py：CSV 按字典读
来源：http://hz.zdqjudy.top/gtxbqnwreg.html

csv.DictReader(f)
来源：http://hz.wangshuangyany.cn/gtmfxsqhfv.html

[U26] Py：并发下载
来源：http://hz.cqqwz.cn/gtrsdasarq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yanxiufei.cn/gtxykdtaua.html

[U27] Py：异步 HTTP
来源：http://hz.aizwys.cn/gtlklvitcb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sysykeji.top/gtmrckkzyz.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtwoovgmmd.html

UserId = int
来源：http://hz.hongshengwenyu.top/gtnmkoxels.html

[U29] Py：属性校验
来源：http://hz.chenlongwang.top/gtvkhnhdbg.html

@property 与 @x.setter 配合
来源：http://hz.dashuyun.cn/gtdjgtprkb.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtmgnbscfc.html

@dataclass(slots=True)
来源：http://hz.chenjidiqi.icu/gtgyzhncgi.html

[U31] Py：单测
来源：http://hz.zhaomingkeji.xyz/gtrwndqtoe.html

python -m pytest -q
来源：http://hz.shanyushiyangtech.top/gthpesoowc.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gtmbwmcwkm.html

ruff format . && ruff check --fix .
来源：http://hz.birdmap.top/gtchwudezt.html

[U33] Py：打包发布
来源：http://hz.vqdsnc.cn/gtgmxgediq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fengsongda.top/gthrxpbdmb.html

[U34] Py：判断编码
来源：http://hz.jinqigufen.top/gtjxosrgrt.html

chardet.detect(raw)
来源：http://hz.vqdsnc.cn/gtoodqwdee.html

[U35] Py：发送邮件
来源：http://hz.ydzc1.top/gtjtkywsjz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nwbrower.top/gtsvqaispb.html

[U36] Py：定时任务
来源：http://hz.redwolf501.top/gtgvfftnfy.html

schedule.every(10).minutes.do(job)
来源：http://hz.jlsjyb.cn/gtitxkfzrj.html

[U37] Py：读写 Excel
来源：http://hz.hammf.cn/gtkwgkvreb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jyoumei.cn/gtgtrvvend.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtacikwenz.html

Path(__file__).resolve().parent
来源：http://hz.wangshuangyany.cn/gtswfckamt.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuetiantiany.cn/gtpptzcwqa.html

sys.stdout.isatty()
来源：http://hz.zhijiandao.cn/gtequeotdq.html

[U40] Py：打印到标准错误
来源：http://hz.aibaodan.cn/gtfyprdaaf.html

print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gthmlnqwor.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yueranfly.top/gtzjatbjbm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhaomingkeji.xyz/gtzelacfax.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ydjk.org.cn/gtoxvvyaui.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zycfv.cn/gtqepeenyw.html

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtifgyjtgs.html

namespace App\Http;
来源：http://hz.chenlongwang.top/gtresnadhw.html

[U44] PHP：开启严格类型
来源：http://hz.svipenyu.cn/gtrwamzhth.html

declare(strict_types=1);
来源：http://hz.cucudq.cn/gtiduoocjv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cqqwz.cn/gtrefeitnv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gteslnlcdo.html

[U46] PHP：可空类型
来源：http://hz.hnxiangtu.top/gtrjekzkwi.html

?string $name = null
来源：http://hz.iojbl.cn/gtmbwkuxog.html

[U47] PHP：联合类型
来源：http://hz.xingfuxueyuan.xyz/gtaneeljcz.html

int|string $id
来源：http://hz.xuanzx.com/gtggnubtpm.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gteonaixtr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydjk.org.cn/gtfjtiosbt.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gtjerpxwom.html

public readonly string $name
来源：http://hz.jinghuilouyu.cn/gtejlesgbc.html

[U50] PHP：构造器属性提升
来源：http://hz.yvedp.cn/gtdgozjjce.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gtjnmoylac.html

[U51] PHP：数组解构
来源：http://hz.chenzaomai.com/gtfzzwqley.html

[$a, $b] = $arr;
来源：http://hz.shuidangran.top/gtvnfrlqmk.html

[U52] PHP：箭头函数
来源：http://hz.ybcxt.top/gtojmwqhdu.html

$double = fn($x) => $x * 2;
来源：http://hz.ydzc1.top/gtiehyxxrk.html

[U53] PHP：空合并运算符
来源：http://hz.guowangkeji.top/gtuaaujyih.html

$v = $a ?? $b ?? "default";
来源：http://hz.snrcjt.cn/gtcnydhyli.html

[U54] PHP：空安全调用
来源：http://hz.fzhhl.top/gtxyznxjmi.html

$obj?->method()
来源：http://hz.gaohongyu789.top/gtfghgavuv.html

[U55] PHP：match 表达式
来源：http://hz.wangdashe.top/gtkdanzppm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.kuanghao11.cn/gtieyxdapt.html

[U56] PHP：命名参数
来源：http://hz.fengsongda.top/gtsjcjsfct.html

f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gttegrxdwu.html

[U57] PHP：字符串插值
来源：http://hz.shuidangran.top/gtzxsamxtx.html

"值: {$a}"
来源：http://hz.dianchejie.cn/gtmimsqrco.html

[U58] PHP：数组三件套
来源：http://hz.52xcode.cn/gtfhzkpwmg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtgcgpkrch.html

[U59] PHP：自定义排序
来源：http://hz.hywenlv.cn/gtjwxhiqrg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gtfzzlgxeq.html

[U60] PHP：JSON 编解码
来源：http://hz.9152youxi.cn/gtnbpszkka.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hfpthk.cn/gtdybntdlf.html

[U61] PHP：正则
来源：http://hz.cucudq.cn/gtealetimz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtfcnzokxm.html

[U62] PHP：日期对象
来源：http://hz.ybcxt.top/gtixniqxdh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.vqdsnc.cn/gtavbwozam.html

[U63] PHP：文件读写
来源：http://hz.sxryk.cn/gttuzpymjr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hysaishi.cn/gtggzxxjta.html

[U64] PHP：目录遍历
来源：http://hz.shuidangran.top/gthezxgwsa.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj202588.top/gtrmaweueh.html

[U65] PHP：会话
来源：http://hz.iojbl.cn/gtkhapfkqk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dianchejie.cn/gtzwkjvfze.html

[U66] PHP：设置 Cookie
来源：http://hz.hnxiangtu.top/gtavjzinsx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cashguo.top/gtyxeqbctq.html

[U67] PHP：处理文件上传
来源：http://hz.feifeiyinyue.top/gtxborugck.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.daxiang520.top/gtortrqdsu.html

[U68] PHP：PDO 连接
来源：http://hz.xziqi.cn/gtyxvifyoy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangkeji.top/gtcgtutgyk.html

[U69] PHP：PDO 预处理
来源：http://hz.hongshengwenyu.top/gtevgxoerv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtyusftwif.html

[U70] PHP：PDO 事务
来源：http://hz.andypj.xyz/gtfdwhlipl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.fengsongda.top/gtpetrrbgp.html

[U71] PHP：抛出异常
来源：http://hz.zycfv.cn/gtgnndugif.html

throw new RuntimeException("失败", 500);
来源：http://hz.ppjwa.cn/gtxtqlqdvd.html

[U72] PHP：写错误日志
来源：http://hz.sufxvd.cn/gtxzxvkvnr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ybcxt.top/gtwrgsavtx.html

[U73] PHP：读取 ini 配置
来源：http://hz.gotoacloud.top/gtnlejdkkz.html

parse_ini_file("config.ini", true)
来源：http://hz.wangshuangyany.cn/gtikkhnpge.html

[U74] PHP：读取环境变量
来源：http://hz.nwbrower.top/gtrtnabixo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.havefunace.top/gtgqcgljgh.html

[U75] PHP：依赖注入
来源：http://hz.jinghuilouyu.cn/gtvvnwqybe.html

composer require psr/container
来源：http://hz.shanyushiyangtech.top/gtobwblddj.html

[U76] PHP：简单路由
来源：http://hz.hnqzz.top/gtgcdmvclp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shangyingyoupin.top/gtfvrmzsli.html

[U77] PHP：模板渲染
来源：http://hz.quarkkingdee.top/gtmqrcpgjj.html

composer require twig/twig
来源：http://hz.chenjidiqi.icu/gtpcwjircq.html

[U78] PHP：单元测试
来源：http://hz.svipenyu.cn/gtsalvudco.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtegaykhha.html

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtpeyjgrln.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gtcdeozths.html

[U80] PHP：代码规范修复
来源：http://hz.yj202588.top/gtbmtxbrzg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhiwuduotai.top/gtmloxrtgm.html

[U81] JS：初始化项目
来源：http://hz.bjfxy.top/gtnjzepwxy.html

npm init -y;  npm i express
来源：http://hz.hnxiangtu.top/gtdnceezwv.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtxxbswjhg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ehwqpu.com/gtjbrspaqo.html

[U83] JS：ES Module 导入导出
来源：http://hz.yonumen.top/gtsawgukzu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ivvv.top/gtshulgaeg.html

[U84] JS：CommonJS 写法
来源：http://hz.zhijiandao.cn/gtprffdrlp.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenlongwang.top/gtldkfefdb.html

[U85] JS：可选链
来源：http://hz.fengsongda.top/gtxnmcqrux.html

a?.b?.c
来源：http://hz.smart0.xyz/gtammqgfxv.html

[U86] JS：空值合并
来源：http://hz.quarkkingdee.top/gtiydrzzhf.html

a ?? b
来源：http://hz.yonumen.top/gtkfrarbkx.html

[U87] JS：解构默认值
来源：http://hz.xylfe.cn/gteoxccnpk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tanke756.top/gtofdxuczz.html

[U88] JS：对象展开合并
来源：http://hz.hammf.cn/gtncvjopbg.html

{ ...a, ...b }
来源：http://hz.tianlin.xyz/gtxdxxfmkl.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gtlcykgldj.html

[...new Set(arr)]
来源：http://hz.daria6918.cn/gtrewcdmom.html

[U90] JS：数字数组排序
来源：http://hz.tian-w.cn/gtwlhvjtnd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtkrgduext.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtvjpffuqu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shzxlz.cn/gtntplemvw.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtkcrdqdoh.html

structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtqkheysvf.html

[U93] JS：模板字符串
来源：http://hz.jiagoushi.top/gtiarntcsw.html

`共 ${n} 条`
来源：http://hz.pycfn.com/gttapymzoe.html

[U94] JS：箭头函数
来源：http://hz.shuidangran.top/gtwjeuiueq.html

const double = x => x * 2;
来源：http://hz.gaohongyu789.top/gtxabrawck.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtizeyucxq.html

new Promise((resolve, reject) => {})
来源：http://hz.dashuyun.cn/gtlspzkgqt.html

[U96] JS：async/await 与异常
来源：http://hz.daxiang520.top/gtebsvnwia.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtplbqtmas.html

[U97] JS：并发请求
来源：http://hz.xylfe.cn/gttgcwcswd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtojnmqoni.html

[U98] JS：fetch 带 JSON
来源：http://hz.sysykeji.top/gtltsvfpij.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sxryk.cn/gttnjppspk.html

[U99] JS：事件监听
来源：http://hz.52xcode.cn/gtekopisxs.html

el.addEventListener("click", e => {})
来源：http://hz.yonumen.top/gtpzypgikk.html

[U100] JS：DOM 查询
来源：http://hz.yj202588.top/gtilzaglbl.html

document.querySelector(".item")
来源：http://hz.chenlongwang.top/gtperxujvy.html

[U101] JS：classList 操作
来源：http://hz.hysaishi.cn/gtffqyuzxz.html

el.classList.toggle("active")
来源：http://hz.hysaishi.cn/gtmcoyrgbf.html

[U102] JS：本地存储
来源：http://hz.nwbrower.top/gtvwaajscl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gzhubu.top/gtsdrbzdie.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gtnswciwnp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.pycfn.com/gtupqnbtjq.html

[U104] JS：防抖
来源：http://hz.ehwqpu.com/gtwhchhjwo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtmmbgejlh.html

[U105] JS：节流
来源：http://hz.cucudq.cn/gtnqvzbcoy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jiagoushi.top/gttbbukelp.html

[U106] JS：日期格式化
来源：http://hz.jinqigfzy.top/gtuokamoiv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.redwolf501.top/gtldkxnrtd.html

[U107] JS：数字千分位
来源：http://hz.meibo888.top/gttjyxmnwp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhijiandao.cn/gtsqanlmhz.html

[U108] JS：随机整数
来源：http://hz.haohaochexian.top/gtlprutbpg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.chenjidiqi.icu/gtsrjklxrx.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtcaospwxa.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtzbgzbhpl.html

[U110] JS：数组分块
来源：http://hz.cashguo.top/gtxdvhadnb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtyixgsmej.html

[U111] JS：对象转 Map
来源：http://hz.bjfxy.top/gtyahvfvrq.html

new Map(Object.entries(obj))
来源：http://hz.jlsjyb.cn/gtkvtxnubk.html

[U112] JS：字符串补位
来源：http://hz.sxryk.cn/gtukbxdrpa.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtliumcqqr.html

[U113] JS：正则替换全部
来源：http://hz.dashuyun.cn/gtdzcpxxcq.html

s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtrxnnbgtf.html

[U114] JS：JSON 深比较
来源：http://hz.yongpay.top/gtlohaquhs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtjisruadc.html

[U115] JS：生成 UUID
来源：http://hz.jiagoushi.top/gtgmbevikm.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtbbxrfdom.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sysykeji.top/gtjswttmxr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jianghu66.top/gtvtprbjyd.html

[U117] JS：单元测试
来源：http://hz.ywan-chungtsiang.top/gtmqnxqojy.html

npm i -D vitest;  npx vitest
来源：http://hz.yvedp.cn/gtgaedgfjz.html

[U118] JS：开发服务器
来源：http://hz.52xcode.cn/gtmowhrpxl.html

npm i -D vite;  npx vite
来源：http://hz.daria6918.cn/gthnomtpzy.html

[U119] JS：生产构建
来源：http://hz.nwbrower.top/gtckraxcve.html

npx vite build
来源：http://hz.haohaochexian.top/gtvvjbntmm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hywenlv.cn/gtjbgmxhbd.html

import.meta.env.VITE_API_URL
来源：http://hz.9152youxi.cn/gtibfbsoho.html

================================================================================
来源：http://hz.zycfv.cn/gteucoubpy.html

统计汇总
来源：http://hz.gogol.net.cn/gtzxowkqsl.html

================================================================================
来源：http://hz.mhx1999.top/gthgrabhvt.html

按语言统计（条）：
来源：http://hz.tanke756.top/gtbtpzdlzf.html

Python ......... 252
来源：http://hz.jinqigfzy.top/gtlplwfsfk.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtxbmnboyk.html

JavaScript ..... 252
来源：http://hz.wangshuangyany.cn/gtgjbfphnv.html

TypeScript ..... 212
来源：http://hz.xuanzx.com/gthunuzyob.html

Java ........... 212
来源：http://hz.zycfv.cn/gtzlvyhmaq.html

Go ............. 212
来源：http://hz.tianlin.xyz/gttuuhnbtl.html

Ruby ........... 212
来源：http://hz.xylfe.cn/gtcccawhkp.html

C# ............. 212
来源：http://hz.zdqjudy.top/gtzussrmtn.html

C .............. 30
来源：http://hz.chenlongwang.top/gtzgfobpaz.html

C++ ............ 30
来源：http://hz.feifeiyinyue.top/gtkgdrsvot.html

SQL ............ 90
来源：http://hz.yuxming.cn/gtjjrwxjhr.html

Bash ........... 80
来源：http://hz.jinyuanbaomall.cn/gtsmplhuzj.html

Kotlin ......... 15
来源：http://hz.jiagoushi.top/gtxrxdcwqi.html

Swift .......... 15
来源：http://hz.jinqigfzy.top/gtvonndvjk.html

Lua ............ 10
来源：http://hz.yj20258888.top/gtqqxwfoev.html

Perl ........... 10
来源：http://hz.ehwqpu.com/gtpxewgszx.html

Scala .......... 10
来源：http://hz.c1oappe.top/gteufqgvbb.html

------------------------------------
来源：http://hz.ywan-chungtsiang.top/gthkrapigo.html

合计 ........... 2106 条
来源：http://hz.cqqwz.cn/gtmplelzkg.html

按章节统计：
来源：http://hz.aibaodan.cn/gtmletvffu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xylfe.cn/gtfpomudsy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtzknconnv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtnjxhlfya.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hywenlv.cn/gtfpoutfvq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.andypj.xyz/gtjiovyplp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtlddfolct.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtqadzsfgm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.meibo888.top/gtwjqlnjvi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtqhpsgfet.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtajkbgvdq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtffhusrhj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtucozaibf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtctksiiwy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhongyouzk.top/gtmnxgdyfy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xingfuxueyuan.xyz/gtwjcvnbub.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtnmwrpqpd.html

Q SQL 专题                              90
来源：http://hz.xziqi.cn/gttobrtglq.html

R Bash 专题                             80
来源：http://hz.shangyingyoupin.top/gtwwdzdimh.html

S C / C++ 专题                          60
来源：http://hz.jqgfzy.top/gtthnqsrgu.html

T 其他语言补充                          60
来源：http://hz.sxryk.cn/gtccbbmwft.html

U 高频实用片段                         120
来源：http://hz.svipenyu.cn/gtvgoperqk.html

------------------------------------
来源：http://hz.dashuyun.cn/gtdjmlpyri.html

合计                                  2106 条
来源：http://hz.dashuyun.cn/gtjmhslzjl.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtokqulrqr.html

使用提醒
来源：http://hz.hnxiangtu.top/gttimvulmv.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtzuzqbpgn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.birdmap.top/gtqsnkkbnf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tian-w.cn/gtkotbbwgu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnqzz.top/gtgcrptwmx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxinkj.top/gturtjbtor.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xylfe.cn/gtoknuygzs.html

—— 文件结束 ——
来源：http://hz.zycfv.cn/gthejqmspz.html

================================================================================
来源：http://hz.cucudq.cn/gtwgpgrfdw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xinyue.icu/gtasqkcxtj.html

Common Programming Examples Cheat Book
来源：http://hz.andypj.xyz/gtimhfrmuo.html

================================================================================
来源：http://hz.zycfv.cn/gtgcskxqog.html

【收录内容】
来源：http://hz.wangdashe.top/gtfwsiaulk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenzaomai.com/gtjxknkong.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yangfankeji.com/gtldldyvhs.html

SQL · Bash · C · C++
来源：http://hz.haohaochexian.top/gtanyfegzs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.feifeiyinyue.top/gtoazroclu.html

【使用说明】
来源：http://hz.zhixingplan.top/gthwddgegb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.tanke756.top/gtdauetxca.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.c1oappe.top/gtdoqwdigo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jlsjyb.cn/gttdwldgds.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.birdmap.top/gtgvxnerdi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xuanzx.com/gtmvkzutio.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sufxvd.cn/gtozqcmrhk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.aibaodan.cn/gtvilychse.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhiwuduotai.top/gtkysqblzz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cucudq.cn/gtzjxtuhqx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.snrcjt.cn/gtbwcqccit.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.wangdashe.top/gtygmpnsif.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgfzy.top/gteclfhogg.html

【文件统计】
来源：http://hz.vqdsnc.cn/gtangoklwp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.meibo888.top/gtdcxwdcxv.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtmivyyknx.html

目  录
来源：http://hz.316326.xyz/gtpsnlzykn.html

--------------------------------------------------------------------------------
来源：http://hz.xuetiantiany.cn/gtakgtoild.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gtjajitjwv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtigbywmck.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtzhzwrqyx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtxasduokd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgufenzy.top/gtwqztzcbr.html


<!-- 参考信息 -->