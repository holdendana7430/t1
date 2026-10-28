代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.feifeiyinyue.top/gtngjjoysm.html

[T57] Scala：模式匹配
来源：http://hz.hammf.cn/gtmtyebadm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daria6918.cn/gthltizlsx.html

[T58] Scala：函数定义
来源：http://hz.havefunace.top/gttygvuhnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jianghu66.top/gtsfabcowm.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtupyemkqp.html

for (i <- 1 to 10) println(i)
来源：http://hz.xylfe.cn/gtrcwikdgj.html

[T60] Scala：折叠
来源：http://hz.shuidangran.top/gtbuyrwchz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daxiang520.top/gtritwxzmg.html

================================================================================
来源：http://hz.haohaochexian.top/gtqjmhshgg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.bjfxy.top/gtggdsawdf.html

================================================================================
来源：http://hz.guannengcc.top/gtbveyqity.html

[U01] Py：创建虚拟环境
来源：http://hz.cqqwz.cn/gtihawzssl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnqzz.top/gtmsxdrbtg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hysaishi.cn/gtvigaeepa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sysykeji.top/gtmyeakyzg.html

[U03] Py：加载 .env 配置
来源：http://hz.ehwqpu.com/gtatdxgqws.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.haohaochexian.top/gtrwhgjtza.html

[U04] Py：变量调试打印
来源：http://hz.havefunace.top/gtfqwrmkec.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangkeji.top/gtpaimhghy.html

[U05] Py：列表去重且保序
来源：http://hz.bjfxy.top/gthljjtaft.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtpjtfbzuj.html

[U06] Py：合并两个字典
来源：http://hz.guowangkeji.top/gtfqchldel.html

{**a, **b}
来源：http://hz.nanxuanxn.top/gtqywncetk.html

[U07] Py：反转字典键值
来源：http://hz.ybcxt.top/gtdtsrmdta.html

{v: k for k, v in d.items()}
来源：http://hz.gaohongyu789.top/gtpaofuihd.html

[U08] Py：展平二维列表
来源：http://hz.xinyue.icu/gtgpmweijd.html

[y for x in nested for y in x]
来源：http://hz.shuidangran.top/gtoccynxhs.html

[U09] Py：字典取最大值的键
来源：http://hz.jianghu66.top/gtzzywrwsa.html

max(d, key=d.get)
来源：http://hz.daxiang520.top/gtcprshhdz.html

[U10] Py：按值排序字典
来源：http://hz.nanxuanxn.top/gtdzdbfron.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtmwryjpyz.html

[U11] Py：生成器表达式
来源：http://hz.jqgfzy.top/gtecdnzwif.html

(x * 2 for x in arr)
来源：http://hz.tian-w.cn/gtgcssabbu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.smart0.xyz/gtvhmslabe.html

Counter(arr).most_common(3)
来源：http://hz.gzhubu.top/gtiobcggvm.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtxsbowybv.html

deque(maxlen=10)
来源：http://hz.mhx1999.top/gtkjylhxdy.html

[U14] Py：分组收集到列表
来源：http://hz.xuanzx.com/gthdcogqgd.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtsveltyzk.html

[U15] Py：高精度计时
来源：http://hz.zycfv.cn/gteqgfkrqs.html

t = time.perf_counter()
来源：http://hz.9152youxi.cn/gtjjgfdqyy.html

[U16] Py：命令行参数解析
来源：http://hz.tian-w.cn/gtyccsdflw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtibwyumtt.html

[U17] Py：初始化日志
来源：http://hz.jiagoushi.top/gtbxiqigyk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhoulong.xyz/gtnodrfrox.html

[U18] Py：预编译正则
来源：http://hz.cheryme.top/gtbbmgigwo.html

pat = re.compile(r"\d+")
来源：http://hz.gaohongyu789.top/gtiuzfnktu.html

[U19] Py：正则替换带回调
来源：http://hz.shangyingyoupin.top/gtbdnbjgnu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gtypeumgiy.html

[U20] Py：缓存函数结果
来源：http://hz.hnxiangtu.top/gtdewetgdd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dashuyun.cn/gtpkafeusb.html

[U21] Py：自定义上下文管理器
来源：http://hz.feifeiyinyue.top/gtfcufceic.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangkeji.top/gtudgwhoju.html

[U22] Py：矩阵转置
来源：http://hz.zhongyouzk.top/gtwglimtrn.html

list(zip(*m))
来源：http://hz.xinyue.icu/gtuspnrsqd.html

[U23] Py：分块读取大文件
来源：http://hz.smart0.xyz/gtsxifmngh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.vqdsnc.cn/gtbbrooyde.html

[U24] Py：路径操作
来源：http://hz.svipenyu.cn/gtgtodvkam.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hysaishi.cn/gttngnclpa.html

[U25] Py：CSV 按字典读
来源：http://hz.gzhubu.top/gtbgkdvaul.html

csv.DictReader(f)
来源：http://hz.316326.xyz/gtoikpbcpv.html

[U26] Py：并发下载
来源：http://hz.jlsjyb.cn/gtatekymjq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinghuilouyu.cn/gtunaccaqh.html

[U27] Py：异步 HTTP
来源：http://hz.aizwys.cn/gtjtazbvgj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenzaomai.com/gthshramrr.html

[U28] Py：类型别名
来源：http://hz.aibaodan.cn/gtonxlxgpo.html

UserId = int
来源：http://hz.tanke756.top/gtrpkzupbd.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtjzmszlzy.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtqbhzipez.html

[U30] Py：数据类
来源：http://hz.jqgfzy.top/gtpgzktzme.html

@dataclass(slots=True)
来源：http://hz.0kj1m.cn/gtsthjggfe.html

[U31] Py：单测
来源：http://hz.jinyuanbaomall.cn/gtmcnqelmf.html

python -m pytest -q
来源：http://hz.ehwqpu.com/gtcdnojitq.html

[U32] Py：代码格式化
来源：http://hz.yangfankeji.com/gtfmoraiop.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtcevivtvw.html

[U33] Py：打包发布
来源：http://hz.ydzc1.top/gttxxgnvbs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuanzhike.top/gttloocojz.html

[U34] Py：判断编码
来源：http://hz.c1oappe.top/gtmksmkwaf.html

chardet.detect(raw)
来源：http://hz.jinqigufen.top/gtvtmqioqv.html

[U35] Py：发送邮件
来源：http://hz.jianghu66.top/gtfxafsqav.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.mhx1999.top/gttxtwwbpj.html

[U36] Py：定时任务
来源：http://hz.yueranfly.top/gtjklbwehc.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinqigfzy.top/gtwtqrnvpn.html

[U37] Py：读写 Excel
来源：http://hz.zdqjudy.top/gthvrqwdse.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangdashe.top/gtpvtesjho.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gtzvnwerck.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gthnllwhft.html

[U39] Py：判断是否在交互环境
来源：http://hz.sysykeji.top/gtsicexofy.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtlwxqzqcm.html

[U40] Py：打印到标准错误
来源：http://hz.xuanzx.com/gtkzdewgns.html

print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gttdtvsgni.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hfpthk.cn/gtmncvpmca.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shuidangran.top/gteyfmavps.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.nwbrower.top/gtxbkcgymk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgufenzy.top/gtaqyeifha.html

[U43] PHP：声明命名空间
来源：http://hz.52xcode.cn/gttbdkckpe.html

namespace App\Http;
来源：http://hz.yangfankeji.com/gtmwxwvmlz.html

[U44] PHP：开启严格类型
来源：http://hz.gzhubu.top/gtofgnzkrv.html

declare(strict_types=1);
来源：http://hz.tian-w.cn/gtmdcnhbdn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gogol.net.cn/gtoshepavk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtgtmlrmmj.html

[U46] PHP：可空类型
来源：http://hz.hongshengwenyu.top/gtsefqdbfb.html

?string $name = null
来源：http://hz.fzhhl.top/gtblnphozg.html

[U47] PHP：联合类型
来源：http://hz.jinqigufen.top/gtljfqguen.html

int|string $id
来源：http://hz.tian-w.cn/gtwkhvlfzk.html

[U48] PHP：纯枚举
来源：http://hz.sxryk.cn/gtivfdwcwj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuetiantiany.cn/gtypkbjohv.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtzzqvypfa.html

public readonly string $name
来源：http://hz.xuanzx.com/gtqguxwetm.html

[U50] PHP：构造器属性提升
来源：http://hz.shanyushiyangtech.top/gtdhlzvlnc.html

public function __construct(private int $id) {}
来源：http://hz.vqdsnc.cn/gtgihbsmuz.html

[U51] PHP：数组解构
来源：http://hz.haohaochexian.top/gtapxrmigf.html

[$a, $b] = $arr;
来源：http://hz.haohaochexian.top/gtshhosner.html

[U52] PHP：箭头函数
来源：http://hz.xuetiantiany.cn/gtmfofdvcl.html

$double = fn($x) => $x * 2;
来源：http://hz.pengpengdd.cyou/gtskjupggd.html

[U53] PHP：空合并运算符
来源：http://hz.nwbrower.top/gtjdwvlwed.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydzc1.top/gtymtngsui.html

[U54] PHP：空安全调用
来源：http://hz.jlsjyb.cn/gtrgpcnzsm.html

$obj?->method()
来源：http://hz.gotoacloud.top/gtvyoclier.html

[U55] PHP：match 表达式
来源：http://hz.hnxiangtu.top/gtbulrxkzu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.9152youxi.cn/gtargzjqip.html

[U56] PHP：命名参数
来源：http://hz.shuidangran.top/gtsfhnvsrg.html

f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtvjmgtfrm.html

[U57] PHP：字符串插值
来源：http://hz.jqgfzy.top/gtfzlpmowb.html

"值: {$a}"
来源：http://hz.ydzc1.top/gtsysleywe.html

[U58] PHP：数组三件套
来源：http://hz.yueranfly.top/gtzdoawzrb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtebwinrxh.html

[U59] PHP：自定义排序
来源：http://hz.wangshuangyany.cn/gtjcspysag.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhijiandao.cn/gtbzceezhy.html

[U60] PHP：JSON 编解码
来源：http://hz.tanke756.top/gtenesfmvq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtiuolcnsv.html

[U61] PHP：正则
来源：http://hz.aizwys.cn/gtdxnmdqbo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtfaksrfic.html

[U62] PHP：日期对象
来源：http://hz.guowangkeji.top/gtrkzlaxlv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxinkj.top/gtyyxenaun.html

[U63] PHP：文件读写
来源：http://hz.jqgfzy.top/gtgoiuahlq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cucudq.cn/gtcamiocwg.html

[U64] PHP：目录遍历
来源：http://hz.52xcode.cn/gtgerkfscx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydzc1.top/gtmyqtvvqo.html

[U65] PHP：会话
来源：http://hz.hfpthk.cn/gtexwgflgm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yueranfly.top/gtxzxrcjbg.html

[U66] PHP：设置 Cookie
来源：http://hz.gzhubu.top/gtszxzltfg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zdqjudy.top/gtgossihni.html

[U67] PHP：处理文件上传
来源：http://hz.dianchejie.cn/gtmvwynfcc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xylfe.cn/gtbdfkaslp.html

[U68] PHP：PDO 连接
来源：http://hz.xingfuxueyuan.xyz/gtehcqdwmw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.316326.xyz/gtovykebwg.html

[U69] PHP：PDO 预处理
来源：http://hz.ppjwa.cn/gtooqmvlzi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.kuanghao11.cn/gtwruipexb.html

[U70] PHP：PDO 事务
来源：http://hz.xziqi.cn/gtnoculjmd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sweek.top/gtanhsseot.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtvplxrfbo.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gtnaaurdhb.html

[U72] PHP：写错误日志
来源：http://hz.ehwqpu.com/gtvhsizmcb.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nwbrower.top/gtucuaighc.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenjidiqi.icu/gtevkxvofc.html

parse_ini_file("config.ini", true)
来源：http://hz.ydjk.org.cn/gtzqphyndm.html

[U74] PHP：读取环境变量
来源：http://hz.zhijiandao.cn/gtuxgztooe.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daria6918.cn/gtqqpmlasx.html

[U75] PHP：依赖注入
来源：http://hz.snrcjt.cn/gthuofuhpg.html

composer require psr/container
来源：http://hz.shanyushiyangtech.top/gtzczjwqru.html

[U76] PHP：简单路由
来源：http://hz.jinqigufen.top/gtqqkadhqc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj20258.top/gtkranqwwa.html

[U77] PHP：模板渲染
来源：http://hz.xingfuxueyuan.xyz/gtujabvric.html

composer require twig/twig
来源：http://hz.xingfuxueyuan.xyz/gtgxjizcpi.html

[U78] PHP：单元测试
来源：http://hz.fzhhl.top/gtbbwnantd.html

composer require --dev phpunit/phpunit
来源：http://hz.zdqjudy.top/gtoaooowjb.html

[U79] PHP：静态分析
来源：http://hz.jlsjyb.cn/gtyjzmduxo.html

composer require --dev phpstan/phpstan
来源：http://hz.jqgfzy.top/gtxwsakodc.html

[U80] PHP：代码规范修复
来源：http://hz.jqgufenzy.top/gtmkeexkdw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sxryk.cn/gtobuttpnd.html

[U81] JS：初始化项目
来源：http://hz.pycfn.com/gtmnpqozam.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtzobvfzmb.html

[U82] JS：package.json 脚本
来源：http://hz.jiagoushi.top/gteogjkeqv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ydjk.org.cn/gtjcaagoma.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhijiandao.cn/gtvytjjokl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.iojbl.cn/gtaanykrgd.html

[U84] JS：CommonJS 写法
来源：http://hz.ivvv.top/gttltqxwni.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.c1oappe.top/gtzfliedcx.html

[U85] JS：可选链
来源：http://hz.sysykeji.top/gtausbcouk.html

a?.b?.c
来源：http://hz.jlsjyb.cn/gtadlhvjka.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtpknklqmu.html

a ?? b
来源：http://hz.yj20258.top/gtuvahnjue.html

[U87] JS：解构默认值
来源：http://hz.ybcxt.top/gtlbdwzueb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.iojbl.cn/gtfainwgtk.html

[U88] JS：对象展开合并
来源：http://hz.tanke756.top/gtjtwdlbxr.html

{ ...a, ...b }
来源：http://hz.nanxuanxn.top/gtrizmgprr.html

[U89] JS：数组去重
来源：http://hz.zdqjudy.top/gtrawsncgw.html

[...new Set(arr)]
来源：http://hz.nanxinkj.top/gtbawlkmae.html

[U90] JS：数字数组排序
来源：http://hz.wangshuangyany.cn/gttkzspgma.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtisewiydv.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangkeji.top/gtgkwjbndq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jyoumei.cn/gtswqkgduy.html

[U92] JS：深拷贝
来源：http://hz.zhijiandao.cn/gtgamjskrb.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gtkflwzvje.html

[U93] JS：模板字符串
来源：http://hz.shangyingyoupin.top/gtsstwucsu.html

`共 ${n} 条`
来源：http://hz.hywenlv.cn/gtdleftuyw.html

[U94] JS：箭头函数
来源：http://hz.yj20258.top/gtpotpvwpt.html

const double = x => x * 2;
来源：http://hz.cheryme.top/gtskdrcggu.html

[U95] JS：Promise 包装
来源：http://hz.jianghu66.top/gtzoaktlna.html

new Promise((resolve, reject) => {})
来源：http://hz.pengpengdd.cyou/gtugxhgmtk.html

[U96] JS：async/await 与异常
来源：http://hz.birdmap.top/gtauccdgui.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtcpofeepd.html

[U97] JS：并发请求
来源：http://hz.52xcode.cn/gtnzbxcmld.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtvztldogh.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangdashe.top/gtfvtgsmgq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xziqi.cn/gtdmjamosb.html

[U99] JS：事件监听
来源：http://hz.tian-w.cn/gttlrufmbm.html

el.addEventListener("click", e => {})
来源：http://hz.yuanzhike.top/gtptalppag.html

[U100] JS：DOM 查询
来源：http://hz.feifeiyinyue.top/gtvmdyoexp.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gtrnoxrpwu.html

[U101] JS：classList 操作
来源：http://hz.yuxming.cn/gtztfdxzxr.html

el.classList.toggle("active")
来源：http://hz.daria6918.cn/gtwyxrzlxe.html

[U102] JS：本地存储
来源：http://hz.yj202588.top/gtyilmadhb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jiagoushi.top/gtjfpakvbv.html

[U103] JS：定时器
来源：http://hz.chenzaomai.com/gtnatlkejp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yanxiufei.cn/gtyxgucrkb.html

[U104] JS：防抖
来源：http://hz.shzxlz.cn/gthjkronku.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gthgjlyszc.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtdqwyenfc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.redwolf501.top/gtibastcee.html

[U106] JS：日期格式化
来源：http://hz.cashguo.top/gthzzyggoz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cqqwz.cn/gtwhkjpqml.html

[U107] JS：数字千分位
来源：http://hz.haohaochexian.top/gtumtntnie.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jlsjyb.cn/gtiekikcst.html

[U108] JS：随机整数
来源：http://hz.c1oappe.top/gthkegwvtd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fzhhl.top/gtnhmfnavb.html

[U109] JS：数组分组
来源：http://hz.nanxuanxn.top/gtmnmllkmz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtpdfcmdgg.html

[U110] JS：数组分块
来源：http://hz.iojbl.cn/gtgzlugtti.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gtvkrhwhkw.html

[U111] JS：对象转 Map
来源：http://hz.smart0.xyz/gtkgfjjxdh.html

new Map(Object.entries(obj))
来源：http://hz.zhijiandao.cn/gtaixekqvo.html

[U112] JS：字符串补位
来源：http://hz.bjfxy.top/gtpknzkgcb.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtdcgqbcwp.html

[U113] JS：正则替换全部
来源：http://hz.ybcxt.top/gtwtkupznu.html

s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtguqyvvhu.html

[U114] JS：JSON 深比较
来源：http://hz.bjfxy.top/gtdgllkwss.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtjvoiklfq.html

[U115] JS：生成 UUID
来源：http://hz.feifeiyinyue.top/gtruqbelpv.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtxrlxhkeu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.fengsongda.top/gtuybykotd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cucudq.cn/gtesddvvuq.html

[U117] JS：单元测试
来源：http://hz.jqgfzy.top/gtfuvlehns.html

npm i -D vitest;  npx vitest
来源：http://hz.svipenyu.cn/gtvaafxzwx.html

[U118] JS：开发服务器
来源：http://hz.0kj1m.cn/gthqmnqaws.html

npm i -D vite;  npx vite
来源：http://hz.haohaochexian.top/gtmmdovchn.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtjtqapzfa.html

npx vite build
来源：http://hz.wangshuangyany.cn/gtgtgkvcze.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuxming.cn/gtoenvlybi.html

import.meta.env.VITE_API_URL
来源：http://hz.yonumen.top/gtgdiiqkpl.html

================================================================================
来源：http://hz.daxiang520.top/gtdaxtzjcv.html

统计汇总
来源：http://hz.yj202588.top/gtnomgbtok.html

================================================================================
来源：http://hz.cheryme.top/gtayleiiam.html

按语言统计（条）：
来源：http://hz.zhaomingkeji.xyz/gtfaqnksbt.html

Python ......... 252
来源：http://hz.zhaomingkeji.xyz/gtvwiweqac.html

PHP ............ 252
来源：http://hz.yongpay.top/gtrckoobyw.html

JavaScript ..... 252
来源：http://hz.hnxiangtu.top/gtkgwajtqs.html

TypeScript ..... 212
来源：http://hz.tanke756.top/gttolpfxjw.html

Java ........... 212
来源：http://hz.nwbrower.top/gtfbngpbdk.html

Go ............. 212
来源：http://hz.xinyue.icu/gtktdpenfe.html

Ruby ........... 212
来源：http://hz.nanxinkj.top/gteymtgduu.html

C# ............. 212
来源：http://hz.zhengqikj.top/gtjgqtuesm.html

C .............. 30
来源：http://hz.daria6918.cn/gtwniqojgf.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtwxmugejz.html

SQL ............ 90
来源：http://hz.hfpthk.cn/gtbmlgvfiv.html

Bash ........... 80
来源：http://hz.shanyushiyangkeji.top/gtkyuuvoxh.html

Kotlin ......... 15
来源：http://hz.yuxming.cn/gtdmtnmgnp.html

Swift .......... 15
来源：http://hz.guowangkeji.top/gtrukgemoa.html

Lua ............ 10
来源：http://hz.yj202588.top/gtpkqguuwh.html

Perl ........... 10
来源：http://hz.guowangkeji.top/gttjvolkxz.html

Scala .......... 10
来源：http://hz.jiagoushi.top/gtaceoicdw.html

------------------------------------
来源：http://hz.316326.xyz/gtbjzctuyk.html

合计 ........... 2106 条
来源：http://hz.jqgfzy.top/gtkasmjrxg.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtlttvxcpx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daria6918.cn/gtldlinunm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtehfmqjip.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtldwkwvlr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtfptqdvfk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtuwnuwlqh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtkluxdtow.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtedlxvvlk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jianghu66.top/gtcfpdfjvr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtyqxohsbo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.bjfxy.top/gtpinkiysv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtwncoqpvm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtiyemuxbc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gttxxvzoay.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtqvitqkcc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxuanxn.top/gtjltftsqn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtamwzxqnt.html

Q SQL 专题                              90
来源：http://hz.cashguo.top/gtqeovhtlx.html

R Bash 专题                             80
来源：http://hz.yangfankeji.com/gtbtvooaoy.html

S C / C++ 专题                          60
来源：http://hz.chenjidiqi.icu/gtjzwqkstg.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gttxfjmetb.html

U 高频实用片段                         120
来源：http://hz.daxiang520.top/gtdzccuifn.html

------------------------------------
来源：http://hz.havefunace.top/gtavdfooxg.html

合计                                  2106 条
来源：http://hz.pengpengdd.cyou/gtbjcpjgbv.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtorhknoqg.html


<!-- 参考信息 -->