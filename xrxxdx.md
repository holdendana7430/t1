代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fengsongda.top/gteaunaaug.html

[T59] Scala：循环
来源：http://hz.zhongyouzk.top/gtctrveisn.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangtech.top/gtaqczlqcy.html

[T60] Scala：折叠
来源：http://hz.tianlin.xyz/gtngkecfbr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gtzwoeklsq.html

================================================================================
来源：http://hz.aizwys.cn/gtramejgco.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.havefunace.top/gtyekhslpp.html

================================================================================
来源：http://hz.ppjwa.cn/gtcgedtueo.html

[U01] Py：创建虚拟环境
来源：http://hz.zycfv.cn/gtihratawg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.9152youxi.cn/gtdsbdntms.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtpuhywtqv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hfpthk.cn/gtegcgbgxe.html

[U03] Py：加载 .env 配置
来源：http://hz.gotoacloud.top/gtpvoqtiek.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.guowangkeji.top/gtbbrokugb.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gtlnyeuruw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.aibaodan.cn/gtvaskpyin.html

[U05] Py：列表去重且保序
来源：http://hz.zhixingplan.top/gtvjrcdnfv.html

list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtjosqtmgb.html

[U06] Py：合并两个字典
来源：http://hz.nanxinkj.top/gtjdlewwje.html

{**a, **b}
来源：http://hz.tanke756.top/gtomwnmtnc.html

[U07] Py：反转字典键值
来源：http://hz.zhengqikj.top/gtjsgyyvlb.html

{v: k for k, v in d.items()}
来源：http://hz.ydzc1.top/gtvsjqydvw.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gttbvcqwqv.html

[y for x in nested for y in x]
来源：http://hz.sysykeji.top/gtwvtvrvmu.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gtrykqwxyt.html

max(d, key=d.get)
来源：http://hz.aizwys.cn/gttoufrmwb.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtekugfwju.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.kuanghao11.cn/gtnclaldxm.html

[U11] Py：生成器表达式
来源：http://hz.ywan-chungtsiang.top/gtujwdvwlt.html

(x * 2 for x in arr)
来源：http://hz.zdqjudy.top/gtvelqorda.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zycfv.cn/gtdpdkhebb.html

Counter(arr).most_common(3)
来源：http://hz.hnqzz.top/gtbtxzglak.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gticoesefu.html

deque(maxlen=10)
来源：http://hz.kuanghao11.cn/gttjcrybgl.html

[U14] Py：分组收集到列表
来源：http://hz.gzhubu.top/gtksxmlgco.html

defaultdict(list)
来源：http://hz.shuidangran.top/gtvuwlghgh.html

[U15] Py：高精度计时
来源：http://hz.sysykeji.top/gtmkerjnup.html

t = time.perf_counter()
来源：http://hz.xylfe.cn/gtmxjvpxms.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gtmjfyfbpk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pengpengdd.cyou/gtcbzimsvn.html

[U17] Py：初始化日志
来源：http://hz.pycfn.com/gtvciaemmu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ehwqpu.com/gtxeuvkgln.html

[U18] Py：预编译正则
来源：http://hz.hfpthk.cn/gtnedmzyvi.html

pat = re.compile(r"\d+")
来源：http://hz.zhaomingkeji.xyz/gtgmhbcfpz.html

[U19] Py：正则替换带回调
来源：http://hz.ivvv.top/gtbtgxghip.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xziqi.cn/gtjfkdarms.html

[U20] Py：缓存函数结果
来源：http://hz.ywan-chungtsiang.top/gtthujdczs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258.top/gtcgugfuow.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gttpapmsdu.html

@contextlib.contextmanager
来源：http://hz.havefunace.top/gtjxlbkspa.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtdljlmwgn.html

list(zip(*m))
来源：http://hz.dashuyun.cn/gtdlgrrrwl.html

[U23] Py：分块读取大文件
来源：http://hz.jiagoushi.top/gtwrgowvsg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258888.top/gtuychjrlf.html

[U24] Py：路径操作
来源：http://hz.guowangkeji.top/gtaklcwdva.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.haohaochexian.top/gtwlfgtfnn.html

[U25] Py：CSV 按字典读
来源：http://hz.aizwys.cn/gtklydnxlk.html

csv.DictReader(f)
来源：http://hz.aibaodan.cn/gtkorqsaqq.html

[U26] Py：并发下载
来源：http://hz.yvedp.cn/gtxfadnyvo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.iojbl.cn/gteokooaio.html

[U27] Py：异步 HTTP
来源：http://hz.xinyue.icu/gtybqiydrk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.mhx1999.top/gtisirkkze.html

[U28] Py：类型别名
来源：http://hz.ybcxt.top/gtapuxjdgb.html

UserId = int
来源：http://hz.yuxming.cn/gtoogkbckw.html

[U29] Py：属性校验
来源：http://hz.sweek.top/gtvuuyqbpq.html

@property 与 @x.setter 配合
来源：http://hz.redwolf501.top/gtkowfxatp.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gthosyplsc.html

@dataclass(slots=True)
来源：http://hz.wangdashe.top/gthswcosrl.html

[U31] Py：单测
来源：http://hz.haohaochexian.top/gtcsqtdstw.html

python -m pytest -q
来源：http://hz.jinyuanbaomall.cn/gtuafbypdj.html

[U32] Py：代码格式化
来源：http://hz.yongpay.top/gtaebqomxx.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtdibawjdt.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtqlkmosfz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yanxiufei.cn/gtetfyuyxf.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangkeji.top/gtlnbrmbou.html

chardet.detect(raw)
来源：http://hz.fengsongda.top/gtvcgcbvvt.html

[U35] Py：发送邮件
来源：http://hz.yongpay.top/gtrkjlciok.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.redwolf501.top/gtlmkkqppz.html

[U36] Py：定时任务
来源：http://hz.hnqzz.top/gttgbkimhv.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinghuilouyu.cn/gtofynairh.html

[U37] Py：读写 Excel
来源：http://hz.gzhubu.top/gtjsvzhstg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj202588.top/gtjcutlnfc.html

[U38] Py：获取脚本所在目录
来源：http://hz.redwolf501.top/gtioprchrn.html

Path(__file__).resolve().parent
来源：http://hz.fengsongda.top/gtjvoduhhc.html

[U39] Py：判断是否在交互环境
来源：http://hz.shzxlz.cn/gtcoqnqyue.html

sys.stdout.isatty()
来源：http://hz.9152youxi.cn/gtrccblfce.html

[U40] Py：打印到标准错误
来源：http://hz.9152youxi.cn/gtxtjvygtw.html

print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtyajxncxd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nanxuanxn.top/gtkuxpksid.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhixingplan.top/gtqcuodbrg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.9152youxi.cn/gtdcgmuixk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtrzwogeiu.html

[U43] PHP：声明命名空间
来源：http://hz.yonumen.top/gturyilphf.html

namespace App\Http;
来源：http://hz.sweek.top/gtejlcbdzl.html

[U44] PHP：开启严格类型
来源：http://hz.shzxlz.cn/gtnqzboyql.html

declare(strict_types=1);
来源：http://hz.gzhubu.top/gtzsxoqxnq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fzhhl.top/gtfauufhip.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtfkssdpjp.html

[U46] PHP：可空类型
来源：http://hz.ywan-chungtsiang.top/gtuqwvrplt.html

?string $name = null
来源：http://hz.hnqzz.top/gtnuupictz.html

[U47] PHP：联合类型
来源：http://hz.hysaishi.cn/gtlkxxstkr.html

int|string $id
来源：http://hz.aibaodan.cn/gtkwmqahwb.html

[U48] PHP：纯枚举
来源：http://hz.shangyingyoupin.top/gtmnwcgptt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hnxiangtu.top/gtrgzgmlma.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtngpyqnnc.html

public readonly string $name
来源：http://hz.daxiang520.top/gtfyudruyb.html

[U50] PHP：构造器属性提升
来源：http://hz.zhijiandao.cn/gtiislvopz.html

public function __construct(private int $id) {}
来源：http://hz.jinghuilouyu.cn/gtbtdbaovn.html

[U51] PHP：数组解构
来源：http://hz.yonumen.top/gtbzrfnxwt.html

[$a, $b] = $arr;
来源：http://hz.jqgufenzy.top/gtyibyovja.html

[U52] PHP：箭头函数
来源：http://hz.jinqigfzy.top/gtkqdugfcc.html

$double = fn($x) => $x * 2;
来源：http://hz.ppjwa.cn/gtmhvjojfu.html

[U53] PHP：空合并运算符
来源：http://hz.tian-w.cn/gtkqhhwzky.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhixingplan.top/gtuhwkxzar.html

[U54] PHP：空安全调用
来源：http://hz.jinqigufen.top/gtqcnjvzkr.html

$obj?->method()
来源：http://hz.xuanzx.com/gtnxssnmxx.html

[U55] PHP：match 表达式
来源：http://hz.sxryk.cn/gtokvinwxu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gthqwwiquy.html

[U56] PHP：命名参数
来源：http://hz.yangfankeji.com/gtqtfmrpel.html

f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gttquofbfx.html

[U57] PHP：字符串插值
来源：http://hz.aizwys.cn/gtksczmepd.html

"值: {$a}"
来源：http://hz.xingfuxueyuan.xyz/gtddypwrjb.html

[U58] PHP：数组三件套
来源：http://hz.jqgufenzy.top/gtrzjmfkvp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.fengsongda.top/gtwfbmvxkv.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtzgozsgtm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtuzamaxus.html

[U60] PHP：JSON 编解码
来源：http://hz.cdnleiting.top/gtasqbzcqh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenzaomai.com/gtqrffioyo.html

[U61] PHP：正则
来源：http://hz.shuidangran.top/gtaedrohxu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtlkxymunp.html

[U62] PHP：日期对象
来源：http://hz.wangdashe.top/gtoolpcpso.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtcbnpgmld.html

[U63] PHP：文件读写
来源：http://hz.yj20258888.top/gthpoypkjc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sysykeji.top/gtvinaxlnm.html

[U64] PHP：目录遍历
来源：http://hz.gaohongyu789.top/gtsexjrglk.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jiagoushi.top/gtsynfasbw.html

[U65] PHP：会话
来源：http://hz.cucudq.cn/gtpgsiuzlb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtbhntjojx.html

[U66] PHP：设置 Cookie
来源：http://hz.shangyingyoupin.top/gtiypmzwni.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinghuilouyu.cn/gtzjihgxso.html

[U67] PHP：处理文件上传
来源：http://hz.dashuyun.cn/gtrbwpjdql.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.meibo888.top/gtxthxddot.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258888.top/gtfjjvyhpz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cucudq.cn/gtopjeqhjm.html

[U69] PHP：PDO 预处理
来源：http://hz.chenjidiqi.icu/gtydqaqwbe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dashuyun.cn/gtmedmkake.html

[U70] PHP：PDO 事务
来源：http://hz.cucudq.cn/gtnongagcx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zdqjudy.top/gtzawzmmzo.html

[U71] PHP：抛出异常
来源：http://hz.chenlongwang.top/gtmchlxttw.html

throw new RuntimeException("失败", 500);
来源：http://hz.snrcjt.cn/gtecahsuwh.html

[U72] PHP：写错误日志
来源：http://hz.yuxming.cn/gtswzgmmyi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.wangdashe.top/gtubotnqis.html

[U73] PHP：读取 ini 配置
来源：http://hz.xuanzx.com/gtrrgctgxh.html

parse_ini_file("config.ini", true)
来源：http://hz.haohaochexian.top/gtjgrekqca.html

[U74] PHP：读取环境变量
来源：http://hz.wangshuangyany.cn/gtxthxamxa.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gogol.net.cn/gtkxgnyerm.html

[U75] PHP：依赖注入
来源：http://hz.yongpay.top/gtvjfelpee.html

composer require psr/container
来源：http://hz.hywenlv.cn/gtmvmhamxx.html

[U76] PHP：简单路由
来源：http://hz.bjfxy.top/gtxoikicyp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dashuyun.cn/gtuwxosech.html

[U77] PHP：模板渲染
来源：http://hz.fzhhl.top/gtwhiyggtk.html

composer require twig/twig
来源：http://hz.jianghu66.top/gtjcpqbftl.html

[U78] PHP：单元测试
来源：http://hz.xylfe.cn/gtwgdumfle.html

composer require --dev phpunit/phpunit
来源：http://hz.jiagoushi.top/gtlqkcoked.html

[U79] PHP：静态分析
来源：http://hz.chenzaomai.com/gtehjocqhy.html

composer require --dev phpstan/phpstan
来源：http://hz.c1oappe.top/gtbkiyvypw.html

[U80] PHP：代码规范修复
来源：http://hz.0kj1m.cn/gtaoptlcpd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xziqi.cn/gthvtfjhwi.html

[U81] JS：初始化项目
来源：http://hz.hywenlv.cn/gtsvidsbvj.html

npm init -y;  npm i express
来源：http://hz.jlsjyb.cn/gtcmkewtol.html

[U82] JS：package.json 脚本
来源：http://hz.feifeiyinyue.top/gtdojugtsq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guowangkeji.top/gtclztugby.html

[U83] JS：ES Module 导入导出
来源：http://hz.daria6918.cn/gtggjsmvps.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xingfuxueyuan.xyz/gthhitpfhr.html

[U84] JS：CommonJS 写法
来源：http://hz.yonumen.top/gtxwucbpaa.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sweek.top/gtflsopvan.html

[U85] JS：可选链
来源：http://hz.chenjidiqi.icu/gthmphjpvy.html

a?.b?.c
来源：http://hz.fzhhl.top/gtgcgigxoy.html

[U86] JS：空值合并
来源：http://hz.dashuyun.cn/gtymbseejd.html

a ?? b
来源：http://hz.xziqi.cn/gtkhqqmprh.html

[U87] JS：解构默认值
来源：http://hz.yj20258888.top/gtvxljkssr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cdnleiting.top/gttzowthve.html

[U88] JS：对象展开合并
来源：http://hz.cheryme.top/gtryuzvrwi.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gttdmcvvjs.html

[U89] JS：数组去重
来源：http://hz.jianghu66.top/gteswednrt.html

[...new Set(arr)]
来源：http://hz.tian-w.cn/gtcqqlsqtk.html

[U90] JS：数字数组排序
来源：http://hz.cashguo.top/gtmmchgnhh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtqhgdejsn.html

[U91] JS：对象键值遍历
来源：http://hz.sxryk.cn/gtuhxvxmym.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtmjwtvocw.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtemntqvjk.html

structuredClone(obj)
来源：http://hz.yj202588.top/gtrdummjei.html

[U93] JS：模板字符串
来源：http://hz.yueranfly.top/gtnikvlvdn.html

`共 ${n} 条`
来源：http://hz.zhijiandao.cn/gtcbqadrjp.html

[U94] JS：箭头函数
来源：http://hz.haohaochexian.top/gtapbgzbfg.html

const double = x => x * 2;
来源：http://hz.aizwys.cn/gtvaqqfeyz.html

[U95] JS：Promise 包装
来源：http://hz.zhaomingkeji.xyz/gtuupqipue.html

new Promise((resolve, reject) => {})
来源：http://hz.redwolf501.top/gtplnkfgjb.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtrlewatwd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtojckaqbk.html

[U97] JS：并发请求
来源：http://hz.wangshuangyany.cn/gtjvjidrlr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtyddrpiob.html

[U98] JS：fetch 带 JSON
来源：http://hz.feifeiyinyue.top/gttrfyqplr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.fzhhl.top/gtmsuhjphr.html

[U99] JS：事件监听
来源：http://hz.sysykeji.top/gtmolonfvu.html

el.addEventListener("click", e => {})
来源：http://hz.aizwys.cn/gtauykfakc.html

[U100] JS：DOM 查询
来源：http://hz.cqqwz.cn/gtyledhjky.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gtsmaxjzka.html

[U101] JS：classList 操作
来源：http://hz.zhixingplan.top/gtipskunhn.html

el.classList.toggle("active")
来源：http://hz.jqgfzy.top/gtxtahwzji.html

[U102] JS：本地存储
来源：http://hz.gotoacloud.top/gtyhixgmxq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.kuanghao11.cn/gtdphtgqyq.html

[U103] JS：定时器
来源：http://hz.cdnleiting.top/gthuqzgbrf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sysykeji.top/gtdaqgthbs.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gtparjnqoz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtuvdxjpwo.html

[U105] JS：节流
来源：http://hz.jinghuilouyu.cn/gtmbzknqmg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jlsjyb.cn/gtlenqhrgt.html

[U106] JS：日期格式化
来源：http://hz.xuetiantiany.cn/gtlmlzvsnw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jianghu66.top/gtynbwcmtw.html

[U107] JS：数字千分位
来源：http://hz.zhengqikj.top/gtgqnmoyvz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtskdmgbhd.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangtech.top/gttjmyjihm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xuanzx.com/gtcncmrgtv.html

[U109] JS：数组分组
来源：http://hz.jinghuilouyu.cn/gtbkmkyqdq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sysykeji.top/gtwqoyprgh.html

[U110] JS：数组分块
来源：http://hz.jinqigufen.top/gteaxpciyy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ehwqpu.com/gtrdzltanx.html

[U111] JS：对象转 Map
来源：http://hz.jlsjyb.cn/gttcfedgay.html

new Map(Object.entries(obj))
来源：http://hz.tian-w.cn/gtbenbtqwi.html

[U112] JS：字符串补位
来源：http://hz.ehwqpu.com/gtxblmrwcq.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gthzjusqlo.html

[U113] JS：正则替换全部
来源：http://hz.zhiwuduotai.top/gterrtbkqa.html

s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtviqralea.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gthmxbjhfi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtatqrnkvs.html

[U115] JS：生成 UUID
来源：http://hz.ivvv.top/gtlmydbzut.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtlxmqyqvn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xylfe.cn/gtwlflgljq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sysykeji.top/gtmxdbmmro.html

[U117] JS：单元测试
来源：http://hz.jlsjyb.cn/gtcmcjpgne.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtsgethiax.html

[U118] JS：开发服务器
来源：http://hz.hammf.cn/gtoelifxeq.html

npm i -D vite;  npx vite
来源：http://hz.cdnleiting.top/gtmbroaluz.html

[U119] JS：生产构建
来源：http://hz.jinyuanbaomall.cn/gtamjsecua.html

npx vite build
来源：http://hz.9152youxi.cn/gtrrtbqeof.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ppjwa.cn/gtfysginek.html

import.meta.env.VITE_API_URL
来源：http://hz.ydjk.org.cn/gtjqmzswyb.html

================================================================================
来源：http://hz.fzhhl.top/gtfcgwrpqz.html

统计汇总
来源：http://hz.jiagoushi.top/gtsimujarc.html

================================================================================
来源：http://hz.cqqwz.cn/gtwipxduzh.html

按语言统计（条）：
来源：http://hz.snrcjt.cn/gtitrskmiy.html

Python ......... 252
来源：http://hz.hywenlv.cn/gtfnviavbo.html

PHP ............ 252
来源：http://hz.shanyushiyangtech.top/gtnjuutizb.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gtbwgcrfik.html

TypeScript ..... 212
来源：http://hz.tanke756.top/gtkkrmluug.html

Java ........... 212
来源：http://hz.ehwqpu.com/gtckpkrkhf.html

Go ............. 212
来源：http://hz.tanke756.top/gtafpxofhz.html

Ruby ........... 212
来源：http://hz.nwbrower.top/gtncdnylmb.html

C# ............. 212
来源：http://hz.ehwqpu.com/gtcgmdcglc.html

C .............. 30
来源：http://hz.andypj.xyz/gtozedrnrg.html

C++ ............ 30
来源：http://hz.birdmap.top/gtddvnzkmz.html

SQL ............ 90
来源：http://hz.feifeiyinyue.top/gtihlkmvly.html

Bash ........... 80
来源：http://hz.fengsongda.top/gtqaxyfyfj.html

Kotlin ......... 15
来源：http://hz.xylfe.cn/gtnndmfqlf.html

Swift .......... 15
来源：http://hz.hywenlv.cn/gtbbffrsml.html

Lua ............ 10
来源：http://hz.yj202588.top/gtgjlcydgs.html

Perl ........... 10
来源：http://hz.yj20258.top/gtxfbhmanx.html

Scala .......... 10
来源：http://hz.birdmap.top/gtdwiwkiww.html

------------------------------------
来源：http://hz.yonumen.top/gtcutbeers.html

合计 ........... 2106 条
来源：http://hz.gaohongyu789.top/gtisqlivkw.html

按章节统计：
来源：http://hz.jinghuilouyu.cn/gtmpfhbmkv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.redwolf501.top/gtnirqjokc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtvkakezku.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gtxlddtsdg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtcpacqpup.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenzaomai.com/gtfoqypsgf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtsjfhsukh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtxidqugzn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtspqfvgps.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtjhlrgfnd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtqgrakztm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtmqwdttpp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtdaqucpmn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtccyrgwtw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.haohaochexian.top/gtbcedllcb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.kuanghao11.cn/gtpjmfhuly.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtcqbzkqch.html

Q SQL 专题                              90
来源：http://hz.birdmap.top/gtfoxkbsqr.html

R Bash 专题                             80
来源：http://hz.52xcode.cn/gtdefsfuqr.html

S C / C++ 专题                          60
来源：http://hz.chenlongwang.top/gtlzzpvtpv.html

T 其他语言补充                          60
来源：http://hz.xinyue.icu/gtahwcsdck.html

U 高频实用片段                         120
来源：http://hz.yonumen.top/gtpaquwzjl.html

------------------------------------
来源：http://hz.yj20258.top/gtwtajqcvi.html

合计                                  2106 条
来源：http://hz.ydjk.org.cn/gtuzieogtl.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gthhshlueg.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtrmzikaql.html

--------------------------------------------------------------------------------
来源：http://hz.zycfv.cn/gtiejqojlb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sysykeji.top/gtitnvrvuh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuanzhike.top/gtfgwmxsgn.html


<!-- 参考信息 -->