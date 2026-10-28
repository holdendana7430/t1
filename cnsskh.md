代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtdawpzvlk.html

[T59] Scala：循环
来源：http://hz.yj20258.top/gtxprwzfnn.html

for (i <- 1 to 10) println(i)
来源：http://hz.xylfe.cn/gttjfepvof.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtuefqqzwi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtggvjkphk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwgkksfnv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yangfankeji.com/gtjthrslew.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsykftdtq.html

[U01] Py：创建虚拟环境
来源：http://hz.havefunace.top/gtxyocikur.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yuxming.cn/gtqxlazgyo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tanke756.top/gtbhtprwrj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.wangdashe.top/gtroqkydbr.html

[U03] Py：加载 .env 配置
来源：http://hz.52xcode.cn/gteqbrnxcy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gtgvbcwdqq.html

[U04] Py：变量调试打印
来源：http://hz.jqgufenzy.top/gthibqpxty.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shzxlz.cn/gtwwyxkcdr.html

[U05] Py：列表去重且保序
来源：http://hz.xylfe.cn/gtrtqnnhxx.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtbcmeocby.html

[U06] Py：合并两个字典
来源：http://hz.yonumen.top/gtbgvfwpfg.html

{**a, **b}
来源：http://hz.nanxinkj.top/gtvdgbdkxx.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtyfgduyjw.html

{v: k for k, v in d.items()}
来源：http://hz.xuetiantiany.cn/gtwjlecwpg.html

[U08] Py：展平二维列表
来源：http://hz.cashguo.top/gtidbpnwpb.html

[y for x in nested for y in x]
来源：http://hz.iojbl.cn/gtgvrnqdcg.html

[U09] Py：字典取最大值的键
来源：http://hz.svipenyu.cn/gtjmsmmcvb.html

max(d, key=d.get)
来源：http://hz.shanyushiyangtech.top/gtmohtnshx.html

[U10] Py：按值排序字典
来源：http://hz.cheryme.top/gtoqslrpre.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.fzhhl.top/gtjugxcrha.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtkkljquum.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gtkawaunxy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinyuanbaomall.cn/gtipnnmvtr.html

Counter(arr).most_common(3)
来源：http://hz.guowangkeji.top/gtkssxmfgr.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gtkktpnatg.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gtsclshlqo.html

[U14] Py：分组收集到列表
来源：http://hz.aizwys.cn/gtcudwljvp.html

defaultdict(list)
来源：http://hz.wangshuangyany.cn/gtsohiosva.html

[U15] Py：高精度计时
来源：http://hz.zhiwuduotai.top/gtncjnezro.html

t = time.perf_counter()
来源：http://hz.yvedp.cn/gtxqoqccig.html

[U16] Py：命令行参数解析
来源：http://hz.52xcode.cn/gtzutomflo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhengqikj.top/gtsbctsjox.html

[U17] Py：初始化日志
来源：http://hz.pycfn.com/gtiatrqrga.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hnxiangtu.top/gtwbttvwrk.html

[U18] Py：预编译正则
来源：http://hz.sufxvd.cn/gthkopbclk.html

pat = re.compile(r"\d+")
来源：http://hz.fzhhl.top/gtwpbbxjnl.html

[U19] Py：正则替换带回调
来源：http://hz.nanxuanxn.top/gtpkfcgiuc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.birdmap.top/gtxxluskgo.html

[U20] Py：缓存函数结果
来源：http://hz.zhiwuduotai.top/gtxeimzvbu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgufenzy.top/gtqbxrdzwa.html

[U21] Py：自定义上下文管理器
来源：http://hz.yangfankeji.com/gtjiexbdwj.html

@contextlib.contextmanager
来源：http://hz.jinghuilouyu.cn/gtupdgbzgh.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtdpgjrgin.html

list(zip(*m))
来源：http://hz.xylfe.cn/gtqymnnkgt.html

[U23] Py：分块读取大文件
来源：http://hz.smart0.xyz/gtdryrdaqy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj202588.top/gtmplqmgqc.html

[U24] Py：路径操作
来源：http://hz.ywan-chungtsiang.top/gtdkfociaq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtfxlwgrsn.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtqlyyqudj.html

csv.DictReader(f)
来源：http://hz.zhixingplan.top/gtlerphgjo.html

[U26] Py：并发下载
来源：http://hz.gzhubu.top/gtwnwquuwa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daria6918.cn/gttevrrwil.html

[U27] Py：异步 HTTP
来源：http://hz.guannengcc.top/gtwzghsevr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhoulong.xyz/gtfxrbxesf.html

[U28] Py：类型别名
来源：http://hz.jqgufenzy.top/gtzmqbjjsm.html

UserId = int
来源：http://hz.xingfuxueyuan.xyz/gtqoccaeqm.html

[U29] Py：属性校验
来源：http://hz.kuanghao11.cn/gtepadzxme.html

@property 与 @x.setter 配合
来源：http://hz.jinyuanbaomall.cn/gttjmmrffb.html

[U30] Py：数据类
来源：http://hz.jianghu66.top/gtazlyvdkp.html

@dataclass(slots=True)
来源：http://hz.zhixingplan.top/gtdptwewrf.html

[U31] Py：单测
来源：http://hz.svipenyu.cn/gtlrqwkcdu.html

python -m pytest -q
来源：http://hz.jianghu66.top/gtkoylgqip.html

[U32] Py：代码格式化
来源：http://hz.jqgfzy.top/gtzhykvudw.html

ruff format . && ruff check --fix .
来源：http://hz.hfpthk.cn/gtzfxywudk.html

[U33] Py：打包发布
来源：http://hz.cashguo.top/gtyckgnbgv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258888.top/gtqsogcxbl.html

[U34] Py：判断编码
来源：http://hz.yj20258.top/gthdkunmsu.html

chardet.detect(raw)
来源：http://hz.xinyue.icu/gtakiioigd.html

[U35] Py：发送邮件
来源：http://hz.ybcxt.top/gtemlyzazp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.chenjidiqi.icu/gtqpeeqftk.html

[U36] Py：定时任务
来源：http://hz.yangfankeji.com/gtgsrvdvyt.html

schedule.every(10).minutes.do(job)
来源：http://hz.iojbl.cn/gtmiwoxdad.html

[U37] Py：读写 Excel
来源：http://hz.yangfankeji.com/gtvbvvxpqn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sxryk.cn/gtfbxmudou.html

[U38] Py：获取脚本所在目录
来源：http://hz.pengpengdd.cyou/gtlroclxcn.html

Path(__file__).resolve().parent
来源：http://hz.ybcxt.top/gtnjvgoirt.html

[U39] Py：判断是否在交互环境
来源：http://hz.svipenyu.cn/gtazxohvft.html

sys.stdout.isatty()
来源：http://hz.nanxinkj.top/gtuimyiati.html

[U40] Py：打印到标准错误
来源：http://hz.shzxlz.cn/gtodgkkiax.html

print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtrzljdrzu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zdqjudy.top/gtupqavwcn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.c1oappe.top/gtqjvpwqmq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hfpthk.cn/gtdnqqjzhd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dianchejie.cn/gtukogueig.html

[U43] PHP：声明命名空间
来源：http://hz.daria6918.cn/gtthkotkho.html

namespace App\Http;
来源：http://hz.aibaodan.cn/gtfjtywzma.html

[U44] PHP：开启严格类型
来源：http://hz.jinghuilouyu.cn/gtjprrlelu.html

declare(strict_types=1);
来源：http://hz.fengsongda.top/gtwcvinsap.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenjidiqi.icu/gtuvlavdla.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gthxilizqx.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtsnzsftqr.html

?string $name = null
来源：http://hz.zhengqikj.top/gtuycnbbsp.html

[U47] PHP：联合类型
来源：http://hz.jqgufenzy.top/gtumyoalnt.html

int|string $id
来源：http://hz.zhengqikj.top/gtipgcsxpp.html

[U48] PHP：纯枚举
来源：http://hz.feifeiyinyue.top/gtgamkejhj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtwtxlogiz.html

[U49] PHP：只读属性
来源：http://hz.yuxming.cn/gtrgoctxia.html

public readonly string $name
来源：http://hz.hysaishi.cn/gtyrwyiuun.html

[U50] PHP：构造器属性提升
来源：http://hz.hysaishi.cn/gtjlwcosyt.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gtoloteboz.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangtech.top/gttebatkzt.html

[$a, $b] = $arr;
来源：http://hz.fzhhl.top/gtnaaezjfm.html

[U52] PHP：箭头函数
来源：http://hz.gogol.net.cn/gtbdtxmrzv.html

$double = fn($x) => $x * 2;
来源：http://hz.ehwqpu.com/gtffpsilxw.html

[U53] PHP：空合并运算符
来源：http://hz.nanxinkj.top/gtjrllgzpt.html

$v = $a ?? $b ?? "default";
来源：http://hz.tian-w.cn/gthcubnrjc.html

[U54] PHP：空安全调用
来源：http://hz.andypj.xyz/gtktjunrgx.html

$obj?->method()
来源：http://hz.shanyushiyangkeji.top/gtqjizzdro.html

[U55] PHP：match 表达式
来源：http://hz.snrcjt.cn/gthrqqdmwl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.0kj1m.cn/gtcqtlwpme.html

[U56] PHP：命名参数
来源：http://hz.shzxlz.cn/gtahesnopn.html

f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtulowjsne.html

[U57] PHP：字符串插值
来源：http://hz.gotoacloud.top/gtcgrpstxe.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtuuxueimi.html

[U58] PHP：数组三件套
来源：http://hz.nanxuanxn.top/gtljhweyxq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ybcxt.top/gtngbytyxa.html

[U59] PHP：自定义排序
来源：http://hz.tianlin.xyz/gtizoukmam.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtjrtsikzk.html

[U60] PHP：JSON 编解码
来源：http://hz.kuanghao11.cn/gtopbnjbdi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuanzx.com/gtpjczjhdx.html

[U61] PHP：正则
来源：http://hz.hammf.cn/gtyxvqkwis.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtotiglbkf.html

[U62] PHP：日期对象
来源：http://hz.xziqi.cn/gtpfhicrjk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sxryk.cn/gtkgkwgeup.html

[U63] PHP：文件读写
来源：http://hz.xinyue.icu/gtgupytchv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.daxiang520.top/gtpgjvdkaq.html

[U64] PHP：目录遍历
来源：http://hz.daxiang520.top/gtmhfuoxyn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ybcxt.top/gtxuunbvnj.html

[U65] PHP：会话
来源：http://hz.fzhhl.top/gtewdjmmpf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gtohmickby.html

[U66] PHP：设置 Cookie
来源：http://hz.yongpay.top/gtccgypdzd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tianlin.xyz/gtcyehvzrs.html

[U67] PHP：处理文件上传
来源：http://hz.hysaishi.cn/gtbymrhlir.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.guowangkeji.top/gtpockmpxt.html

[U68] PHP：PDO 连接
来源：http://hz.hammf.cn/gtiquoykot.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hnxiangtu.top/gttdfbaooy.html

[U69] PHP：PDO 预处理
来源：http://hz.feifeiyinyue.top/gtdthvybuq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dianchejie.cn/gtprlkwiew.html

[U70] PHP：PDO 事务
来源：http://hz.chenlongwang.top/gtathsidur.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sxryk.cn/gtqbgfwhef.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtukpgbvwx.html

throw new RuntimeException("失败", 500);
来源：http://hz.dianchejie.cn/gtrpcsclcp.html

[U72] PHP：写错误日志
来源：http://hz.52xcode.cn/gtjwllvtca.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hammf.cn/gtygpultxz.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigufen.top/gtdyckenxy.html

parse_ini_file("config.ini", true)
来源：http://hz.gogol.net.cn/gtwkyqsaeh.html

[U74] PHP：读取环境变量
来源：http://hz.hysaishi.cn/gtoszgidqt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ybcxt.top/gttwyucjqo.html

[U75] PHP：依赖注入
来源：http://hz.zhaomingkeji.xyz/gtedlrzetb.html

composer require psr/container
来源：http://hz.bjfxy.top/gtxhacoqfe.html

[U76] PHP：简单路由
来源：http://hz.cucudq.cn/gtpcnkvelj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.kuanghao11.cn/gtespymftv.html

[U77] PHP：模板渲染
来源：http://hz.nanxinkj.top/gtrqntmerl.html

composer require twig/twig
来源：http://hz.ydzc1.top/gtonumrtlu.html

[U78] PHP：单元测试
来源：http://hz.yonumen.top/gtztungpye.html

composer require --dev phpunit/phpunit
来源：http://hz.yj20258888.top/gtqkdfogyl.html

[U79] PHP：静态分析
来源：http://hz.yuanzhike.top/gtdzyactxp.html

composer require --dev phpstan/phpstan
来源：http://hz.hammf.cn/gtokliyaqe.html

[U80] PHP：代码规范修复
来源：http://hz.yongpay.top/gthcgjmqjf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hfpthk.cn/gtoufagzyp.html

[U81] JS：初始化项目
来源：http://hz.ppjwa.cn/gtqakuwvpn.html

npm init -y;  npm i express
来源：http://hz.zhongyouzk.top/gtnohabpvd.html

[U82] JS：package.json 脚本
来源：http://hz.pengpengdd.cyou/gthcvfieto.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shanyushiyangkeji.top/gtqrbkljat.html

[U83] JS：ES Module 导入导出
来源：http://hz.guowangkeji.top/gtitosjhxv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cucudq.cn/gtgwbmlxms.html

[U84] JS：CommonJS 写法
来源：http://hz.fengsongda.top/gtdfyexmmv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hywenlv.cn/gtfzajehkp.html

[U85] JS：可选链
来源：http://hz.dianchejie.cn/gtxsjbfctc.html

a?.b?.c
来源：http://hz.hnxiangtu.top/gtbrdoysqm.html

[U86] JS：空值合并
来源：http://hz.yongpay.top/gtvnvzuymh.html

a ?? b
来源：http://hz.zhengqikj.top/gtxdlrmaau.html

[U87] JS：解构默认值
来源：http://hz.tian-w.cn/gtxfijhxeo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cdnleiting.top/gtjxmcrrin.html

[U88] JS：对象展开合并
来源：http://hz.ehwqpu.com/gtmhpdahmn.html

{ ...a, ...b }
来源：http://hz.zycfv.cn/gtdqabwusp.html

[U89] JS：数组去重
来源：http://hz.0kj1m.cn/gtljxnbpef.html

[...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtohbxiqrs.html

[U90] JS：数字数组排序
来源：http://hz.andypj.xyz/gtjyjhewpw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtmnqrploq.html

[U91] JS：对象键值遍历
来源：http://hz.sufxvd.cn/gtihmsllca.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xingfuxueyuan.xyz/gtwozokaxk.html

[U92] JS：深拷贝
来源：http://hz.yongpay.top/gthscjufjn.html

structuredClone(obj)
来源：http://hz.jyoumei.cn/gtlbdnbexa.html

[U93] JS：模板字符串
来源：http://hz.hfpthk.cn/gtygdszrfg.html

`共 ${n} 条`
来源：http://hz.chenjidiqi.icu/gtmjfqihxd.html

[U94] JS：箭头函数
来源：http://hz.tian-w.cn/gtwqbmciib.html

const double = x => x * 2;
来源：http://hz.shanyushiyangkeji.top/gttnessdas.html

[U95] JS：Promise 包装
来源：http://hz.yj20258888.top/gtjfnmoayq.html

new Promise((resolve, reject) => {})
来源：http://hz.hnqzz.top/gtmqatgtus.html

[U96] JS：async/await 与异常
来源：http://hz.zdqjudy.top/gtupfmeoyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtefasmsoi.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtxkodzfzp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtakotlkhx.html

[U98] JS：fetch 带 JSON
来源：http://hz.shanyushiyangtech.top/gtuevaqmas.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gtuyxbnngh.html

[U99] JS：事件监听
来源：http://hz.jinyuanbaomall.cn/gtitbsublw.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtfozffviu.html

[U100] JS：DOM 查询
来源：http://hz.jlsjyb.cn/gttyudmhbw.html

document.querySelector(".item")
来源：http://hz.bjfxy.top/gtfcuxapjq.html

[U101] JS：classList 操作
来源：http://hz.andypj.xyz/gtcytwqfyv.html

el.classList.toggle("active")
来源：http://hz.chenjidiqi.icu/gtceilmanh.html

[U102] JS：本地存储
来源：http://hz.guowangkeji.top/gtuuuktfad.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtumydlqob.html

[U103] JS：定时器
来源：http://hz.xingfuxueyuan.xyz/gtabihbpaj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.fzhhl.top/gtvzqinefc.html

[U104] JS：防抖
来源：http://hz.hammf.cn/gtjpwapkcy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtmukskoyv.html

[U105] JS：节流
来源：http://hz.mhx1999.top/gtogcjujle.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tian-w.cn/gtwjyswzzw.html

[U106] JS：日期格式化
来源：http://hz.zdqjudy.top/gtaylqbijl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ywan-chungtsiang.top/gtanilrvhf.html

[U107] JS：数字千分位
来源：http://hz.xziqi.cn/gthuiktnfr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shuidangran.top/gtxthjldoy.html

[U108] JS：随机整数
来源：http://hz.hnxiangtu.top/gtxzarvxtg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gtrdeepjwn.html

[U109] JS：数组分组
来源：http://hz.wangshuangyany.cn/gtavavpszs.html

Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtmlufniaa.html

[U110] JS：数组分块
来源：http://hz.redwolf501.top/gtjzcrmvug.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.redwolf501.top/gticofhjud.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtjanhauji.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gtblzkodzz.html

[U112] JS：字符串补位
来源：http://hz.jinyuanbaomall.cn/gtpuczplxz.html

"7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtdhldkfag.html

[U113] JS：正则替换全部
来源：http://hz.yueranfly.top/gtixsnmqzs.html

s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtzvnecewj.html

[U114] JS：JSON 深比较
来源：http://hz.316326.xyz/gtymsvuogu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtillkdklz.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtvfhinipb.html

crypto.randomUUID()
来源：http://hz.tanke756.top/gtamekvlyy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigfzy.top/gtftaxmymz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gttywzhrua.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtqoaurgcx.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgufenzy.top/gtmeyrylqg.html

[U118] JS：开发服务器
来源：http://hz.zycfv.cn/gtmjtjgpyp.html

npm i -D vite;  npx vite
来源：http://hz.fzhhl.top/gtojdselmx.html

[U119] JS：生产构建
来源：http://hz.zhongyouzk.top/gtzgadjqrd.html

npx vite build
来源：http://hz.shzxlz.cn/gthbhxrvlq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhijiandao.cn/gthrcvjffe.html

import.meta.env.VITE_API_URL
来源：http://hz.xylfe.cn/gtvxyofmtx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtytqvqdaf.html

统计汇总
来源：http://hz.yueranfly.top/gtzuemeizm.html

================================================================================
来源：http://hz.nwbrower.top/gtpawvnihb.html

按语言统计（条）：
来源：http://hz.hammf.cn/gtlbbqbsaq.html

Python ......... 252
来源：http://hz.tian-w.cn/gtphhhfuey.html

PHP ............ 252
来源：http://hz.0kj1m.cn/gthrcgsahf.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gtzdddzznf.html

TypeScript ..... 212
来源：http://hz.xingfuxueyuan.xyz/gtasuvwcbp.html

Java ........... 212
来源：http://hz.zhaomingkeji.xyz/gtqavzzonk.html

Go ............. 212
来源：http://hz.9152youxi.cn/gtdyuhdtxs.html

Ruby ........... 212
来源：http://hz.hammf.cn/gtltxxkgfm.html

C# ............. 212
来源：http://hz.dashuyun.cn/gtuqzdcmhs.html

C .............. 30
来源：http://hz.shangyingyoupin.top/gtaydfgmyl.html

C++ ............ 30
来源：http://hz.guannengcc.top/gtdcukyztx.html

SQL ............ 90
来源：http://hz.ppjwa.cn/gtxbkrrwwg.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtjaipjpbm.html

Kotlin ......... 15
来源：http://hz.jianghu66.top/gtwbxjathf.html

Swift .......... 15
来源：http://hz.gaohongyu789.top/gtedaoywxb.html

Lua ............ 10
来源：http://hz.iojbl.cn/gtwmgndfog.html

Perl ........... 10
来源：http://hz.yuanzhike.top/gtnsaciuen.html

Scala .......... 10
来源：http://hz.hammf.cn/gtksjrapia.html

------------------------------------
来源：http://hz.sysykeji.top/gtgiqmfkga.html

合计 ........... 2106 条
来源：http://hz.mhx1999.top/gtmqgeenjy.html

按章节统计：
来源：http://hz.jinghuilouyu.cn/gtglnrffqx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtzancstvh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtktitvghw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtlclzztjl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtnqyetexv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sufxvd.cn/gtsuqvhurv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtqxzyjczu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtlnubzkyx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtpzfrctzd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gteonnochv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.kuanghao11.cn/gtxnsaewew.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtmtkcyvlk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtyhdftygl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtzkktlfwe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtusymzjnz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jianghu66.top/gtvautyprt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtahynblnx.html

Q SQL 专题                              90
来源：http://hz.zhixingplan.top/gtstvnmzww.html

R Bash 专题                             80
来源：http://hz.zhengqikj.top/gtgnnwhvom.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtscvwomph.html

T 其他语言补充                          60
来源：http://hz.meibo888.top/gtjiayvzeg.html

U 高频实用片段                         120
来源：http://hz.xinyue.icu/gtniausqtq.html

------------------------------------
来源：http://hz.cheryme.top/gtqtvrxrts.html

合计                                  2106 条
来源：http://hz.chenlongwang.top/gtmkusjmzb.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gttzqvbkhk.html

使用提醒
来源：http://hz.yvedp.cn/gtblebklfk.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtnfxpqyxg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.bjfxy.top/gtkpzsbhlx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.mhx1999.top/gtebtmywkd.html


<!-- 参考信息 -->