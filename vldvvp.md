代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gtqdhbtdfe.html

================================================================================
来源：http://hz.guowangkeji.top/gthmdheprj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgfzy.top/gtgmafajoc.html

================================================================================
来源：http://hz.yuxming.cn/gtfhhiewyl.html

[U01] Py：创建虚拟环境
来源：http://hz.nwbrower.top/gtukljhjug.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pycfn.com/gtnzptdpev.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hysaishi.cn/gtxfluperb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ybcxt.top/gtslcxfjwr.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtpfxnhvlu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtxpnazvjt.html

[U04] Py：变量调试打印
来源：http://hz.nanxinkj.top/gtsdkiozwg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jlsjyb.cn/gtotekmqma.html

[U05] Py：列表去重且保序
来源：http://hz.zhixingplan.top/gtwvhsxzsk.html

list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtsughzquz.html

[U06] Py：合并两个字典
来源：http://hz.tianlin.xyz/gtohyuqcct.html

{**a, **b}
来源：http://hz.cqqwz.cn/gteystujaa.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangkeji.top/gtgyzqznjq.html

{v: k for k, v in d.items()}
来源：http://hz.meibo888.top/gtwysclkfu.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtehxnrdyf.html

[y for x in nested for y in x]
来源：http://hz.xingfuxueyuan.xyz/gtcvueelzk.html

[U09] Py：字典取最大值的键
来源：http://hz.0kj1m.cn/gtzreqzruo.html

max(d, key=d.get)
来源：http://hz.hongshengwenyu.top/gtkxienxea.html

[U10] Py：按值排序字典
来源：http://hz.c1oappe.top/gtojlhhjta.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dashuyun.cn/gtxaqmmvuw.html

[U11] Py：生成器表达式
来源：http://hz.jinghuilouyu.cn/gttmhqykwd.html

(x * 2 for x in arr)
来源：http://hz.aibaodan.cn/gtdaoftzku.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangshuangyany.cn/gtwmbdkodv.html

Counter(arr).most_common(3)
来源：http://hz.yueranfly.top/gtgqodyiem.html

[U13] Py：固定长度队列
来源：http://hz.guannengcc.top/gtagmrbhxe.html

deque(maxlen=10)
来源：http://hz.haohaochexian.top/gtvzzersfe.html

[U14] Py：分组收集到列表
来源：http://hz.feifeiyinyue.top/gtmucgupom.html

defaultdict(list)
来源：http://hz.c1oappe.top/gtezlxpuoy.html

[U15] Py：高精度计时
来源：http://hz.tian-w.cn/gtywsxtowr.html

t = time.perf_counter()
来源：http://hz.mhx1999.top/gtxxnjpnay.html

[U16] Py：命令行参数解析
来源：http://hz.yj20258888.top/gtcbozdqsr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtzjznuusn.html

[U17] Py：初始化日志
来源：http://hz.yj202588.top/gtiprllgns.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.snrcjt.cn/gtnocqsxex.html

[U18] Py：预编译正则
来源：http://hz.andypj.xyz/gtekcnfbnh.html

pat = re.compile(r"\d+")
来源：http://hz.zhijiandao.cn/gtqurmzqgi.html

[U19] Py：正则替换带回调
来源：http://hz.sweek.top/gtxgqekpmx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.feifeiyinyue.top/gthhbadzlh.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtyrdlbiuk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ydzc1.top/gtkggwlooa.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gtqnjrervl.html

@contextlib.contextmanager
来源：http://hz.jinqigufen.top/gtvbwhbxmu.html

[U22] Py：矩阵转置
来源：http://hz.ydzc1.top/gthecskqbd.html

list(zip(*m))
来源：http://hz.havefunace.top/gtnjhxstsj.html

[U23] Py：分块读取大文件
来源：http://hz.hywenlv.cn/gtgilskcbt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinqigfzy.top/gtdshqmhwj.html

[U24] Py：路径操作
来源：http://hz.zycfv.cn/gtcdmqzupw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydjk.org.cn/gtptwxwelg.html

[U25] Py：CSV 按字典读
来源：http://hz.316326.xyz/gtkbahvgzc.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtqupxtgga.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtvaqoumlv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nanxuanxn.top/gtuowdmfth.html

[U27] Py：异步 HTTP
来源：http://hz.yvedp.cn/gtvoibbvud.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtdrglgjrj.html

[U28] Py：类型别名
来源：http://hz.sysykeji.top/gtelsglgvs.html

UserId = int
来源：http://hz.tianlin.xyz/gtfanajfhz.html

[U29] Py：属性校验
来源：http://hz.xylfe.cn/gtxvorlhtc.html

@property 与 @x.setter 配合
来源：http://hz.kuanghao11.cn/gtdjwxoram.html

[U30] Py：数据类
来源：http://hz.xylfe.cn/gtaawmywgw.html

@dataclass(slots=True)
来源：http://hz.guannengcc.top/gturhnrtze.html

[U31] Py：单测
来源：http://hz.zhiwuduotai.top/gtgvytnqkk.html

python -m pytest -q
来源：http://hz.jinqigufen.top/gtlsqgkblj.html

[U32] Py：代码格式化
来源：http://hz.tanke756.top/gtcunvycga.html

ruff format . && ruff check --fix .
来源：http://hz.ybcxt.top/gtwrdmcivr.html

[U33] Py：打包发布
来源：http://hz.zhengqikj.top/gtwobklryr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhengqikj.top/gtynlvzbxo.html

[U34] Py：判断编码
来源：http://hz.cheryme.top/gtkdpcdpac.html

chardet.detect(raw)
来源：http://hz.jqgfzy.top/gtmaahcnyx.html

[U35] Py：发送邮件
来源：http://hz.birdmap.top/gthatulwed.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinqigfzy.top/gtrbclcaxn.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtiqvhgdft.html

schedule.every(10).minutes.do(job)
来源：http://hz.wangdashe.top/gtlwjgzbzq.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gtknrqfpgm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hfpthk.cn/gttykdouhb.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinqigfzy.top/gtycqfxtol.html

Path(__file__).resolve().parent
来源：http://hz.pycfn.com/gtupzachxe.html

[U39] Py：判断是否在交互环境
来源：http://hz.iojbl.cn/gtnxvuljhy.html

sys.stdout.isatty()
来源：http://hz.aizwys.cn/gtfybnusny.html

[U40] Py：打印到标准错误
来源：http://hz.sxryk.cn/gtgzalseiz.html

print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtfpdxsisy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cqqwz.cn/gtqrwbiuue.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.52xcode.cn/gtqbxarnpe.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenlongwang.top/gtemnwqfej.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dianchejie.cn/gtlrzirznu.html

[U43] PHP：声明命名空间
来源：http://hz.fzhhl.top/gtcpqjwabb.html

namespace App\Http;
来源：http://hz.hammf.cn/gtekzmqigj.html

[U44] PHP：开启严格类型
来源：http://hz.yueranfly.top/gtzrwqpvju.html

declare(strict_types=1);
来源：http://hz.jyoumei.cn/gtfogsisky.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dashuyun.cn/gtsgxosjrw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtpfgljfcl.html

[U46] PHP：可空类型
来源：http://hz.hongshengwenyu.top/gtkwvkzsmj.html

?string $name = null
来源：http://hz.ivvv.top/gtiafximfp.html

[U47] PHP：联合类型
来源：http://hz.yangfankeji.com/gtjuiifzba.html

int|string $id
来源：http://hz.shuidangran.top/gtmnzngqhq.html

[U48] PHP：纯枚举
来源：http://hz.daxiang520.top/gtmnfeidqe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.smart0.xyz/gtrdekbimo.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gtlncicnhe.html

public readonly string $name
来源：http://hz.daxiang520.top/gtwjpwwexv.html

[U50] PHP：构造器属性提升
来源：http://hz.zdqjudy.top/gtqmwuukjq.html

public function __construct(private int $id) {}
来源：http://hz.chenlongwang.top/gtgyzoiwud.html

[U51] PHP：数组解构
来源：http://hz.sufxvd.cn/gthqrzsuww.html

[$a, $b] = $arr;
来源：http://hz.zycfv.cn/gtiygoxmld.html

[U52] PHP：箭头函数
来源：http://hz.tanke756.top/gtmjqytyug.html

$double = fn($x) => $x * 2;
来源：http://hz.shanyushiyangkeji.top/gtzvyuflwg.html

[U53] PHP：空合并运算符
来源：http://hz.jyoumei.cn/gtgtekumrf.html

$v = $a ?? $b ?? "default";
来源：http://hz.smart0.xyz/gtbnvkbjtu.html

[U54] PHP：空安全调用
来源：http://hz.yj20258.top/gtxbeddjnx.html

$obj?->method()
来源：http://hz.shanyushiyangtech.top/gtxmxpchek.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtbnamznje.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenjidiqi.icu/gtceefhfko.html

[U56] PHP：命名参数
来源：http://hz.smart0.xyz/gtgevbtxri.html

f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtyxjajmlr.html

[U57] PHP：字符串插值
来源：http://hz.snrcjt.cn/gtuqrcxqyh.html

"值: {$a}"
来源：http://hz.yuxming.cn/gtnzwnhtoe.html

[U58] PHP：数组三件套
来源：http://hz.jinghuilouyu.cn/gtzekrkkxd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shuidangran.top/gtyfpnetiz.html

[U59] PHP：自定义排序
来源：http://hz.jinghuilouyu.cn/gtxoekpneb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtfvvoncya.html

[U60] PHP：JSON 编解码
来源：http://hz.ydzc1.top/gtbnehgrpq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gtvkbxkdja.html

[U61] PHP：正则
来源：http://hz.ydzc1.top/gtozmtizct.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtfwjvpsja.html

[U62] PHP：日期对象
来源：http://hz.fzhhl.top/gteafzivak.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zycfv.cn/gtqouzdqog.html

[U63] PHP：文件读写
来源：http://hz.hongshengwenyu.top/gtorcnrbat.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hongshengwenyu.top/gtinqxdyng.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtfoxxtkcr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tianlin.xyz/gtqodhttew.html

[U65] PHP：会话
来源：http://hz.dianchejie.cn/gtruyrrejl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nanxuanxn.top/gtalozvgwg.html

[U66] PHP：设置 Cookie
来源：http://hz.yuanzhike.top/gtpemgacuo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sufxvd.cn/gtthiycbis.html

[U67] PHP：处理文件上传
来源：http://hz.hnqzz.top/gtujtkztsc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jlsjyb.cn/gtdiovaahe.html

[U68] PHP：PDO 连接
来源：http://hz.hysaishi.cn/gtlddbovqu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigufen.top/gtwwzklzvu.html

[U69] PHP：PDO 预处理
来源：http://hz.dianchejie.cn/gtohvgnixs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgufenzy.top/gtipsvheaa.html

[U70] PHP：PDO 事务
来源：http://hz.316326.xyz/gtlsthxkbm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuetiantiany.cn/gtohxzjemp.html

[U71] PHP：抛出异常
来源：http://hz.nwbrower.top/gtmcufkayn.html

throw new RuntimeException("失败", 500);
来源：http://hz.svipenyu.cn/gtsgywuuff.html

[U72] PHP：写错误日志
来源：http://hz.vqdsnc.cn/gtliypwvrd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.c1oappe.top/gtueztnzib.html

[U73] PHP：读取 ini 配置
来源：http://hz.cdnleiting.top/gtkoizsdfh.html

parse_ini_file("config.ini", true)
来源：http://hz.gaohongyu789.top/gtgwmjhipw.html

[U74] PHP：读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtnzfneogm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hysaishi.cn/gtzqnvqxda.html

[U75] PHP：依赖注入
来源：http://hz.guannengcc.top/gtdaolwzvn.html

composer require psr/container
来源：http://hz.chenjidiqi.icu/gtnfqalybn.html

[U76] PHP：简单路由
来源：http://hz.cucudq.cn/gtuysmvoyu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gttqkmzhmi.html

[U77] PHP：模板渲染
来源：http://hz.jiagoushi.top/gtjzchzvyf.html

composer require twig/twig
来源：http://hz.yuxming.cn/gtocdwxkkz.html

[U78] PHP：单元测试
来源：http://hz.shanyushiyangkeji.top/gtzqhhoxyq.html

composer require --dev phpunit/phpunit
来源：http://hz.yj202588.top/gtqieshzei.html

[U79] PHP：静态分析
来源：http://hz.jianghu66.top/gtclyuqakk.html

composer require --dev phpstan/phpstan
来源：http://hz.pycfn.com/gtfwxaqtzq.html

[U80] PHP：代码规范修复
来源：http://hz.chenlongwang.top/gtosslxxos.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gogol.net.cn/gtwjqgbxde.html

[U81] JS：初始化项目
来源：http://hz.sweek.top/gtgjtmokrz.html

npm init -y;  npm i express
来源：http://hz.gogol.net.cn/gtwdxjaqgw.html

[U82] JS：package.json 脚本
来源：http://hz.tianlin.xyz/gtfceprxqh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.svipenyu.cn/gtmlbqeerk.html

[U83] JS：ES Module 导入导出
来源：http://hz.hongshengwenyu.top/gtepsbsrbv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.svipenyu.cn/gturqltwwv.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gtbrdosqcb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.0kj1m.cn/gtkjzxfcro.html

[U85] JS：可选链
来源：http://hz.yanxiufei.cn/gtltyylxjx.html

a?.b?.c
来源：http://hz.dashuyun.cn/gtrkryyhkn.html

[U86] JS：空值合并
来源：http://hz.daxiang520.top/gtlzbyhugt.html

a ?? b
来源：http://hz.chenjidiqi.icu/gtojbinppc.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gteysvkdwq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xuanzx.com/gtzoyluciw.html

[U88] JS：对象展开合并
来源：http://hz.zhongyouzk.top/gtobcvqrdb.html

{ ...a, ...b }
来源：http://hz.havefunace.top/gtkyeqgfiy.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangkeji.top/gtshtartkq.html

[...new Set(arr)]
来源：http://hz.0kj1m.cn/gtojbxotxd.html

[U90] JS：数字数组排序
来源：http://hz.yj20258888.top/gtwcqsaucp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtxgoiqsda.html

[U91] JS：对象键值遍历
来源：http://hz.svipenyu.cn/gtepfkquop.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yongpay.top/gtftmitpkr.html

[U92] JS：深拷贝
来源：http://hz.ydzc1.top/gtnynhcriu.html

structuredClone(obj)
来源：http://hz.cashguo.top/gtphgoffcg.html

[U93] JS：模板字符串
来源：http://hz.zycfv.cn/gtcqxnwtdo.html

`共 ${n} 条`
来源：http://hz.316326.xyz/gtiyoocqic.html

[U94] JS：箭头函数
来源：http://hz.yongpay.top/gtjgppcurp.html

const double = x => x * 2;
来源：http://hz.nwbrower.top/gtdiscskhb.html

[U95] JS：Promise 包装
来源：http://hz.xinyue.icu/gtydingmoi.html

new Promise((resolve, reject) => {})
来源：http://hz.cucudq.cn/gtnzkddopw.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtckebwubh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtengedvyz.html

[U97] JS：并发请求
来源：http://hz.pengpengdd.cyou/gtvjqhyoer.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtctpeehwa.html

[U98] JS：fetch 带 JSON
来源：http://hz.ehwqpu.com/gtegwttiqr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hysaishi.cn/gtlqqcafrc.html

[U99] JS：事件监听
来源：http://hz.shangyingyoupin.top/gtkkbzpkjs.html

el.addEventListener("click", e => {})
来源：http://hz.svipenyu.cn/gtnnkdudzf.html

[U100] JS：DOM 查询
来源：http://hz.zhixingplan.top/gtupqzwaff.html

document.querySelector(".item")
来源：http://hz.cashguo.top/gtaktmbqjl.html

[U101] JS：classList 操作
来源：http://hz.tianlin.xyz/gtcvfwxfpk.html

el.classList.toggle("active")
来源：http://hz.bjfxy.top/gttfwvfcfg.html

[U102] JS：本地存储
来源：http://hz.svipenyu.cn/gtxdwdwcio.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtegaokttl.html

[U103] JS：定时器
来源：http://hz.ybcxt.top/gtsphgroca.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jlsjyb.cn/gtgwcbwwfk.html

[U104] JS：防抖
来源：http://hz.gzhubu.top/gtepbkdsfv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtvtxcxoio.html

[U105] JS：节流
来源：http://hz.smart0.xyz/gtlqniubys.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dashuyun.cn/gtwfiwjgsi.html

[U106] JS：日期格式化
来源：http://hz.aizwys.cn/gtvndfwdji.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangtech.top/gtmkcsmjoe.html

[U107] JS：数字千分位
来源：http://hz.c1oappe.top/gtjurpwyxz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigfzy.top/gtlwucnaeb.html

[U108] JS：随机整数
来源：http://hz.zhoulong.xyz/gtlmchpyjd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.havefunace.top/gtobfrmvxg.html

[U109] JS：数组分组
来源：http://hz.hfpthk.cn/gtjhhcrihd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtfxwnbdjk.html

[U110] JS：数组分块
来源：http://hz.haohaochexian.top/gtpiystset.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hfpthk.cn/gtlgcccwqu.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gtgtwkgbse.html

new Map(Object.entries(obj))
来源：http://hz.ybcxt.top/gttwangedf.html

[U112] JS：字符串补位
来源：http://hz.yuxming.cn/gthvtbatan.html

"7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtpxdqfzzo.html

[U113] JS：正则替换全部
来源：http://hz.dashuyun.cn/gtaymclbej.html

s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtvnpsxtjy.html

[U114] JS：JSON 深比较
来源：http://hz.aibaodan.cn/gtrkbvdcpd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.vqdsnc.cn/gtbtqngrtm.html

[U115] JS：生成 UUID
来源：http://hz.chenlongwang.top/gtblhilpov.html

crypto.randomUUID()
来源：http://hz.yueranfly.top/gtwrirsesi.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtnpqbbrro.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hywenlv.cn/gtpwtmrhan.html

[U117] JS：单元测试
来源：http://hz.iojbl.cn/gtxomgnmzo.html

npm i -D vitest;  npx vitest
来源：http://hz.guowangkeji.top/gtsewuilwj.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gtjfopvofl.html

npm i -D vite;  npx vite
来源：http://hz.vqdsnc.cn/gtagjnisvd.html

[U119] JS：生产构建
来源：http://hz.dianchejie.cn/gthbnnxomq.html

npx vite build
来源：http://hz.sysykeji.top/gtqksefukt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.dianchejie.cn/gtlpvkugfl.html

import.meta.env.VITE_API_URL
来源：http://hz.kuanghao11.cn/gtuicxzjoj.html

================================================================================
来源：http://hz.bjfxy.top/gtsdaxadvk.html

统计汇总
来源：http://hz.ydzc1.top/gtjhdecnuo.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtlbyrdbub.html

按语言统计（条）：
来源：http://hz.bjfxy.top/gtepeibkyt.html

Python ......... 252
来源：http://hz.ydjk.org.cn/gtmhuuqddx.html

PHP ............ 252
来源：http://hz.ydjk.org.cn/gtknvgnqpm.html

JavaScript ..... 252
来源：http://hz.gotoacloud.top/gtnhjngnhh.html

TypeScript ..... 212
来源：http://hz.yj20258.top/gtddrlhldq.html

Java ........... 212
来源：http://hz.aibaodan.cn/gteaysldor.html

Go ............. 212
来源：http://hz.sysykeji.top/gtwtqpmgzg.html

Ruby ........... 212
来源：http://hz.yj20258888.top/gtxbikgqpq.html

C# ............. 212
来源：http://hz.ivvv.top/gtzvtjopia.html

C .............. 30
来源：http://hz.birdmap.top/gtasmubijl.html

C++ ............ 30
来源：http://hz.daxiang520.top/gtlpyewyhr.html

SQL ............ 90
来源：http://hz.yuxming.cn/gtlzbgflkq.html

Bash ........... 80
来源：http://hz.ehwqpu.com/gtwereizxb.html

Kotlin ......... 15
来源：http://hz.yonumen.top/gtxvdqlqnr.html

Swift .......... 15
来源：http://hz.iojbl.cn/gtilzegosx.html

Lua ............ 10
来源：http://hz.yanxiufei.cn/gtuimshcgx.html

Perl ........... 10
来源：http://hz.feifeiyinyue.top/gttfswaqzd.html

Scala .......... 10
来源：http://hz.tanke756.top/gtynfxufxz.html

------------------------------------
来源：http://hz.jiagoushi.top/gtuxcxomtd.html

合计 ........... 2106 条
来源：http://hz.andypj.xyz/gtuhmghgkh.html

按章节统计：
来源：http://hz.quarkkingdee.top/gtvojlkmfx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258.top/gtqgzzbdtk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtddbcjaev.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtxqqsblru.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gttvghvpew.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.pycfn.com/gtpmcvzotm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtdbyujlbi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtkfrgumdq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtgzaqpzcp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gthksuluto.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gotoacloud.top/gtpcwlwjpr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtdrpfdihz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtyxtsyyiq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtkaofuuuc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.birdmap.top/gtlodzqtwd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangkeji.top/gthilhkaor.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtkktalzgq.html

Q SQL 专题                              90
来源：http://hz.ydzc1.top/gtzoaaeepo.html

R Bash 专题                             80
来源：http://hz.jlsjyb.cn/gtrcepnygn.html

S C / C++ 专题                          60
来源：http://hz.yangfankeji.com/gtkfzdxlsx.html

T 其他语言补充                          60
来源：http://hz.jinyuanbaomall.cn/gtftfouapd.html

U 高频实用片段                         120
来源：http://hz.hnqzz.top/gtxiooznjt.html

------------------------------------
来源：http://hz.jqgfzy.top/gtzmcegkiy.html

合计                                  2106 条
来源：http://hz.nwbrower.top/gticdleedf.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtevqcszzk.html

使用提醒
来源：http://hz.xuetiantiany.cn/gtwyyuefbl.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtkvaplent.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.redwolf501.top/gthbnltyzz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.0kj1m.cn/gtgonlrkpc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.havefunace.top/gttlmsnaeu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cqqwz.cn/gtetlhqtlt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.havefunace.top/gtgwhozibp.html

—— 文件结束 ——
来源：http://hz.pycfn.com/gtrhomdias.html


<!-- 参考信息 -->