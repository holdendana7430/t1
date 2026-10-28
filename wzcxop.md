代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://hz.tianlin.xyz/gtypyymihz.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtyrptabob.html

println("Hello")
来源：http://hz.ehwqpu.com/gtcasgnziq.html

[T52] Scala：变量
来源：http://hz.dashuyun.cn/gtnodykgke.html

val a = 1;  var b = 2
来源：http://hz.zhaomingkeji.xyz/gtkhjesmsr.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gtwtodhqan.html

s"值: $b"
来源：http://hz.ybcxt.top/gtwzlrlgla.html

[T54] Scala：集合映射
来源：http://hz.nanxuanxn.top/gtrandqvxg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ywan-chungtsiang.top/gttmshyufx.html

[T55] Scala：集合过滤
来源：http://hz.cheryme.top/gtkberjowy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jlsjyb.cn/gthnlmzlcy.html

[T56] Scala：样例类
来源：http://hz.cucudq.cn/gtnbjycukc.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gtdbctubiz.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gtcqewejgh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhixingplan.top/gtgxipxfsj.html

[T58] Scala：函数定义
来源：http://hz.gaohongyu789.top/gtuegzzpre.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yuanzhike.top/gtqjlimhjw.html

[T59] Scala：循环
来源：http://hz.bjfxy.top/gtymvskkkb.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtsvnghcwo.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gtfdtbznxy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtximhbxtx.html

================================================================================
来源：http://hz.jyoumei.cn/gtywmrfidj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jyoumei.cn/gtpbmnppjs.html

================================================================================
来源：http://hz.yueranfly.top/gtelcjdymg.html

[U01] Py：创建虚拟环境
来源：http://hz.zhixingplan.top/gtiotoaaiv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cdnleiting.top/gtixkhsolt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigfzy.top/gtoceienba.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtucvyorjz.html

[U03] Py：加载 .env 配置
来源：http://hz.hysaishi.cn/gtefgjasrz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yueranfly.top/gtvsqaufhb.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gtdqlduxdn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yvedp.cn/gtyonruamk.html

[U05] Py：列表去重且保序
来源：http://hz.fengsongda.top/gtbssfpnxa.html

list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtwgxgqsch.html

[U06] Py：合并两个字典
来源：http://hz.zdqjudy.top/gtnvonkihj.html

{**a, **b}
来源：http://hz.hywenlv.cn/gtholrxuet.html

[U07] Py：反转字典键值
来源：http://hz.yangfankeji.com/gtnknxqmsk.html

{v: k for k, v in d.items()}
来源：http://hz.bjfxy.top/gtmtnyccma.html

[U08] Py：展平二维列表
来源：http://hz.aizwys.cn/gtponhfxev.html

[y for x in nested for y in x]
来源：http://hz.yongpay.top/gtymnjkxxq.html

[U09] Py：字典取最大值的键
来源：http://hz.svipenyu.cn/gtqpbsiqlg.html

max(d, key=d.get)
来源：http://hz.guowangkeji.top/gtwlyvhkmj.html

[U10] Py：按值排序字典
来源：http://hz.wangshuangyany.cn/gtgmymbvwl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sysykeji.top/gtsxaiyuph.html

[U11] Py：生成器表达式
来源：http://hz.tanke756.top/gtcbkzptdb.html

(x * 2 for x in arr)
来源：http://hz.tian-w.cn/gtzbvaspgi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtvcerwjxz.html

Counter(arr).most_common(3)
来源：http://hz.jianghu66.top/gtaceymryz.html

[U13] Py：固定长度队列
来源：http://hz.redwolf501.top/gtwhakwtmt.html

deque(maxlen=10)
来源：http://hz.nanxuanxn.top/gtrxojywjz.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gtifxqcheg.html

defaultdict(list)
来源：http://hz.yj20258.top/gtufseqrci.html

[U15] Py：高精度计时
来源：http://hz.dianchejie.cn/gtluddwnjx.html

t = time.perf_counter()
来源：http://hz.sufxvd.cn/gtbmjerdxo.html

[U16] Py：命令行参数解析
来源：http://hz.yangfankeji.com/gthjwnhfys.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtqncfogdx.html

[U17] Py：初始化日志
来源：http://hz.jqgfzy.top/gtluqwcohm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258.top/gtwltxgyht.html

[U18] Py：预编译正则
来源：http://hz.tian-w.cn/gtpcjccahf.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258888.top/gttdnjdmrv.html

[U19] Py：正则替换带回调
来源：http://hz.xinyue.icu/gtutqlrmjh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenlongwang.top/gtbjivxprw.html

[U20] Py：缓存函数结果
来源：http://hz.jlsjyb.cn/gtyclhdcly.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gzhubu.top/gtsktfsvfk.html

[U21] Py：自定义上下文管理器
来源：http://hz.wangshuangyany.cn/gtgzxfnxok.html

@contextlib.contextmanager
来源：http://hz.nwbrower.top/gtwuvemloh.html

[U22] Py：矩阵转置
来源：http://hz.dianchejie.cn/gtpeezklfq.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gtvdzpxoxo.html

[U23] Py：分块读取大文件
来源：http://hz.jinyuanbaomall.cn/gtkkstoiup.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtfviabvew.html

[U24] Py：路径操作
来源：http://hz.ydzc1.top/gtxgqmuxpi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtsmaeawcp.html

[U25] Py：CSV 按字典读
来源：http://hz.zycfv.cn/gtpoazjapm.html

csv.DictReader(f)
来源：http://hz.zhengqikj.top/gtwtkyoqsb.html

[U26] Py：并发下载
来源：http://hz.wangdashe.top/gtjdodzhtu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.tianlin.xyz/gtroxpijjs.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtiedqdwwq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj202588.top/gtayhstrmz.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gtqqjhpmcu.html

UserId = int
来源：http://hz.dashuyun.cn/gtwzjskbws.html

[U29] Py：属性校验
来源：http://hz.havefunace.top/gthistaysp.html

@property 与 @x.setter 配合
来源：http://hz.daria6918.cn/gtnxecttrr.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gttigxupqe.html

@dataclass(slots=True)
来源：http://hz.fzhhl.top/gtalpcihpo.html

[U31] Py：单测
来源：http://hz.0kj1m.cn/gtxdopowzz.html

python -m pytest -q
来源：http://hz.chenzaomai.com/gtmksqnsni.html

[U32] Py：代码格式化
来源：http://hz.hammf.cn/gtbywihatn.html

ruff format . && ruff check --fix .
来源：http://hz.yanxiufei.cn/gtlbuikcop.html

[U33] Py：打包发布
来源：http://hz.zhiwuduotai.top/gtwxgfyxfl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sxryk.cn/gtbcdsuiie.html

[U34] Py：判断编码
来源：http://hz.52xcode.cn/gtqrfygmpm.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtcxplhxfo.html

[U35] Py：发送邮件
来源：http://hz.xziqi.cn/gthkcvbiet.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cashguo.top/gtaigaqpjw.html

[U36] Py：定时任务
来源：http://hz.xinyue.icu/gtraewmhcz.html

schedule.every(10).minutes.do(job)
来源：http://hz.wangdashe.top/gtozavnqin.html

[U37] Py：读写 Excel
来源：http://hz.xinyue.icu/gtihmpjafe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ybcxt.top/gtwkyibvvq.html

[U38] Py：获取脚本所在目录
来源：http://hz.zycfv.cn/gtjyropltd.html

Path(__file__).resolve().parent
来源：http://hz.birdmap.top/gtpozpjkal.html

[U39] Py：判断是否在交互环境
来源：http://hz.cdnleiting.top/gtvavlabic.html

sys.stdout.isatty()
来源：http://hz.meibo888.top/gtujwuzvxr.html

[U40] Py：打印到标准错误
来源：http://hz.zdqjudy.top/gtrcriwieg.html

print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gttdzqxvun.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yanxiufei.cn/gttxznnnyg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sysykeji.top/gtnxqdcbsh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.52xcode.cn/gtdkyufozr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cucudq.cn/gtyppwyhrj.html

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtcwyiayjx.html

namespace App\Http;
来源：http://hz.hnqzz.top/gtasditjlv.html

[U44] PHP：开启严格类型
来源：http://hz.jyoumei.cn/gtafvqpanr.html

declare(strict_types=1);
来源：http://hz.jianghu66.top/gtmsnkbvzw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhongyouzk.top/gtnfkblvlq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtbejpljrs.html

[U46] PHP：可空类型
来源：http://hz.yonumen.top/gtsakiggup.html

?string $name = null
来源：http://hz.yongpay.top/gtbknfyvti.html

[U47] PHP：联合类型
来源：http://hz.pengpengdd.cyou/gtaiciuonp.html

int|string $id
来源：http://hz.jlsjyb.cn/gtjheuyqgl.html

[U48] PHP：纯枚举
来源：http://hz.shanyushiyangkeji.top/gtmbmabxkg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gzhubu.top/gtjkmkufub.html

[U49] PHP：只读属性
来源：http://hz.ydzc1.top/gteteebcqa.html

public readonly string $name
来源：http://hz.guowangkeji.top/gtodbmbtpd.html

[U50] PHP：构造器属性提升
来源：http://hz.cqqwz.cn/gtnqqejefm.html

public function __construct(private int $id) {}
来源：http://hz.fengsongda.top/gtcgmyzwmn.html

[U51] PHP：数组解构
来源：http://hz.wangshuangyany.cn/gtbqtmfshl.html

[$a, $b] = $arr;
来源：http://hz.xingfuxueyuan.xyz/gtcnkqnncq.html

[U52] PHP：箭头函数
来源：http://hz.jyoumei.cn/gtbnqhnxge.html

$double = fn($x) => $x * 2;
来源：http://hz.0kj1m.cn/gtildsafms.html

[U53] PHP：空合并运算符
来源：http://hz.chenjidiqi.icu/gtalxzkubq.html

$v = $a ?? $b ?? "default";
来源：http://hz.guowangkeji.top/gtumvdqooe.html

[U54] PHP：空安全调用
来源：http://hz.gogol.net.cn/gtulkzslvc.html

$obj?->method()
来源：http://hz.iojbl.cn/gtizzwjcvr.html

[U55] PHP：match 表达式
来源：http://hz.gaohongyu789.top/gthbwaabnt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cucudq.cn/gtzceyzdrk.html

[U56] PHP：命名参数
来源：http://hz.feifeiyinyue.top/gttqnxhhay.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtnozqjbsj.html

[U57] PHP：字符串插值
来源：http://hz.hnxiangtu.top/gtovrhgjgh.html

"值: {$a}"
来源：http://hz.xinyue.icu/gtynayceoe.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtamtmozkz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigfzy.top/gtsevgdqtg.html

[U59] PHP：自定义排序
来源：http://hz.xuetiantiany.cn/gtwlapodva.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtoyzaleeb.html

[U60] PHP：JSON 编解码
来源：http://hz.cashguo.top/gtekpisibn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.daxiang520.top/gtbhnkmtic.html

[U61] PHP：正则
来源：http://hz.cqqwz.cn/gtvylxnzny.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gtgqpjnycc.html

[U62] PHP：日期对象
来源：http://hz.ehwqpu.com/gtdpgtfdgm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.quarkkingdee.top/gtvwkandgr.html

[U63] PHP：文件读写
来源：http://hz.hysaishi.cn/gtxvnhwaxn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.redwolf501.top/gtuwdlmkzi.html

[U64] PHP：目录遍历
来源：http://hz.ydzc1.top/gtfyknfpac.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tanke756.top/gtspbasutd.html

[U65] PHP：会话
来源：http://hz.zhixingplan.top/gtugyvnvex.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yvedp.cn/gtpxpnnorz.html

[U66] PHP：设置 Cookie
来源：http://hz.hnxiangtu.top/gtckimyjxz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnxiangtu.top/gtprlvqldj.html

[U67] PHP：处理文件上传
来源：http://hz.yongpay.top/gtzjshegnc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.9152youxi.cn/gtscsshggf.html

[U68] PHP：PDO 连接
来源：http://hz.nwbrower.top/gtfcbszpnr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shzxlz.cn/gtxqubbrlc.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtuviviznn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ybcxt.top/gttjxncezq.html

[U70] PHP：PDO 事务
来源：http://hz.zhoulong.xyz/gtszlxogdy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shzxlz.cn/gtwuyiapod.html

[U71] PHP：抛出异常
来源：http://hz.hywenlv.cn/gtmzjntiqi.html

throw new RuntimeException("失败", 500);
来源：http://hz.snrcjt.cn/gtcvsmaoim.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangkeji.top/gtfrptorit.html

error_log("失败: " . $e->getMessage());
来源：http://hz.guannengcc.top/gtwnbrlouk.html

[U73] PHP：读取 ini 配置
来源：http://hz.feifeiyinyue.top/gtsbgpctpb.html

parse_ini_file("config.ini", true)
来源：http://hz.yueranfly.top/gtooaidqvu.html

[U74] PHP：读取环境变量
来源：http://hz.dianchejie.cn/gtzwnuaeqb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinghuilouyu.cn/gtcxjefhuq.html

[U75] PHP：依赖注入
来源：http://hz.xuanzx.com/gtnaiymmbz.html

composer require psr/container
来源：http://hz.ppjwa.cn/gtktnhqzpq.html

[U76] PHP：简单路由
来源：http://hz.yangfankeji.com/gtlkxklkux.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.0kj1m.cn/gtvlbjrfdx.html

[U77] PHP：模板渲染
来源：http://hz.wangdashe.top/gtslnesuyb.html

composer require twig/twig
来源：http://hz.hfpthk.cn/gtgnpxudvt.html

[U78] PHP：单元测试
来源：http://hz.meibo888.top/gtrgsayetx.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtqdcbmeop.html

[U79] PHP：静态分析
来源：http://hz.yanxiufei.cn/gtyilwgqlj.html

composer require --dev phpstan/phpstan
来源：http://hz.52xcode.cn/gtngekatjx.html

[U80] PHP：代码规范修复
来源：http://hz.zhijiandao.cn/gtoboqbkwn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nanxuanxn.top/gtkejtitcb.html

[U81] JS：初始化项目
来源：http://hz.52xcode.cn/gtyxiiynrf.html

npm init -y;  npm i express
来源：http://hz.snrcjt.cn/gtlixozgat.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangkeji.top/gtxthlcoki.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtosutyknt.html

[U83] JS：ES Module 导入导出
来源：http://hz.sysykeji.top/gtclhyuunz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yvedp.cn/gtwlmzzlag.html

[U84] JS：CommonJS 写法
来源：http://hz.ybcxt.top/gtmypdxwlo.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtpvktbfgz.html

[U85] JS：可选链
来源：http://hz.snrcjt.cn/gtsneracvl.html

a?.b?.c
来源：http://hz.quarkkingdee.top/gtmobmiymh.html

[U86] JS：空值合并
来源：http://hz.xylfe.cn/gtqplhqnga.html

a ?? b
来源：http://hz.xuetiantiany.cn/gtlpyrpgcg.html

[U87] JS：解构默认值
来源：http://hz.vqdsnc.cn/gtkddetgpe.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gtyfvcectp.html

[U88] JS：对象展开合并
来源：http://hz.birdmap.top/gteoqfwxrs.html

{ ...a, ...b }
来源：http://hz.zhixingplan.top/gttjhjbhqf.html

[U89] JS：数组去重
来源：http://hz.jinqigufen.top/gtabpiozrc.html

[...new Set(arr)]
来源：http://hz.pycfn.com/gtkfnyeyqz.html

[U90] JS：数字数组排序
来源：http://hz.xingfuxueyuan.xyz/gtkjylflaq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtbhbikhkv.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtrmetjsom.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ivvv.top/gtstatiksy.html

[U92] JS：深拷贝
来源：http://hz.tian-w.cn/gtsfgdjvjy.html

structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtnfajjggw.html

[U93] JS：模板字符串
来源：http://hz.smart0.xyz/gtbvecfvac.html

`共 ${n} 条`
来源：http://hz.hammf.cn/gtxapjmrkn.html

[U94] JS：箭头函数
来源：http://hz.andypj.xyz/gtlgswuimy.html

const double = x => x * 2;
来源：http://hz.ehwqpu.com/gtwxeafxag.html

[U95] JS：Promise 包装
来源：http://hz.daria6918.cn/gtkchgzoku.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtpkpbnjmy.html

[U96] JS：async/await 与异常
来源：http://hz.tanke756.top/gtewsyynur.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtjkmrlexk.html

[U97] JS：并发请求
来源：http://hz.ehwqpu.com/gtjmmsljty.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtvkhudika.html

[U98] JS：fetch 带 JSON
来源：http://hz.tianlin.xyz/gtjhlqcnhb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sweek.top/gtfhnzhbnj.html

[U99] JS：事件监听
来源：http://hz.9152youxi.cn/gttishaxyv.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gteemtkzgf.html

[U100] JS：DOM 查询
来源：http://hz.nanxuanxn.top/gtdsgvmiwv.html

document.querySelector(".item")
来源：http://hz.guannengcc.top/gtizjdnsew.html

[U101] JS：classList 操作
来源：http://hz.shuidangran.top/gtzllcfvkc.html

el.classList.toggle("active")
来源：http://hz.jqgufenzy.top/gtnchhqkxc.html

[U102] JS：本地存储
来源：http://hz.hammf.cn/gtvevhkxpd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.vqdsnc.cn/gtzeulvqmg.html

[U103] JS：定时器
来源：http://hz.gzhubu.top/gtbcpcsmxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gotoacloud.top/gtdspyxrvo.html

[U104] JS：防抖
来源：http://hz.ehwqpu.com/gtavujetql.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtaynrdytr.html

[U105] JS：节流
来源：http://hz.bjfxy.top/gterdttbej.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ehwqpu.com/gtwzuhhmfo.html

[U106] JS：日期格式化
来源：http://hz.chenlongwang.top/gtwjhqnwfl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gttprrnedk.html

[U107] JS：数字千分位
来源：http://hz.shzxlz.cn/gtrqkjauqn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.snrcjt.cn/gtnvxtzzlq.html

[U108] JS：随机整数
来源：http://hz.hywenlv.cn/gtgcqdjvko.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gotoacloud.top/gtrqcwbhjb.html

[U109] JS：数组分组
来源：http://hz.gzhubu.top/gtrrhijzmg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ppjwa.cn/gtmepqayuq.html

[U110] JS：数组分块
来源：http://hz.jinqigfzy.top/gtgpglvzfu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.smart0.xyz/gttgpqenom.html

[U111] JS：对象转 Map
来源：http://hz.shanyushiyangtech.top/gtkmbforxc.html

new Map(Object.entries(obj))
来源：http://hz.feifeiyinyue.top/gtskshwnru.html

[U112] JS：字符串补位
来源：http://hz.ywan-chungtsiang.top/gtlhceuyig.html

"7".padStart(3, "0")
来源：http://hz.pycfn.com/gtsdnyxdrd.html

[U113] JS：正则替换全部
来源：http://hz.pengpengdd.cyou/gtpxxtismj.html

s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtvvzuoviq.html

[U114] JS：JSON 深比较
来源：http://hz.iojbl.cn/gteakurrol.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtzkffmtrg.html

[U115] JS：生成 UUID
来源：http://hz.hfpthk.cn/gthvrdyxla.html

crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtrjdjhktf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.haohaochexian.top/gtckyryyur.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenzaomai.com/gtajrxybsw.html

[U117] JS：单元测试
来源：http://hz.yonumen.top/gtidzsmnve.html

npm i -D vitest;  npx vitest
来源：http://hz.jlsjyb.cn/gtkojgkqbb.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtuirxyham.html

npm i -D vite;  npx vite
来源：http://hz.gzhubu.top/gtdjqnppis.html

[U119] JS：生产构建
来源：http://hz.snrcjt.cn/gtgedyaanr.html

npx vite build
来源：http://hz.cashguo.top/gtqfguvvng.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtjoutprza.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtdfgfzpyi.html

================================================================================
来源：http://hz.yvedp.cn/gtmfgenolo.html

统计汇总
来源：http://hz.xinyue.icu/gtvfouqhkr.html

================================================================================
来源：http://hz.yuxming.cn/gtofbncnid.html

按语言统计（条）：
来源：http://hz.yvedp.cn/gtfdguvlot.html

Python ......... 252
来源：http://hz.hnqzz.top/gtdcfcprho.html

PHP ............ 252
来源：http://hz.tianlin.xyz/gtvylgxmgx.html

JavaScript ..... 252
来源：http://hz.0kj1m.cn/gtcpobbzsj.html

TypeScript ..... 212
来源：http://hz.nanxuanxn.top/gtkqojdyij.html

Java ........... 212
来源：http://hz.daria6918.cn/gtxgxybtpi.html

Go ............. 212
来源：http://hz.bjfxy.top/gtcqkfotrs.html

Ruby ........... 212
来源：http://hz.ybcxt.top/gtfyxfyvmf.html

C# ............. 212
来源：http://hz.cdnleiting.top/gtzxsdhxea.html

C .............. 30
来源：http://hz.hnqzz.top/gtmhmoqmgk.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtiaenuujb.html

SQL ............ 90
来源：http://hz.zycfv.cn/gtqzedemvp.html

Bash ........... 80
来源：http://hz.havefunace.top/gtmvgorkrx.html

Kotlin ......... 15
来源：http://hz.52xcode.cn/gtnuaxxfgc.html

Swift .......... 15
来源：http://hz.quarkkingdee.top/gtrhllqqle.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtaausahwy.html

Perl ........... 10
来源：http://hz.zhengqikj.top/gtmyatmmhs.html

Scala .......... 10
来源：http://hz.sysykeji.top/gtsohlmhpu.html

------------------------------------
来源：http://hz.yongpay.top/gthvmnwhew.html

合计 ........... 2106 条
来源：http://hz.yonumen.top/gtjwjwwagu.html

按章节统计：
来源：http://hz.sxryk.cn/gtkcihdkrr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtmemioqgz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtjuvljvap.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtwyjhiesu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtkioteoht.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.guannengcc.top/gtskjflyto.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gthzhqhyis.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xuanzx.com/gtbdrjmrlu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtbvqsuoob.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtawezsfpj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtydsctgfc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtfhbrlmnm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtvyiatdio.html


<!-- 参考信息 -->