代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://hz.cucudq.cn/gtwdwnxgyw.html

[T51] Scala：Hello World
来源：http://hz.tianlin.xyz/gtluwhqkdu.html

println("Hello")
来源：http://hz.yj202588.top/gtdfpqmnsw.html

[T52] Scala：变量
来源：http://hz.jinyuanbaomall.cn/gtdtlzrvus.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtvyxdewaw.html

[T53] Scala：字符串插值
来源：http://hz.hongshengwenyu.top/gtgpjkzgom.html

s"值: $b"
来源：http://hz.fengsongda.top/gtwcniwdpc.html

[T54] Scala：集合映射
来源：http://hz.zhongyouzk.top/gtgjhmxkob.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xingfuxueyuan.xyz/gtvwjspwve.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtsspubbjp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gtyrmbzbke.html

[T56] Scala：样例类
来源：http://hz.quarkkingdee.top/gtbrvdwnqp.html

case class User(name: String, age: Int)
来源：http://hz.hfpthk.cn/gtxsknvlvq.html

[T57] Scala：模式匹配
来源：http://hz.shangyingyoupin.top/gtbmmmfnid.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hysaishi.cn/gtmnahzhfi.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gttxeclyoy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xingfuxueyuan.xyz/gtwvgrjqfv.html

[T59] Scala：循环
来源：http://hz.yanxiufei.cn/gtepawoots.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhoulong.xyz/gtervvgerl.html

[T60] Scala：折叠
来源：http://hz.cucudq.cn/gtubshaufv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cqqwz.cn/gtkoxnlpou.html

================================================================================
来源：http://hz.pycfn.com/gtlalcbfre.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtapgzzugg.html

================================================================================
来源：http://hz.jianghu66.top/gtpekulsaj.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gttkgullpu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cashguo.top/gtmzghhtbs.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigufen.top/gtzmcltalv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xziqi.cn/gthgrizfws.html

[U03] Py：加载 .env 配置
来源：http://hz.zdqjudy.top/gtmpnwzibo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.52xcode.cn/gtuudhhtmj.html

[U04] Py：变量调试打印
来源：http://hz.smart0.xyz/gtjfcoxmtw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.316326.xyz/gtdtyihmzb.html

[U05] Py：列表去重且保序
来源：http://hz.daria6918.cn/gtbzogpgyj.html

list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gticvkcvrs.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gtrxmszfqi.html

{**a, **b}
来源：http://hz.yonumen.top/gtggpxuaqy.html

[U07] Py：反转字典键值
来源：http://hz.xingfuxueyuan.xyz/gtwlrqgogs.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtofdooefh.html

[U08] Py：展平二维列表
来源：http://hz.jqgfzy.top/gtqbsxumgc.html

[y for x in nested for y in x]
来源：http://hz.cqqwz.cn/gtijggakcm.html

[U09] Py：字典取最大值的键
来源：http://hz.nanxinkj.top/gtryawggmm.html

max(d, key=d.get)
来源：http://hz.shanyushiyangtech.top/gtmfhefspc.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gtzbxojzdd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.quarkkingdee.top/gtnwhwphbm.html

[U11] Py：生成器表达式
来源：http://hz.zycfv.cn/gtztuuubyi.html

(x * 2 for x in arr)
来源：http://hz.yuxming.cn/gtpxhcozng.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gtyowkhdwr.html

Counter(arr).most_common(3)
来源：http://hz.c1oappe.top/gtcivrhmdg.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangtech.top/gtuifeifle.html

deque(maxlen=10)
来源：http://hz.smart0.xyz/gtblrvueap.html

[U14] Py：分组收集到列表
来源：http://hz.wangshuangyany.cn/gtcjatchdi.html

defaultdict(list)
来源：http://hz.shanyushiyangtech.top/gtkptosikc.html

[U15] Py：高精度计时
来源：http://hz.feifeiyinyue.top/gtpcfzbtvx.html

t = time.perf_counter()
来源：http://hz.jinghuilouyu.cn/gtxsxecnhr.html

[U16] Py：命令行参数解析
来源：http://hz.jqgfzy.top/gtsraqlgll.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gtmlefuocc.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtckbqckvg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.52xcode.cn/gtpssnbqnw.html

[U18] Py：预编译正则
来源：http://hz.mhx1999.top/gtkelmlcdn.html

pat = re.compile(r"\d+")
来源：http://hz.yueranfly.top/gtunlkqquh.html

[U19] Py：正则替换带回调
来源：http://hz.hysaishi.cn/gtcpkdqigp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj20258888.top/gtssqoxuwb.html

[U20] Py：缓存函数结果
来源：http://hz.wangshuangyany.cn/gtcmuljwdc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.c1oappe.top/gtuhxywjin.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinyuanbaomall.cn/gtgagplewl.html

@contextlib.contextmanager
来源：http://hz.daria6918.cn/gtfwwrqxjh.html

[U22] Py：矩阵转置
来源：http://hz.gogol.net.cn/gtzazmwcnl.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtgvpmojcv.html

[U23] Py：分块读取大文件
来源：http://hz.zhengqikj.top/gtixxptdgd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.nanxuanxn.top/gtxmgzfluz.html

[U24] Py：路径操作
来源：http://hz.andypj.xyz/gtglzbhjgg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cucudq.cn/gtdpvqbded.html

[U25] Py：CSV 按字典读
来源：http://hz.redwolf501.top/gtnsqzzvug.html

csv.DictReader(f)
来源：http://hz.yueranfly.top/gthuhoxmov.html

[U26] Py：并发下载
来源：http://hz.zhijiandao.cn/gtannnxhgb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtmrllugow.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtmjyfemdt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenzaomai.com/gtsvqznslc.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtlpqqriuc.html

UserId = int
来源：http://hz.jinghuilouyu.cn/gtsvppyhme.html

[U29] Py：属性校验
来源：http://hz.ivvv.top/gtvpyodats.html

@property 与 @x.setter 配合
来源：http://hz.jinghuilouyu.cn/gtqbmluwdy.html

[U30] Py：数据类
来源：http://hz.hfpthk.cn/gtvwqlkjue.html

@dataclass(slots=True)
来源：http://hz.dianchejie.cn/gtjkpaikgx.html

[U31] Py：单测
来源：http://hz.hnqzz.top/gtlwxlnpgj.html

python -m pytest -q
来源：http://hz.chenzaomai.com/gtbieoslqa.html

[U32] Py：代码格式化
来源：http://hz.wangshuangyany.cn/gttzqhkska.html

ruff format . && ruff check --fix .
来源：http://hz.shuidangran.top/gtdqcotgmo.html

[U33] Py：打包发布
来源：http://hz.cqqwz.cn/gtwsinevmb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.9152youxi.cn/gtjessidzy.html

[U34] Py：判断编码
来源：http://hz.sxryk.cn/gtvujunuow.html

chardet.detect(raw)
来源：http://hz.cucudq.cn/gtwavfdust.html

[U35] Py：发送邮件
来源：http://hz.sxryk.cn/gtaugdalse.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.aizwys.cn/gtzcgbhnwz.html

[U36] Py：定时任务
来源：http://hz.gaohongyu789.top/gtfoaslaun.html

schedule.every(10).minutes.do(job)
来源：http://hz.gogol.net.cn/gtxxmvbpqm.html

[U37] Py：读写 Excel
来源：http://hz.pengpengdd.cyou/gtncvcrqpo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinyuanbaomall.cn/gtedaymakm.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhaomingkeji.xyz/gtsfozgyjz.html

Path(__file__).resolve().parent
来源：http://hz.jinghuilouyu.cn/gtyluwxvvb.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhoulong.xyz/gtjzdudfci.html

sys.stdout.isatty()
来源：http://hz.tianlin.xyz/gtgvlcfqai.html

[U40] Py：打印到标准错误
来源：http://hz.aibaodan.cn/gtthqkkkem.html

print("err", file=sys.stderr)
来源：http://hz.yongpay.top/gtbmuuedva.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhijiandao.cn/gthszsibrl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigfzy.top/gtqbipwgqa.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yanxiufei.cn/gtzcrdahtd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fengsongda.top/gtwurdbtoo.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangkeji.top/gtjsomfwoy.html

namespace App\Http;
来源：http://hz.yuanzhike.top/gtcswwhogg.html

[U44] PHP：开启严格类型
来源：http://hz.zhoulong.xyz/gtndzhoees.html

declare(strict_types=1);
来源：http://hz.cdnleiting.top/gtpzataptr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.aibaodan.cn/gtbawybzzx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtcsehonmf.html

[U46] PHP：可空类型
来源：http://hz.yangfankeji.com/gtpddebdaq.html

?string $name = null
来源：http://hz.ivvv.top/gtbihonxvp.html

[U47] PHP：联合类型
来源：http://hz.jqgfzy.top/gtfkyqnmce.html

int|string $id
来源：http://hz.ydjk.org.cn/gtsxrmwwfh.html

[U48] PHP：纯枚举
来源：http://hz.jyoumei.cn/gtopbvtheq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.wangdashe.top/gteipqlnsz.html

[U49] PHP：只读属性
来源：http://hz.cashguo.top/gtfadlixab.html

public readonly string $name
来源：http://hz.pycfn.com/gteqjqcyuu.html

[U50] PHP：构造器属性提升
来源：http://hz.shuidangran.top/gtiklhzxfp.html

public function __construct(private int $id) {}
来源：http://hz.zhijiandao.cn/gtngppleqw.html

[U51] PHP：数组解构
来源：http://hz.shzxlz.cn/gtkucqarqt.html

[$a, $b] = $arr;
来源：http://hz.feifeiyinyue.top/gtmqguqlqz.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtfxbebprd.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtfgvpmnam.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gtobwpwbpq.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigfzy.top/gtopkhlpxh.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gtlqrjtknb.html

$obj?->method()
来源：http://hz.aibaodan.cn/gtghdqlfhj.html

[U55] PHP：match 表达式
来源：http://hz.yangfankeji.com/gtygtlymwa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gtjxgrrmul.html

[U56] PHP：命名参数
来源：http://hz.c1oappe.top/gtbmxfaznn.html

f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtunioexal.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gtfzhkogon.html

"值: {$a}"
来源：http://hz.fzhhl.top/gteogvvmzz.html

[U58] PHP：数组三件套
来源：http://hz.shanyushiyangtech.top/gtyaavgldi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yuanzhike.top/gtlkofdmly.html

[U59] PHP：自定义排序
来源：http://hz.meibo888.top/gtygvxfiqm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenzaomai.com/gtbbztblaa.html

[U60] PHP：JSON 编解码
来源：http://hz.yuanzhike.top/gtamptnktc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gtpmjsyeeq.html

[U61] PHP：正则
来源：http://hz.yonumen.top/gthmtndjnu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnqzz.top/gtthkwuudc.html

[U62] PHP：日期对象
来源：http://hz.wangdashe.top/gtjkywyydw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhoulong.xyz/gtommryzjd.html

[U63] PHP：文件读写
来源：http://hz.hnqzz.top/gtqfwrvwaz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gtjjxjlqkn.html

[U64] PHP：目录遍历
来源：http://hz.yongpay.top/gtnzgewpgu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shanyushiyangtech.top/gtoxvqbtid.html

[U65] PHP：会话
来源：http://hz.hnqzz.top/gtzrvmiqys.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinqigufen.top/gtlzamscoo.html

[U66] PHP：设置 Cookie
来源：http://hz.vqdsnc.cn/gtprsorxpx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.kuanghao11.cn/gtbbypstul.html

[U67] PHP：处理文件上传
来源：http://hz.yonumen.top/gtvogzrnwx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.birdmap.top/gtdpzgmeid.html

[U68] PHP：PDO 连接
来源：http://hz.xylfe.cn/gtcgayhuxk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cucudq.cn/gtpqmhlppx.html

[U69] PHP：PDO 预处理
来源：http://hz.316326.xyz/gteebnsqny.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.bjfxy.top/gtmgowwfdz.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtrbibypda.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhongyouzk.top/gtpyookbdy.html

[U71] PHP：抛出异常
来源：http://hz.wangshuangyany.cn/gtgxvdgbpq.html

throw new RuntimeException("失败", 500);
来源：http://hz.vqdsnc.cn/gttlsxdjrw.html

[U72] PHP：写错误日志
来源：http://hz.daria6918.cn/gtpbkuknlh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sufxvd.cn/gtuelwenhf.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtrwmezqsy.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigfzy.top/gtaxupadiy.html

[U74] PHP：读取环境变量
来源：http://hz.cdnleiting.top/gtcjfwjwqp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gzhubu.top/gtnnbfoptx.html

[U75] PHP：依赖注入
来源：http://hz.jianghu66.top/gtzkpejobx.html

composer require psr/container
来源：http://hz.yangfankeji.com/gtsvgnkigg.html

[U76] PHP：简单路由
来源：http://hz.yonumen.top/gtusoqxete.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.kuanghao11.cn/gtkzcgipyi.html

[U77] PHP：模板渲染
来源：http://hz.jiagoushi.top/gtkupundfl.html

composer require twig/twig
来源：http://hz.andypj.xyz/gthsaxffsn.html

[U78] PHP：单元测试
来源：http://hz.ydzc1.top/gtclbbrpcb.html

composer require --dev phpunit/phpunit
来源：http://hz.guowangkeji.top/gtpnvnkhus.html

[U79] PHP：静态分析
来源：http://hz.ehwqpu.com/gtctaaqmhc.html

composer require --dev phpstan/phpstan
来源：http://hz.0kj1m.cn/gtvdqdajmn.html

[U80] PHP：代码规范修复
来源：http://hz.jinghuilouyu.cn/gtlvrjuejz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hywenlv.cn/gtggljgbft.html

[U81] JS：初始化项目
来源：http://hz.wangshuangyany.cn/gtiqciuiwo.html

npm init -y;  npm i express
来源：http://hz.jqgfzy.top/gtddwkkvcc.html

[U82] JS：package.json 脚本
来源：http://hz.zhiwuduotai.top/gtjiozbbpz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guannengcc.top/gtqqwrhimv.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhixingplan.top/gtuknorwrl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ppjwa.cn/gtsmlhippl.html

[U84] JS：CommonJS 写法
来源：http://hz.xuetiantiany.cn/gtvcdqfamd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuanzhike.top/gtfvqtvkwx.html

[U85] JS：可选链
来源：http://hz.havefunace.top/gtzaojlcsz.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtnfxdcohj.html

[U86] JS：空值合并
来源：http://hz.xinyue.icu/gthttvtuwf.html

a ?? b
来源：http://hz.chenlongwang.top/gtprglpuvo.html

[U87] JS：解构默认值
来源：http://hz.hywenlv.cn/gtdjoggjyf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shuidangran.top/gtovlddqxr.html

[U88] JS：对象展开合并
来源：http://hz.xuanzx.com/gtnxpwjpyr.html

{ ...a, ...b }
来源：http://hz.c1oappe.top/gtfepquirw.html

[U89] JS：数组去重
来源：http://hz.cashguo.top/gtkhpnzaiz.html

[...new Set(arr)]
来源：http://hz.gogol.net.cn/gtdmfudtuc.html

[U90] JS：数字数组排序
来源：http://hz.guannengcc.top/gtotqzpolz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtqutsmmiv.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtzwuclxjo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.kuanghao11.cn/gtypyapzge.html

[U92] JS：深拷贝
来源：http://hz.tianlin.xyz/gtzdowuxvq.html

structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtikrqcdqn.html

[U93] JS：模板字符串
来源：http://hz.yongpay.top/gtyxqhckqz.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtarovmlhw.html

[U94] JS：箭头函数
来源：http://hz.mhx1999.top/gtfpeessid.html

const double = x => x * 2;
来源：http://hz.svipenyu.cn/gtnwgnxnuw.html

[U95] JS：Promise 包装
来源：http://hz.hfpthk.cn/gtacafpiha.html

new Promise((resolve, reject) => {})
来源：http://hz.xingfuxueyuan.xyz/gtyyqrlxln.html

[U96] JS：async/await 与异常
来源：http://hz.jyoumei.cn/gtonsnaess.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtjjssicpn.html

[U97] JS：并发请求
来源：http://hz.jianghu66.top/gtoxotwsji.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtrfyekhkq.html

[U98] JS：fetch 带 JSON
来源：http://hz.xinyue.icu/gtblbvcmzf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sxryk.cn/gtuornrmjj.html

[U99] JS：事件监听
来源：http://hz.aibaodan.cn/gtqgshnhio.html

el.addEventListener("click", e => {})
来源：http://hz.hnqzz.top/gtkcukhpij.html

[U100] JS：DOM 查询
来源：http://hz.0kj1m.cn/gtwxhaduaw.html

document.querySelector(".item")
来源：http://hz.jinghuilouyu.cn/gtygunztvv.html

[U101] JS：classList 操作
来源：http://hz.jinyuanbaomall.cn/gtapaabkll.html

el.classList.toggle("active")
来源：http://hz.gzhubu.top/gtmtomfnvo.html

[U102] JS：本地存储
来源：http://hz.jlsjyb.cn/gtpigjfjax.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenzaomai.com/gtorwtpqvu.html

[U103] JS：定时器
来源：http://hz.hongshengwenyu.top/gtuqpyprbb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cucudq.cn/gtokemxruf.html

[U104] JS：防抖
来源：http://hz.yuxming.cn/gtdqsslogq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtutihuzvf.html

[U105] JS：节流
来源：http://hz.hammf.cn/gtyewcnxei.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gogol.net.cn/gthliogcod.html

[U106] JS：日期格式化
来源：http://hz.kuanghao11.cn/gtmfyvhxbl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cheryme.top/gtxxwymmnh.html

[U107] JS：数字千分位
来源：http://hz.gzhubu.top/gtcwnacwtk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cucudq.cn/gtjkngoyvb.html

[U108] JS：随机整数
来源：http://hz.hnxiangtu.top/gtceekqvwy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nwbrower.top/gtvtlumpnv.html

[U109] JS：数组分组
来源：http://hz.havefunace.top/gtagaaxdpr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtzbhsxbde.html

[U110] JS：数组分块
来源：http://hz.hywenlv.cn/gthzzvhdaq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhoulong.xyz/gtalohvzzi.html

[U111] JS：对象转 Map
来源：http://hz.daria6918.cn/gtrbmlgvhw.html

new Map(Object.entries(obj))
来源：http://hz.fengsongda.top/gtcfjfjocd.html

[U112] JS：字符串补位
来源：http://hz.dianchejie.cn/gtiztakrzv.html

"7".padStart(3, "0")
来源：http://hz.meibo888.top/gttvttqkjo.html

[U113] JS：正则替换全部
来源：http://hz.jinqigufen.top/gtynvuznxf.html

s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtiuedifij.html

[U114] JS：JSON 深比较
来源：http://hz.vqdsnc.cn/gtbwxiqtnb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hywenlv.cn/gtkcygceoj.html

[U115] JS：生成 UUID
来源：http://hz.gogol.net.cn/gtujbjmkba.html

crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtsluaimio.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sxryk.cn/gtcmdnbgnx.html

/** @param {string} name */ function f(name) {}
来源：http://hz.quarkkingdee.top/gtmhqdzcdf.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangtech.top/gtisciolng.html

npm i -D vitest;  npx vitest
来源：http://hz.ehwqpu.com/gtlqilyolx.html

[U118] JS：开发服务器
来源：http://hz.daria6918.cn/gtnfqpzlnw.html

npm i -D vite;  npx vite
来源：http://hz.vqdsnc.cn/gtzfyqtxji.html

[U119] JS：生产构建
来源：http://hz.bjfxy.top/gtdqzbhebm.html

npx vite build
来源：http://hz.hongshengwenyu.top/gtskmlnsns.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zdqjudy.top/gtdlzmtbfz.html

import.meta.env.VITE_API_URL
来源：http://hz.ydzc1.top/gtglgpwioz.html

================================================================================
来源：http://hz.aizwys.cn/gtzpkpnbot.html

统计汇总
来源：http://hz.yongpay.top/gthkrjliuo.html

================================================================================
来源：http://hz.yongpay.top/gtcydspycv.html

按语言统计（条）：
来源：http://hz.wangshuangyany.cn/gttwlmrjaj.html

Python ......... 252
来源：http://hz.sxryk.cn/gtizrifmkk.html

PHP ............ 252
来源：http://hz.dianchejie.cn/gtygmrqtlu.html

JavaScript ..... 252
来源：http://hz.yvedp.cn/gtygvgmtpd.html

TypeScript ..... 212
来源：http://hz.aizwys.cn/gturddkiej.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtrihywaie.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtuzgdggdg.html

Ruby ........... 212
来源：http://hz.guowangkeji.top/gtyrhmljgx.html

C# ............. 212
来源：http://hz.ehwqpu.com/gtwmgezuos.html

C .............. 30
来源：http://hz.andypj.xyz/gtupibhtef.html

C++ ............ 30
来源：http://hz.kuanghao11.cn/gthdqnxnse.html

SQL ............ 90
来源：http://hz.svipenyu.cn/gttegzqfoi.html

Bash ........... 80
来源：http://hz.daxiang520.top/gtvxdsglop.html

Kotlin ......... 15
来源：http://hz.fzhhl.top/gtslfjehcv.html

Swift .......... 15
来源：http://hz.52xcode.cn/gtqzhozdjp.html

Lua ............ 10
来源：http://hz.zhiwuduotai.top/gtqeleqxob.html

Perl ........... 10
来源：http://hz.cdnleiting.top/gtmiutnncn.html

Scala .......... 10
来源：http://hz.nwbrower.top/gtuutnngrr.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtdvyjowns.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangtech.top/gttegvhycm.html

按章节统计：
来源：http://hz.chenlongwang.top/gtdnpjonli.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtrrcywrys.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtydyjfxcn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gthngwfang.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gtoqhbfxth.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fengsongda.top/gtmcgaxich.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xylfe.cn/gtyxpwmliq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtkotvidnn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtxwslgjlb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtdjuhqied.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gaohongyu789.top/gtalsvotuu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtbdbcfmcg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtehdzzwiw.html


<!-- 参考信息 -->