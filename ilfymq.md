代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhaomingkeji.xyz/gtsjvaffhz.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtyoflyewo.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtynesvkrf.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gttpljjxgf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.meibo888.top/gtltxujfri.html

================================================================================
来源：http://hz.0kj1m.cn/gttrtaphpy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtbqadfzcw.html

================================================================================
来源：http://hz.mhx1999.top/gtcrfmhasj.html

[U01] Py：创建虚拟环境
来源：http://hz.ppjwa.cn/gtwvpgirth.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pycfn.com/gtpzstdkwb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.0kj1m.cn/gtknsewtbw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gttafiiuso.html

[U03] Py：加载 .env 配置
来源：http://hz.nanxuanxn.top/gtntfjtmuk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhaomingkeji.xyz/gtbmprynyp.html

[U04] Py：变量调试打印
来源：http://hz.sxryk.cn/gtysgvntip.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhongyouzk.top/gtigigkjmr.html

[U05] Py：列表去重且保序
来源：http://hz.aibaodan.cn/gtqoflgzbh.html

list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtqmxznmqh.html

[U06] Py：合并两个字典
来源：http://hz.yj20258.top/gtvjqvobbx.html

{**a, **b}
来源：http://hz.daxiang520.top/gthbhzzjbt.html

[U07] Py：反转字典键值
来源：http://hz.gotoacloud.top/gtajopnoow.html

{v: k for k, v in d.items()}
来源：http://hz.9152youxi.cn/gtanhxqwuf.html

[U08] Py：展平二维列表
来源：http://hz.yonumen.top/gtjwicduzy.html

[y for x in nested for y in x]
来源：http://hz.aizwys.cn/gtwxttdndg.html

[U09] Py：字典取最大值的键
来源：http://hz.nwbrower.top/gtgkhwwyup.html

max(d, key=d.get)
来源：http://hz.c1oappe.top/gtwcojwmff.html

[U10] Py：按值排序字典
来源：http://hz.havefunace.top/gtsenjnawx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xingfuxueyuan.xyz/gtovucrxaj.html

[U11] Py：生成器表达式
来源：http://hz.iojbl.cn/gtaairssdy.html

(x * 2 for x in arr)
来源：http://hz.vqdsnc.cn/gtgrbdrsbz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sweek.top/gtekvwlsth.html

Counter(arr).most_common(3)
来源：http://hz.hfpthk.cn/gtlqcnyivw.html

[U13] Py：固定长度队列
来源：http://hz.cdnleiting.top/gtjmbhohkf.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gthdwakxdi.html

[U14] Py：分组收集到列表
来源：http://hz.mhx1999.top/gtkiqgsuya.html

defaultdict(list)
来源：http://hz.jianghu66.top/gtdgljofqm.html

[U15] Py：高精度计时
来源：http://hz.sweek.top/gtadvsgfkm.html

t = time.perf_counter()
来源：http://hz.bjfxy.top/gtylmwmlch.html

[U16] Py：命令行参数解析
来源：http://hz.xingfuxueyuan.xyz/gtqjaafdtj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigfzy.top/gtmfmqgyjy.html

[U17] Py：初始化日志
来源：http://hz.daria6918.cn/gtothwcdtp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtsnodword.html

[U18] Py：预编译正则
来源：http://hz.pengpengdd.cyou/gtuhvzherf.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangkeji.top/gttvllgapd.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtwsiatbny.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtrbzpzlpq.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtfxywoplu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hammf.cn/gtfjrinzft.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydjk.org.cn/gtqyvhtytd.html

@contextlib.contextmanager
来源：http://hz.tianlin.xyz/gtpizyqhmp.html

[U22] Py：矩阵转置
来源：http://hz.mhx1999.top/gtpnaceztw.html

list(zip(*m))
来源：http://hz.wangshuangyany.cn/gtwjihtdbl.html

[U23] Py：分块读取大文件
来源：http://hz.svipenyu.cn/gtuuianagu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangkeji.top/gtnpzrdxmh.html

[U24] Py：路径操作
来源：http://hz.mhx1999.top/gtlpuxjqox.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tianlin.xyz/gtnjwykflf.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gtezvitjpf.html

csv.DictReader(f)
来源：http://hz.guowangkeji.top/gtxyuznpty.html

[U26] Py：并发下载
来源：http://hz.0kj1m.cn/gthzlqdwul.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgufenzy.top/gtjfrvxzjg.html

[U27] Py：异步 HTTP
来源：http://hz.ydzc1.top/gtcqwzefbz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxuanxn.top/gtdxkrepvf.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtjqlxspme.html

UserId = int
来源：http://hz.shzxlz.cn/gtvbqqonjj.html

[U29] Py：属性校验
来源：http://hz.yj20258888.top/gtdywjpyhk.html

@property 与 @x.setter 配合
来源：http://hz.cheryme.top/gtsnmswxkg.html

[U30] Py：数据类
来源：http://hz.aizwys.cn/gtlufglsci.html

@dataclass(slots=True)
来源：http://hz.snrcjt.cn/gtsgtpmrqa.html

[U31] Py：单测
来源：http://hz.hammf.cn/gtrjicibgr.html

python -m pytest -q
来源：http://hz.xylfe.cn/gtxkfppdkc.html

[U32] Py：代码格式化
来源：http://hz.hongshengwenyu.top/gtzdowwzkp.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtfuvyppnh.html

[U33] Py：打包发布
来源：http://hz.zhongyouzk.top/gtwuiemefz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigfzy.top/gtasznspsq.html

[U34] Py：判断编码
来源：http://hz.yongpay.top/gticqwieyg.html

chardet.detect(raw)
来源：http://hz.nwbrower.top/gtdicuaodi.html

[U35] Py：发送邮件
来源：http://hz.yuxming.cn/gtfebzkmhf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ybcxt.top/gtzszigfop.html

[U36] Py：定时任务
来源：http://hz.ywan-chungtsiang.top/gtrtnmfpzc.html

schedule.every(10).minutes.do(job)
来源：http://hz.vqdsnc.cn/gteotfddwh.html

[U37] Py：读写 Excel
来源：http://hz.xuetiantiany.cn/gtwolumhft.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gtznflozwy.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtnrvlufjd.html

Path(__file__).resolve().parent
来源：http://hz.yj20258888.top/gttkrgzhpw.html

[U39] Py：判断是否在交互环境
来源：http://hz.haohaochexian.top/gtugodjmsv.html

sys.stdout.isatty()
来源：http://hz.cdnleiting.top/gtpqilxehh.html

[U40] Py：打印到标准错误
来源：http://hz.nanxuanxn.top/gtudcaxtpi.html

print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtcuzbzlqb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.bjfxy.top/gttczffawt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sysykeji.top/gtaggvuxsl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj202588.top/gtckvvoaks.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hammf.cn/gtefzvxgqo.html

[U43] PHP：声明命名空间
来源：http://hz.jyoumei.cn/gteecgdccn.html

namespace App\Http;
来源：http://hz.gzhubu.top/gtultlmssa.html

[U44] PHP：开启严格类型
来源：http://hz.cashguo.top/gtwzpceumz.html

declare(strict_types=1);
来源：http://hz.jinyuanbaomall.cn/gtydhroktq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xylfe.cn/gtcheamadf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtzntyqozg.html

[U46] PHP：可空类型
来源：http://hz.hammf.cn/gtlkzeogst.html

?string $name = null
来源：http://hz.wangdashe.top/gtqmbhodtd.html

[U47] PHP：联合类型
来源：http://hz.aizwys.cn/gtjvmltdul.html

int|string $id
来源：http://hz.jinghuilouyu.cn/gtttxcrskz.html

[U48] PHP：纯枚举
来源：http://hz.shzxlz.cn/gtuolzbttp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydjk.org.cn/gtyfulpdbc.html

[U49] PHP：只读属性
来源：http://hz.zhijiandao.cn/gtsgzsuofa.html

public readonly string $name
来源：http://hz.zhongyouzk.top/gtacxattgw.html

[U50] PHP：构造器属性提升
来源：http://hz.nwbrower.top/gtenadphwo.html

public function __construct(private int $id) {}
来源：http://hz.c1oappe.top/gtaadybwwd.html

[U51] PHP：数组解构
来源：http://hz.dashuyun.cn/gtkpuylwdt.html

[$a, $b] = $arr;
来源：http://hz.wangshuangyany.cn/gtuwiiuupg.html

[U52] PHP：箭头函数
来源：http://hz.tanke756.top/gtkweasxcz.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxinkj.top/gtxrunbvun.html

[U53] PHP：空合并运算符
来源：http://hz.hysaishi.cn/gttpteenjm.html

$v = $a ?? $b ?? "default";
来源：http://hz.haohaochexian.top/gtyhxawsvk.html

[U54] PHP：空安全调用
来源：http://hz.mhx1999.top/gtbczytqag.html

$obj?->method()
来源：http://hz.sweek.top/gtkpexohqq.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtsqjmrfee.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gogol.net.cn/gtqlssczve.html

[U56] PHP：命名参数
来源：http://hz.aibaodan.cn/gtzyzrggvq.html

f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtfbjdfczy.html

[U57] PHP：字符串插值
来源：http://hz.smart0.xyz/gtnadumlse.html

"值: {$a}"
来源：http://hz.jinqigfzy.top/gtniqbdmcn.html

[U58] PHP：数组三件套
来源：http://hz.xziqi.cn/gtlvkixbco.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigfzy.top/gtrlfhydgi.html

[U59] PHP：自定义排序
来源：http://hz.yangfankeji.com/gtpuzwpwbo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuetiantiany.cn/gtvebgrkto.html

[U60] PHP：JSON 编解码
来源：http://hz.daria6918.cn/gtmkjhmuka.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhiwuduotai.top/gtemiyjtwb.html

[U61] PHP：正则
来源：http://hz.cashguo.top/gtywbtujbs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtfteviptb.html

[U62] PHP：日期对象
来源：http://hz.cdnleiting.top/gtrpqzvnvp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hnxiangtu.top/gtowwgpixb.html

[U63] PHP：文件读写
来源：http://hz.yj20258.top/gtkzfvliux.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.haohaochexian.top/gtobulxpzp.html

[U64] PHP：目录遍历
来源：http://hz.smart0.xyz/gtttbohxlr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.birdmap.top/gtqsszwcft.html

[U65] PHP：会话
来源：http://hz.ivvv.top/gtgtrnkert.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dashuyun.cn/gtjugzowvy.html

[U66] PHP：设置 Cookie
来源：http://hz.svipenyu.cn/gtyzqbvjdr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sufxvd.cn/gtnvqrqcul.html

[U67] PHP：处理文件上传
来源：http://hz.yuxming.cn/gtumcbckgk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xziqi.cn/gtpqachktj.html

[U68] PHP：PDO 连接
来源：http://hz.svipenyu.cn/gtpwwvrywp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangkeji.top/gtghfxohvg.html

[U69] PHP：PDO 预处理
来源：http://hz.52xcode.cn/gtmpvtboiu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.aibaodan.cn/gtarufhpxb.html

[U70] PHP：PDO 事务
来源：http://hz.meibo888.top/gtqpenxtpf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgfzy.top/gtbrrwacxn.html

[U71] PHP：抛出异常
来源：http://hz.yj20258888.top/gtlmlpunqd.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj20258888.top/gtpshptprf.html

[U72] PHP：写错误日志
来源：http://hz.xziqi.cn/gtekqfascy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yvedp.cn/gtjheduflt.html

[U73] PHP：读取 ini 配置
来源：http://hz.nanxinkj.top/gthzismzrd.html

parse_ini_file("config.ini", true)
来源：http://hz.xinyue.icu/gtyimyhbza.html

[U74] PHP：读取环境变量
来源：http://hz.hnqzz.top/gtcuyeqoef.html

getenv("APP_ENV") ?: "production"
来源：http://hz.fzhhl.top/gtkfppxije.html

[U75] PHP：依赖注入
来源：http://hz.hywenlv.cn/gttrbzbhfs.html

composer require psr/container
来源：http://hz.gaohongyu789.top/gtqdotqvxy.html

[U76] PHP：简单路由
来源：http://hz.nanxuanxn.top/gtoxnnyyjz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinqigufen.top/gtmtpepjcd.html

[U77] PHP：模板渲染
来源：http://hz.9152youxi.cn/gthzlbfieb.html

composer require twig/twig
来源：http://hz.cucudq.cn/gtyocgvjik.html

[U78] PHP：单元测试
来源：http://hz.nanxinkj.top/gtfnjkapql.html

composer require --dev phpunit/phpunit
来源：http://hz.shzxlz.cn/gtueukfdox.html

[U79] PHP：静态分析
来源：http://hz.cqqwz.cn/gtqcdzmvdy.html

composer require --dev phpstan/phpstan
来源：http://hz.ywan-chungtsiang.top/gtdgrqjxcq.html

[U80] PHP：代码规范修复
来源：http://hz.ivvv.top/gtwmhpvbjp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cucudq.cn/gteyahjrjf.html

[U81] JS：初始化项目
来源：http://hz.xziqi.cn/gtmhtstgeq.html

npm init -y;  npm i express
来源：http://hz.redwolf501.top/gttntxdekv.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtwwplgwfb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.wangshuangyany.cn/gtmeoehwpe.html

[U83] JS：ES Module 导入导出
来源：http://hz.guowangkeji.top/gtovpquzoz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenjidiqi.icu/gtftgilwxb.html

[U84] JS：CommonJS 写法
来源：http://hz.yonumen.top/gtbktuwhpd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hysaishi.cn/gtdsrpjbms.html

[U85] JS：可选链
来源：http://hz.gaohongyu789.top/gtwguggfsu.html

a?.b?.c
来源：http://hz.havefunace.top/gtkisuuger.html

[U86] JS：空值合并
来源：http://hz.zhijiandao.cn/gtplezpicr.html

a ?? b
来源：http://hz.xziqi.cn/gtnbgnmnhg.html

[U87] JS：解构默认值
来源：http://hz.hongshengwenyu.top/gtcivrqezq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuanzhike.top/gttactorey.html

[U88] JS：对象展开合并
来源：http://hz.quarkkingdee.top/gtwkhozckc.html

{ ...a, ...b }
来源：http://hz.hammf.cn/gtmizcarzd.html

[U89] JS：数组去重
来源：http://hz.ydjk.org.cn/gtwfqrdbqg.html

[...new Set(arr)]
来源：http://hz.hammf.cn/gtzotmyubc.html

[U90] JS：数字数组排序
来源：http://hz.zhixingplan.top/gtyxxnqthj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtewvzmiiz.html

[U91] JS：对象键值遍历
来源：http://hz.zdqjudy.top/gtqrmmtuur.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangshuangyany.cn/gttnkaxoef.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gteqtpqila.html

structuredClone(obj)
来源：http://hz.bjfxy.top/gtsouffxcv.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangkeji.top/gthvqffvpx.html

`共 ${n} 条`
来源：http://hz.ydjk.org.cn/gtgqdytnog.html

[U94] JS：箭头函数
来源：http://hz.shanyushiyangkeji.top/gtfrmrpryx.html

const double = x => x * 2;
来源：http://hz.9152youxi.cn/gtrkqjoyaw.html

[U95] JS：Promise 包装
来源：http://hz.hnqzz.top/gtlihpfhsx.html

new Promise((resolve, reject) => {})
来源：http://hz.zhoulong.xyz/gtnxqiunks.html

[U96] JS：async/await 与异常
来源：http://hz.shangyingyoupin.top/gtgpxujpgp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtjxosxjmp.html

[U97] JS：并发请求
来源：http://hz.jyoumei.cn/gttobehrqw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtqlijubaa.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhijiandao.cn/gtidaamolk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yanxiufei.cn/gtqaovakjh.html

[U99] JS：事件监听
来源：http://hz.jianghu66.top/gthmosnfkw.html

el.addEventListener("click", e => {})
来源：http://hz.yvedp.cn/gtimrjrnro.html

[U100] JS：DOM 查询
来源：http://hz.guannengcc.top/gtczxbwaiy.html

document.querySelector(".item")
来源：http://hz.haohaochexian.top/gtaliluyyd.html

[U101] JS：classList 操作
来源：http://hz.iojbl.cn/gtsmaorqjh.html

el.classList.toggle("active")
来源：http://hz.dianchejie.cn/gtfqwzfrms.html

[U102] JS：本地存储
来源：http://hz.jinqigufen.top/gtujzqhyqy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.wangdashe.top/gtwuonxqdg.html

[U103] JS：定时器
来源：http://hz.birdmap.top/gtwxcwdisf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhaomingkeji.xyz/gtfbvnluuj.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gtmgfexsoh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtkaodmgge.html

[U105] JS：节流
来源：http://hz.zhongyouzk.top/gtsbtxzrad.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhongyouzk.top/gtvbydhosi.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtwevudopq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.pengpengdd.cyou/gtzkkuzywd.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtxkyspxri.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cucudq.cn/gtloylnykx.html

[U108] JS：随机整数
来源：http://hz.daxiang520.top/gtidezygmg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gogol.net.cn/gtsgmqxarw.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtrihpbqda.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtysbkumiq.html

[U110] JS：数组分块
来源：http://hz.shanyushiyangtech.top/gteluryiwe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.havefunace.top/gtfmjryito.html

[U111] JS：对象转 Map
来源：http://hz.gaohongyu789.top/gtxdlimtlk.html

new Map(Object.entries(obj))
来源：http://hz.jqgufenzy.top/gtkjwytfvo.html

[U112] JS：字符串补位
来源：http://hz.cucudq.cn/gtsllzdsvp.html

"7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtbhcnpgzc.html

[U113] JS：正则替换全部
来源：http://hz.xylfe.cn/gthgimedtv.html

s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtvtbdedbx.html

[U114] JS：JSON 深比较
来源：http://hz.52xcode.cn/gtgzmpvhkr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtlgmbelsj.html

[U115] JS：生成 UUID
来源：http://hz.bjfxy.top/gtrcixtoel.html

crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtcdrjiase.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jyoumei.cn/gtsggthrqf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gtgqkgcvzm.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtagikutrs.html

npm i -D vitest;  npx vitest
来源：http://hz.sweek.top/gtdrilkomp.html

[U118] JS：开发服务器
来源：http://hz.chenjidiqi.icu/gtmsyhhkdw.html

npm i -D vite;  npx vite
来源：http://hz.cqqwz.cn/gtucfseizx.html

[U119] JS：生产构建
来源：http://hz.ybcxt.top/gtieakapcq.html

npx vite build
来源：http://hz.yanxiufei.cn/gtyuebyykm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.dianchejie.cn/gtgkmiruxn.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gtvaqdykak.html

================================================================================
来源：http://hz.xylfe.cn/gtrxynwsye.html

统计汇总
来源：http://hz.hnqzz.top/gtmyxbigps.html

================================================================================
来源：http://hz.gogol.net.cn/gtwmlikdga.html

按语言统计（条）：
来源：http://hz.yanxiufei.cn/gttbdnvmgs.html

Python ......... 252
来源：http://hz.ybcxt.top/gtqlzcyyad.html

PHP ............ 252
来源：http://hz.gaohongyu789.top/gtzjyrahxt.html

JavaScript ..... 252
来源：http://hz.dashuyun.cn/gtagdsaiog.html

TypeScript ..... 212
来源：http://hz.cashguo.top/gtheqjyfvj.html

Java ........... 212
来源：http://hz.nanxuanxn.top/gtkpxibvdz.html

Go ............. 212
来源：http://hz.zhiwuduotai.top/gtczeepmfx.html

Ruby ........... 212
来源：http://hz.hywenlv.cn/gtrggnivsy.html

C# ............. 212
来源：http://hz.redwolf501.top/gtmdmjuryq.html

C .............. 30
来源：http://hz.jinqigfzy.top/gtquireypd.html

C++ ............ 30
来源：http://hz.tanke756.top/gtwirkbueo.html

SQL ............ 90
来源：http://hz.52xcode.cn/gtychpzpmg.html

Bash ........... 80
来源：http://hz.dianchejie.cn/gtrdttuelf.html

Kotlin ......... 15
来源：http://hz.gaohongyu789.top/gtmrvidhci.html

Swift .......... 15
来源：http://hz.bjfxy.top/gtivyxnonu.html

Lua ............ 10
来源：http://hz.xziqi.cn/gtyqvwtffn.html

Perl ........... 10
来源：http://hz.52xcode.cn/gtisvpewck.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtojcbbnln.html

------------------------------------
来源：http://hz.0kj1m.cn/gtmzndvdlw.html

合计 ........... 2106 条
来源：http://hz.haohaochexian.top/gtqfedycnm.html

按章节统计：
来源：http://hz.zdqjudy.top/gtwekygscw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtyuntmiiw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtdyvwezmw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtryglfldo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yangfankeji.com/gtjaldwtqu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.guowangkeji.top/gtznqbxfre.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fengsongda.top/gtiiyoggag.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtwfhzbydt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gttbuqmwxz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtzcdxiwfh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ehwqpu.com/gtmqlfshvj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtxviwozvm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtbxxnrddh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtwhngjlup.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtbnypljke.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhengqikj.top/gtlcurleqf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtfasuvdkb.html

Q SQL 专题                              90
来源：http://hz.chenjidiqi.icu/gtilcckyfc.html

R Bash 专题                             80
来源：http://hz.quarkkingdee.top/gtwyjrsycf.html

S C / C++ 专题                          60
来源：http://hz.hnxiangtu.top/gtvkkmubms.html

T 其他语言补充                          60
来源：http://hz.birdmap.top/gtqzgkaltg.html

U 高频实用片段                         120
来源：http://hz.feifeiyinyue.top/gtfazfuebl.html

------------------------------------
来源：http://hz.mhx1999.top/gtwgttoxzz.html

合计                                  2106 条
来源：http://hz.wangshuangyany.cn/gtgpqmzrpa.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtnszozpxx.html

使用提醒
来源：http://hz.jyoumei.cn/gttszfcuwp.html

--------------------------------------------------------------------------------
来源：http://hz.daria6918.cn/gtqechaocp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xuetiantiany.cn/gtrxrxlxpd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nanxinkj.top/gtfgvrvsyx.html


<!-- 参考信息 -->