代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.andypj.xyz/gtpkmxinvy.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gtcwukyhpe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnqzz.top/gtpfqyrdrf.html

[T58] Scala：函数定义
来源：http://hz.nanxinkj.top/gtctqvnvmd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sweek.top/gttoqtxkjr.html

[T59] Scala：循环
来源：http://hz.sysykeji.top/gtetocnszc.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinqigfzy.top/gtzpmaiagq.html

[T60] Scala：折叠
来源：http://hz.gotoacloud.top/gtodaumvpa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.quarkkingdee.top/gtrubmrcsm.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbdndtvvr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtnxthfcup.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtzuxpvluf.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtbddzbowl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtpjljxnqo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxuanxn.top/gtfgcuxcgt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shangyingyoupin.top/gtvnfjxmaj.html

[U03] Py：加载 .env 配置
来源：http://hz.jlsjyb.cn/gtxvdihddk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sysykeji.top/gtucanapjd.html

[U04] Py：变量调试打印
来源：http://hz.iojbl.cn/gtgzrwglar.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtdtckgvfw.html

[U05] Py：列表去重且保序
来源：http://hz.birdmap.top/gtoatfsweq.html

list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtixmgasoq.html

[U06] Py：合并两个字典
来源：http://hz.cheryme.top/gtbnhdyhbl.html

{**a, **b}
来源：http://hz.zdqjudy.top/gtatpaumda.html

[U07] Py：反转字典键值
来源：http://hz.shuidangran.top/gtxowrkwih.html

{v: k for k, v in d.items()}
来源：http://hz.ppjwa.cn/gtnudggudl.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtmrzydrai.html

[y for x in nested for y in x]
来源：http://hz.jlsjyb.cn/gtoccemnii.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtlrprbcyz.html

max(d, key=d.get)
来源：http://hz.mhx1999.top/gtkgtexhei.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gtnhgafgdy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tanke756.top/gtiqxqrais.html

[U11] Py：生成器表达式
来源：http://hz.guowangkeji.top/gtrdlnpvve.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtlkkabrti.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hysaishi.cn/gtvnsktdix.html

Counter(arr).most_common(3)
来源：http://hz.zhaomingkeji.xyz/gtsbgcxjoi.html

[U13] Py：固定长度队列
来源：http://hz.haohaochexian.top/gtyoswfrqn.html

deque(maxlen=10)
来源：http://hz.ybcxt.top/gtnkpaehtl.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtsnfjlgsa.html

defaultdict(list)
来源：http://hz.tianlin.xyz/gtycvtumys.html

[U15] Py：高精度计时
来源：http://hz.guowangkeji.top/gttdytzhtb.html

t = time.perf_counter()
来源：http://hz.yueranfly.top/gtxvxnmxif.html

[U16] Py：命令行参数解析
来源：http://hz.svipenyu.cn/gtkumvtnob.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xingfuxueyuan.xyz/gtnomrnsoy.html

[U17] Py：初始化日志
来源：http://hz.yj202588.top/gthoxiutxq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.0kj1m.cn/gtcglsvfpc.html

[U18] Py：预编译正则
来源：http://hz.gzhubu.top/gtkjiaryov.html

pat = re.compile(r"\d+")
来源：http://hz.9152youxi.cn/gtjgisdbcu.html

[U19] Py：正则替换带回调
来源：http://hz.nanxuanxn.top/gtpbzndzky.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnqzz.top/gtxjvzzkjg.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtqvyrbgek.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jlsjyb.cn/gtkqgvbnxi.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gtfhplkkjw.html

@contextlib.contextmanager
来源：http://hz.hongshengwenyu.top/gtihngvfow.html

[U22] Py：矩阵转置
来源：http://hz.hongshengwenyu.top/gtcsnosdax.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtdiigameh.html

[U23] Py：分块读取大文件
来源：http://hz.fengsongda.top/gtuvdblnxg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258888.top/gtkmakoigc.html

[U24] Py：路径操作
来源：http://hz.fengsongda.top/gtipeoyhky.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtewwgpjuk.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtztrdumoc.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtlxvoyyqa.html

[U26] Py：并发下载
来源：http://hz.316326.xyz/gtbfoexkoo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtijsaheba.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtcypdfntk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xinyue.icu/gtgauhdido.html

[U28] Py：类型别名
来源：http://hz.zhaomingkeji.xyz/gtmxjwhszc.html

UserId = int
来源：http://hz.yuxming.cn/gtaxmfwkfy.html

[U29] Py：属性校验
来源：http://hz.nanxuanxn.top/gtwqtdgsfu.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtbivzkmex.html

[U30] Py：数据类
来源：http://hz.9152youxi.cn/gtmetizkfc.html

@dataclass(slots=True)
来源：http://hz.yvedp.cn/gtleyyjvzr.html

[U31] Py：单测
来源：http://hz.zhijiandao.cn/gtjtsqsxbu.html

python -m pytest -q
来源：http://hz.bjfxy.top/gtznctplbk.html

[U32] Py：代码格式化
来源：http://hz.zhaomingkeji.xyz/gtmruzafuu.html

ruff format . && ruff check --fix .
来源：http://hz.gaohongyu789.top/gtdaiiyybb.html

[U33] Py：打包发布
来源：http://hz.cqqwz.cn/gtznzizkwf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shanyushiyangkeji.top/gtcefnvosd.html

[U34] Py：判断编码
来源：http://hz.pengpengdd.cyou/gtgcusbelr.html

chardet.detect(raw)
来源：http://hz.cqqwz.cn/gtoxrefrwm.html

[U35] Py：发送邮件
来源：http://hz.shuidangran.top/gtkfhfecrj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tian-w.cn/gtkfamfqrs.html

[U36] Py：定时任务
来源：http://hz.hongshengwenyu.top/gtcmdcuqdd.html

schedule.every(10).minutes.do(job)
来源：http://hz.ehwqpu.com/gtuqobdtrw.html

[U37] Py：读写 Excel
来源：http://hz.gaohongyu789.top/gtvxzzdkza.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shuidangran.top/gtuosykfli.html

[U38] Py：获取脚本所在目录
来源：http://hz.iojbl.cn/gtmtqacdcm.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gttvapfknh.html

[U39] Py：判断是否在交互环境
来源：http://hz.yuxming.cn/gtoxtqhrun.html

sys.stdout.isatty()
来源：http://hz.ybcxt.top/gtiqxheqhj.html

[U40] Py：打印到标准错误
来源：http://hz.ehwqpu.com/gtlrgdqjyh.html

print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtzoiyuhtu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shuidangran.top/gtatfsfzcx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jyoumei.cn/gtanalxvly.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.316326.xyz/gtgylxuabt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sysykeji.top/gtaufqkcir.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtxqiyhvgu.html

namespace App\Http;
来源：http://hz.sysykeji.top/gtlfznvjnt.html

[U44] PHP：开启严格类型
来源：http://hz.xylfe.cn/gtpvubymwf.html

declare(strict_types=1);
来源：http://hz.jqgufenzy.top/gtkzyvfsmo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cucudq.cn/gtxtalsnmr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtjecvswod.html

[U46] PHP：可空类型
来源：http://hz.cdnleiting.top/gtfijejznc.html

?string $name = null
来源：http://hz.xuanzx.com/gtwpbwzjtn.html

[U47] PHP：联合类型
来源：http://hz.redwolf501.top/gturssnkuf.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtzmoayyjf.html

[U48] PHP：纯枚举
来源：http://hz.yangfankeji.com/gtofgunrfm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtbygpopey.html

[U49] PHP：只读属性
来源：http://hz.hnqzz.top/gtubjxgfls.html

public readonly string $name
来源：http://hz.zycfv.cn/gtliyfcvnn.html

[U50] PHP：构造器属性提升
来源：http://hz.zhaomingkeji.xyz/gtldlujphb.html

public function __construct(private int $id) {}
来源：http://hz.xuetiantiany.cn/gtqqrbhgzg.html

[U51] PHP：数组解构
来源：http://hz.ehwqpu.com/gtlkxvboim.html

[$a, $b] = $arr;
来源：http://hz.shanyushiyangtech.top/gtxhknydjr.html

[U52] PHP：箭头函数
来源：http://hz.yangfankeji.com/gtnfyhepvw.html

$double = fn($x) => $x * 2;
来源：http://hz.xylfe.cn/gtkncmvbag.html

[U53] PHP：空合并运算符
来源：http://hz.zycfv.cn/gtrlxadgiv.html

$v = $a ?? $b ?? "default";
来源：http://hz.shuidangran.top/gtbbfxirjl.html

[U54] PHP：空安全调用
来源：http://hz.yuxming.cn/gtireqzutq.html

$obj?->method()
来源：http://hz.jinyuanbaomall.cn/gtjcpubkjf.html

[U55] PHP：match 表达式
来源：http://hz.svipenyu.cn/gtfuwegjae.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shanyushiyangkeji.top/gtaewrrclu.html

[U56] PHP：命名参数
来源：http://hz.dashuyun.cn/gtxdnrjxgd.html

f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtemrujglk.html

[U57] PHP：字符串插值
来源：http://hz.zhiwuduotai.top/gtifntvubf.html

"值: {$a}"
来源：http://hz.cucudq.cn/gtrookicjc.html

[U58] PHP：数组三件套
来源：http://hz.jinghuilouyu.cn/gtnzkfjvyp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jianghu66.top/gttefntlrw.html

[U59] PHP：自定义排序
来源：http://hz.jianghu66.top/gtzypmywmr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gthkyiakss.html

[U60] PHP：JSON 编解码
来源：http://hz.ybcxt.top/gtocyopygq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shanyushiyangtech.top/gtqldcyjkf.html

[U61] PHP：正则
来源：http://hz.cashguo.top/gtisgywmbe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gtvironvfq.html

[U62] PHP：日期对象
来源：http://hz.zdqjudy.top/gtqezgnaon.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nwbrower.top/gtxgnsnbda.html

[U63] PHP：文件读写
来源：http://hz.yuxming.cn/gtcctmvczw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aibaodan.cn/gttbidhhzo.html

[U64] PHP：目录遍历
来源：http://hz.sxryk.cn/gtitzljrqn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tianlin.xyz/gtloifegom.html

[U65] PHP：会话
来源：http://hz.svipenyu.cn/gtxzbycprg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gtnfeifqvd.html

[U66] PHP：设置 Cookie
来源：http://hz.gzhubu.top/gtsqxlylsu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnqzz.top/gtgdemwpnh.html

[U67] PHP：处理文件上传
来源：http://hz.iojbl.cn/gtafkbjngc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gzhubu.top/gttpmcdtyo.html

[U68] PHP：PDO 连接
来源：http://hz.ydzc1.top/gtaaccegke.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yvedp.cn/gtqlmekqoj.html

[U69] PHP：PDO 预处理
来源：http://hz.zhongyouzk.top/gtszlzojsh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gtvvxaqaao.html

[U70] PHP：PDO 事务
来源：http://hz.pycfn.com/gtqywtkekz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.redwolf501.top/gtuppuravv.html

[U71] PHP：抛出异常
来源：http://hz.andypj.xyz/gtfztriltz.html

throw new RuntimeException("失败", 500);
来源：http://hz.ivvv.top/gtmtjxwsck.html

[U72] PHP：写错误日志
来源：http://hz.ydjk.org.cn/gtineikrwm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yvedp.cn/gtmoxwscwv.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhaomingkeji.xyz/gtkacxtzcc.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtoancvked.html

[U74] PHP：读取环境变量
来源：http://hz.zhixingplan.top/gtwjwtolvp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtwuogvuqk.html

[U75] PHP：依赖注入
来源：http://hz.mhx1999.top/gtzegxjtjk.html

composer require psr/container
来源：http://hz.xuetiantiany.cn/gtmjkehodk.html

[U76] PHP：简单路由
来源：http://hz.nanxinkj.top/gtcgizrtoy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gzhubu.top/gtvrdzzrcl.html

[U77] PHP：模板渲染
来源：http://hz.hywenlv.cn/gtxnyxkgzo.html

composer require twig/twig
来源：http://hz.0kj1m.cn/gtvwqgoxpr.html

[U78] PHP：单元测试
来源：http://hz.iojbl.cn/gtswyuveew.html

composer require --dev phpunit/phpunit
来源：http://hz.aizwys.cn/gtyeyhwqrj.html

[U79] PHP：静态分析
来源：http://hz.yueranfly.top/gtcstjppxd.html

composer require --dev phpstan/phpstan
来源：http://hz.jiagoushi.top/gtrsobtlqp.html

[U80] PHP：代码规范修复
来源：http://hz.jyoumei.cn/gtbwgwqyxm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jyoumei.cn/gtujmokfvb.html

[U81] JS：初始化项目
来源：http://hz.yongpay.top/gtkeiplqwo.html

npm init -y;  npm i express
来源：http://hz.kuanghao11.cn/gtyevxastn.html

[U82] JS：package.json 脚本
来源：http://hz.jiagoushi.top/gtfzytgqgq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yongpay.top/gtvfnqaaef.html

[U83] JS：ES Module 导入导出
来源：http://hz.316326.xyz/gtsidgkrii.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.9152youxi.cn/gtaxmcgshh.html

[U84] JS：CommonJS 写法
来源：http://hz.zdqjudy.top/gtdzqavspf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.fzhhl.top/gtkpkqqhlg.html

[U85] JS：可选链
来源：http://hz.jinqigfzy.top/gtgfjhktkk.html

a?.b?.c
来源：http://hz.zdqjudy.top/gtevmkzain.html

[U86] JS：空值合并
来源：http://hz.daria6918.cn/gtelcdccbr.html

a ?? b
来源：http://hz.yj20258888.top/gtegonpiqm.html

[U87] JS：解构默认值
来源：http://hz.havefunace.top/gttoapvwpb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hywenlv.cn/gtyqqirifu.html

[U88] JS：对象展开合并
来源：http://hz.tian-w.cn/gtpmteckvu.html

{ ...a, ...b }
来源：http://hz.hnqzz.top/gtmjjnfvwh.html

[U89] JS：数组去重
来源：http://hz.daxiang520.top/gtrhonywjf.html

[...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtiyzlkwyd.html

[U90] JS：数字数组排序
来源：http://hz.0kj1m.cn/gthofzrizz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtujrzzpzv.html

[U91] JS：对象键值遍历
来源：http://hz.vqdsnc.cn/gtbxhqpdxk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgufenzy.top/gtghinureg.html

[U92] JS：深拷贝
来源：http://hz.gaohongyu789.top/gtjryhxgtl.html

structuredClone(obj)
来源：http://hz.jianghu66.top/gtzzxccnfs.html

[U93] JS：模板字符串
来源：http://hz.svipenyu.cn/gtmqrajbac.html

`共 ${n} 条`
来源：http://hz.aizwys.cn/gtscjolegf.html

[U94] JS：箭头函数
来源：http://hz.fzhhl.top/gtklplnxgm.html

const double = x => x * 2;
来源：http://hz.vqdsnc.cn/gtczbhqquy.html

[U95] JS：Promise 包装
来源：http://hz.ivvv.top/gttxawvjez.html

new Promise((resolve, reject) => {})
来源：http://hz.yj20258888.top/gtsrqmssjr.html

[U96] JS：async/await 与异常
来源：http://hz.hnxiangtu.top/gtnqutrgbn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtsbgmdaea.html

[U97] JS：并发请求
来源：http://hz.vqdsnc.cn/gtiumbyaud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtpwxhjihs.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangshuangyany.cn/gtyxuvjphx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daxiang520.top/gtwimwnljf.html

[U99] JS：事件监听
来源：http://hz.bjfxy.top/gtixhckyyd.html

el.addEventListener("click", e => {})
来源：http://hz.sweek.top/gtjhtrhoex.html

[U100] JS：DOM 查询
来源：http://hz.cqqwz.cn/gtkcrxlpcj.html

document.querySelector(".item")
来源：http://hz.zhongyouzk.top/gtrhxkzxok.html

[U101] JS：classList 操作
来源：http://hz.nanxuanxn.top/gtsmefoese.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangkeji.top/gtsncfthmj.html

[U102] JS：本地存储
来源：http://hz.pengpengdd.cyou/gteinykvmz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.iojbl.cn/gtsfgtjqjz.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtlvuxggwb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuanzhike.top/gtsdbiichq.html

[U104] JS：防抖
来源：http://hz.c1oappe.top/gtorhnbpyn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtpmtckicc.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtoprbgjgz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gogol.net.cn/gtfddeszif.html

[U106] JS：日期格式化
来源：http://hz.zhaomingkeji.xyz/gtmihvnzow.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ppjwa.cn/gtqtnecuqt.html

[U107] JS：数字千分位
来源：http://hz.zhiwuduotai.top/gtuodzpwkg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtmqipmmfc.html

[U108] JS：随机整数
来源：http://hz.guannengcc.top/gtjjjslcfv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.pengpengdd.cyou/gtideqqxnf.html

[U109] JS：数组分组
来源：http://hz.hywenlv.cn/gtqnprbxja.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gtkfxkmrok.html

[U110] JS：数组分块
来源：http://hz.smart0.xyz/gtwpxvhbjf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuxming.cn/gtzozcbote.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtpbbikjtk.html

new Map(Object.entries(obj))
来源：http://hz.ivvv.top/gtmjehwdnb.html

[U112] JS：字符串补位
来源：http://hz.zhiwuduotai.top/gtgbumuswc.html

"7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtowkkfscr.html

[U113] JS：正则替换全部
来源：http://hz.yuanzhike.top/gtbhgqjxiq.html

s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gttwtfxazz.html

[U114] JS：JSON 深比较
来源：http://hz.mhx1999.top/gtxarhohsm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtefugldkb.html

[U115] JS：生成 UUID
来源：http://hz.shzxlz.cn/gtygoqdshm.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtehnifszp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xziqi.cn/gtgpmdjfij.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhijiandao.cn/gtbuksojin.html

[U117] JS：单元测试
来源：http://hz.xziqi.cn/gtfhggqqji.html

npm i -D vitest;  npx vitest
来源：http://hz.fengsongda.top/gtejyjigqy.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtddxegemx.html

npm i -D vite;  npx vite
来源：http://hz.smart0.xyz/gtagrkuixh.html

[U119] JS：生产构建
来源：http://hz.ybcxt.top/gtnjjqqatw.html

npx vite build
来源：http://hz.iojbl.cn/gtjodbmswq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj202588.top/gtuzykivuj.html

import.meta.env.VITE_API_URL
来源：http://hz.zycfv.cn/gtuaegfany.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqotlwrve.html

统计汇总
来源：http://hz.shanyushiyangkeji.top/gtdjlpttta.html

================================================================================
来源：http://hz.sufxvd.cn/gtjwzyvumg.html

按语言统计（条）：
来源：http://hz.chenzaomai.com/gtdffzvdew.html

Python ......... 252
来源：http://hz.yuxming.cn/gtdtfcjbek.html

PHP ............ 252
来源：http://hz.ehwqpu.com/gtvjupapdq.html

JavaScript ..... 252
来源：http://hz.xziqi.cn/gtfuqhjhbj.html

TypeScript ..... 212
来源：http://hz.xingfuxueyuan.xyz/gtzhkozeza.html

Java ........... 212
来源：http://hz.gotoacloud.top/gtnortekpt.html

Go ............. 212
来源：http://hz.svipenyu.cn/gtwmdhqytw.html

Ruby ........... 212
来源：http://hz.c1oappe.top/gtvxdqiqzo.html

C# ............. 212
来源：http://hz.sysykeji.top/gtgxvivcun.html

C .............. 30
来源：http://hz.zhixingplan.top/gtjbjuares.html

C++ ............ 30
来源：http://hz.9152youxi.cn/gtipztmrqb.html

SQL ............ 90
来源：http://hz.sweek.top/gtvrjmidaa.html

Bash ........... 80
来源：http://hz.snrcjt.cn/gtviuuxrly.html

Kotlin ......... 15
来源：http://hz.pengpengdd.cyou/gtxwnncsvj.html

Swift .......... 15
来源：http://hz.daxiang520.top/gtnjxldoas.html

Lua ............ 10
来源：http://hz.guannengcc.top/gtvptjyotc.html

Perl ........... 10
来源：http://hz.aizwys.cn/gtfhirycdz.html

Scala .......... 10
来源：http://hz.vqdsnc.cn/gtxunmzyil.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtgnbfkszv.html

合计 ........... 2106 条
来源：http://hz.tanke756.top/gtdcvvvjkk.html

按章节统计：
来源：http://hz.tianlin.xyz/gtiwavhgnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtxaxkqalb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtxxsexllf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtladgicup.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtwwbrlhrv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnxiangtu.top/gtwhbhqrrk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj20258888.top/gtdzwhhnwa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtkyaepdhy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.daxiang520.top/gttoomughn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtzwdvksap.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtlinrclbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtfctryysk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtuqfezgxl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtrefwgqxl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtizxqbeji.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangkeji.top/gtcarmlyrb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtxpvgxmke.html

Q SQL 专题                              90
来源：http://hz.daxiang520.top/gteuyjfnev.html

R Bash 专题                             80
来源：http://hz.daria6918.cn/gtjrqlfntd.html

S C / C++ 专题                          60
来源：http://hz.haohaochexian.top/gtgbeoxtnn.html

T 其他语言补充                          60
来源：http://hz.cucudq.cn/gtyhztlqgr.html

U 高频实用片段                         120
来源：http://hz.tian-w.cn/gtnlhngctr.html

------------------------------------
来源：http://hz.dashuyun.cn/gtopwfbioy.html

合计                                  2106 条
来源：http://hz.xylfe.cn/gtssebjlnj.html

--------------------------------------------------------------------------------
来源：http://hz.tianlin.xyz/gtjdvncpsn.html


<!-- 参考信息 -->