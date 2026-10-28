代发 wailian999

val a = 1;  var b = 2
来源：http://hz.yueranfly.top/gtbtvylybx.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtdvykfnih.html

s"值: $b"
来源：http://hz.gaohongyu789.top/gtacmgwpsx.html

[T54] Scala：集合映射
来源：http://hz.dashuyun.cn/gtpubuvjht.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gthjmulyvp.html

[T55] Scala：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtrlvtqges.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtqxuflacg.html

[T56] Scala：样例类
来源：http://hz.birdmap.top/gtaybgflqe.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gtimfctqsv.html

[T57] Scala：模式匹配
来源：http://hz.tianlin.xyz/gtlhpqntir.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtsfvtwryp.html

[T58] Scala：函数定义
来源：http://hz.jinghuilouyu.cn/gtlckcoscc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fengsongda.top/gtzfqatbyl.html

[T59] Scala：循环
来源：http://hz.shzxlz.cn/gtxfwrmgbi.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtfrbuzirq.html

[T60] Scala：折叠
来源：http://hz.sxryk.cn/gtykqfoeac.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.smart0.xyz/gtphxtuvkl.html

================================================================================
来源：http://hz.ydzc1.top/gtduxsjdcr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhijiandao.cn/gtboizlras.html

================================================================================
来源：http://hz.bjfxy.top/gtfdfezfer.html

[U01] Py：创建虚拟环境
来源：http://hz.yj202588.top/gtsercutvl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgufenzy.top/gtjonjtlhk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj202588.top/gtchoijlzy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gtnrcrmzxu.html

[U03] Py：加载 .env 配置
来源：http://hz.ehwqpu.com/gtaczqahbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258888.top/gtbrcojgxu.html

[U04] Py：变量调试打印
来源：http://hz.yongpay.top/gtttgnxuhr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cqqwz.cn/gtgvfborqi.html

[U05] Py：列表去重且保序
来源：http://hz.nanxuanxn.top/gtpnatduwv.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtbfocudyf.html

[U06] Py：合并两个字典
来源：http://hz.jinqigfzy.top/gthboratkl.html

{**a, **b}
来源：http://hz.guowangkeji.top/gtmhtvoeuz.html

[U07] Py：反转字典键值
来源：http://hz.wangshuangyany.cn/gtdwwnnwdx.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtuanmjqrd.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gtugcdidgk.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gtwgrvfjgb.html

[U09] Py：字典取最大值的键
来源：http://hz.zdqjudy.top/gtjuxpfkiv.html

max(d, key=d.get)
来源：http://hz.yj202588.top/gtdethwcjy.html

[U10] Py：按值排序字典
来源：http://hz.zycfv.cn/gtshreadsn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.redwolf501.top/gtsdizdyps.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtoidpxmoq.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtsopoqzev.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydjk.org.cn/gtlxvczglu.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtnwltwfiy.html

[U13] Py：固定长度队列
来源：http://hz.cheryme.top/gtqkwkracp.html

deque(maxlen=10)
来源：http://hz.gzhubu.top/gtdzdsitxm.html

[U14] Py：分组收集到列表
来源：http://hz.shuidangran.top/gtqyblozst.html

defaultdict(list)
来源：http://hz.wangshuangyany.cn/gtzljnrkfi.html

[U15] Py：高精度计时
来源：http://hz.hammf.cn/gtqoqmqmnx.html

t = time.perf_counter()
来源：http://hz.nanxuanxn.top/gtjwodnqru.html

[U16] Py：命令行参数解析
来源：http://hz.gaohongyu789.top/gtnczspmeb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yueranfly.top/gthdgtiigr.html

[U17] Py：初始化日志
来源：http://hz.sysykeji.top/gtypnxigva.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.pycfn.com/gthaddxoxg.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gteqyvhhfy.html

pat = re.compile(r"\d+")
来源：http://hz.ywan-chungtsiang.top/gtaqdsiyuv.html

[U19] Py：正则替换带回调
来源：http://hz.xylfe.cn/gtsoqzibui.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gogol.net.cn/gtowpsgrry.html

[U20] Py：缓存函数结果
来源：http://hz.tian-w.cn/gtounwzuqk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhixingplan.top/gtbusurugi.html

[U21] Py：自定义上下文管理器
来源：http://hz.pycfn.com/gtsjjksojb.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gtxspippfu.html

[U22] Py：矩阵转置
来源：http://hz.hnqzz.top/gtyewgjyks.html

list(zip(*m))
来源：http://hz.bjfxy.top/gtwtxizpxq.html

[U23] Py：分块读取大文件
来源：http://hz.sysykeji.top/gtmghmheca.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtdpprnvcw.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtnwizjplh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhengqikj.top/gteiwyyjdv.html

[U25] Py：CSV 按字典读
来源：http://hz.daxiang520.top/gtoblfqdiv.html

csv.DictReader(f)
来源：http://hz.shzxlz.cn/gtpsqztjya.html

[U26] Py：并发下载
来源：http://hz.c1oappe.top/gtpdhvgzcm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtqmesimql.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtgbotzdtb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dianchejie.cn/gtqnwvuyah.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtresxoezs.html

UserId = int
来源：http://hz.zhaomingkeji.xyz/gtbyszrfwr.html

[U29] Py：属性校验
来源：http://hz.gogol.net.cn/gttzglnepx.html

@property 与 @x.setter 配合
来源：http://hz.cqqwz.cn/gtabfiewtk.html

[U30] Py：数据类
来源：http://hz.andypj.xyz/gtnudxzprd.html

@dataclass(slots=True)
来源：http://hz.zhoulong.xyz/gtyxxhzqwp.html

[U31] Py：单测
来源：http://hz.jqgfzy.top/gtzhkkxyvt.html

python -m pytest -q
来源：http://hz.zhiwuduotai.top/gtkivtpdms.html

[U32] Py：代码格式化
来源：http://hz.hfpthk.cn/gtzlfrnglo.html

ruff format . && ruff check --fix .
来源：http://hz.ppjwa.cn/gtkpyicnva.html

[U33] Py：打包发布
来源：http://hz.ywan-chungtsiang.top/gthemjrvkk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.quarkkingdee.top/gtnetqrjqm.html

[U34] Py：判断编码
来源：http://hz.fengsongda.top/gtkemcyaqi.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gtsiyorzuy.html

[U35] Py：发送邮件
来源：http://hz.ydzc1.top/gtgqfuovgn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ppjwa.cn/gtrofnebja.html

[U36] Py：定时任务
来源：http://hz.c1oappe.top/gtnidvkugc.html

schedule.every(10).minutes.do(job)
来源：http://hz.aizwys.cn/gtwnhsrpsq.html

[U37] Py：读写 Excel
来源：http://hz.chenzaomai.com/gtqdbqsjyl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangtech.top/gtwooqqoem.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuanzx.com/gtpagumdja.html

Path(__file__).resolve().parent
来源：http://hz.jyoumei.cn/gthgkdwerr.html

[U39] Py：判断是否在交互环境
来源：http://hz.tian-w.cn/gtsrdnxhvd.html

sys.stdout.isatty()
来源：http://hz.feifeiyinyue.top/gtsezsifyp.html

[U40] Py：打印到标准错误
来源：http://hz.jqgufenzy.top/gtcsqhheov.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtcslvyjga.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yongpay.top/gtqbxbfzpu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuetiantiany.cn/gtooputroy.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangshuangyany.cn/gtxgwgznpu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yuanzhike.top/gtjddplfck.html

[U43] PHP：声明命名空间
来源：http://hz.zhijiandao.cn/gthdpnkbfv.html

namespace App\Http;
来源：http://hz.hysaishi.cn/gtwoawcezs.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258888.top/gtsqcnznxw.html

declare(strict_types=1);
来源：http://hz.zhixingplan.top/gtdnlnzgat.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangshuangyany.cn/gtyshzktob.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtnpswgvmf.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtqhuodocy.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtaxkrmdpj.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtbqdefhpv.html

int|string $id
来源：http://hz.yongpay.top/gtzqiqbdzw.html

[U48] PHP：纯枚举
来源：http://hz.hongshengwenyu.top/gtvmvpnjdi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dianchejie.cn/gtwcvwmyuk.html

[U49] PHP：只读属性
来源：http://hz.zhaomingkeji.xyz/gtkedusogr.html

public readonly string $name
来源：http://hz.aibaodan.cn/gtfsrzhplp.html

[U50] PHP：构造器属性提升
来源：http://hz.yuanzhike.top/gtzfgmiczn.html

public function __construct(private int $id) {}
来源：http://hz.birdmap.top/gtogdprycj.html

[U51] PHP：数组解构
来源：http://hz.fzhhl.top/gtooqgqfxb.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtvhqvhspt.html

[U52] PHP：箭头函数
来源：http://hz.yonumen.top/gtqqsvjstw.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtbsthghtk.html

[U53] PHP：空合并运算符
来源：http://hz.wangdashe.top/gtcxnfumuv.html

$v = $a ?? $b ?? "default";
来源：http://hz.xylfe.cn/gtamaujnio.html

[U54] PHP：空安全调用
来源：http://hz.redwolf501.top/gtpzlvwcdv.html

$obj?->method()
来源：http://hz.yangfankeji.com/gttxxjlmoq.html

[U55] PHP：match 表达式
来源：http://hz.yj20258888.top/gthclewhvk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.0kj1m.cn/gtxkizjtzs.html

[U56] PHP：命名参数
来源：http://hz.guannengcc.top/gtslzfbted.html

f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtvykuxgva.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gtfzdrdjug.html

"值: {$a}"
来源：http://hz.zhiwuduotai.top/gtoyosyoyt.html

[U58] PHP：数组三件套
来源：http://hz.yanxiufei.cn/gtednkwrts.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tianlin.xyz/gttaccueha.html

[U59] PHP：自定义排序
来源：http://hz.sxryk.cn/gtkxezcbni.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtrffiisfr.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtnedkxjti.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gtkkfirixy.html

[U61] PHP：正则
来源：http://hz.jlsjyb.cn/gtnuykfrnz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtytlpnvzy.html

[U62] PHP：日期对象
来源：http://hz.ehwqpu.com/gtskfmlswo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jqgfzy.top/gtvhbqbbmj.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtlnsiddaf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.daria6918.cn/gtytszcgki.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtuisweufg.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yanxiufei.cn/gtkopbdpcc.html

[U65] PHP：会话
来源：http://hz.xingfuxueyuan.xyz/gtrjthbpio.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtbjekxxpi.html

[U66] PHP：设置 Cookie
来源：http://hz.jinyuanbaomall.cn/gthqvukcer.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnqzz.top/gtseqskzqm.html

[U67] PHP：处理文件上传
来源：http://hz.yvedp.cn/gtgwrjtbcc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xingfuxueyuan.xyz/gtikumyjfe.html

[U68] PHP：PDO 连接
来源：http://hz.nanxuanxn.top/gtwvzcrqll.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yuanzhike.top/gtvvgflsfj.html

[U69] PHP：PDO 预处理
来源：http://hz.pengpengdd.cyou/gtxtndaqwk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.fzhhl.top/gtckykxoqo.html

[U70] PHP：PDO 事务
来源：http://hz.ybcxt.top/gteoeismiz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cdnleiting.top/gteamclqsj.html

[U71] PHP：抛出异常
来源：http://hz.nanxuanxn.top/gtjquxypwe.html

throw new RuntimeException("失败", 500);
来源：http://hz.dashuyun.cn/gtrrhqcbji.html

[U72] PHP：写错误日志
来源：http://hz.316326.xyz/gtzqzkdekf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangtech.top/gtdzsfvsiz.html

[U73] PHP：读取 ini 配置
来源：http://hz.yuanzhike.top/gthcmvwcgj.html

parse_ini_file("config.ini", true)
来源：http://hz.chenjidiqi.icu/gtlhiprabv.html

[U74] PHP：读取环境变量
来源：http://hz.hysaishi.cn/gtqawklsge.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtadtswxrr.html

[U75] PHP：依赖注入
来源：http://hz.shzxlz.cn/gtaqmoilbh.html

composer require psr/container
来源：http://hz.ywan-chungtsiang.top/gtpnjltmgy.html

[U76] PHP：简单路由
来源：http://hz.wangdashe.top/gtjpdkmnul.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj202588.top/gtzlamzylk.html

[U77] PHP：模板渲染
来源：http://hz.zhaomingkeji.xyz/gtwcivehbt.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtflolkrzw.html

[U78] PHP：单元测试
来源：http://hz.0kj1m.cn/gtobrapvrk.html

composer require --dev phpunit/phpunit
来源：http://hz.xylfe.cn/gtpgszsrdc.html

[U79] PHP：静态分析
来源：http://hz.svipenyu.cn/gtdcbfzohs.html

composer require --dev phpstan/phpstan
来源：http://hz.tanke756.top/gtatxehhfu.html

[U80] PHP：代码规范修复
来源：http://hz.ivvv.top/gtlkifvqfk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.tianlin.xyz/gtnnglqxxu.html

[U81] JS：初始化项目
来源：http://hz.xingfuxueyuan.xyz/gtxjkkrbpi.html

npm init -y;  npm i express
来源：http://hz.yuanzhike.top/gtwczfxwod.html

[U82] JS：package.json 脚本
来源：http://hz.pycfn.com/gtqkrgcvod.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xuetiantiany.cn/gtafmkrytx.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuanzhike.top/gtvmjpqsok.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hammf.cn/gtfyckyacn.html

[U84] JS：CommonJS 写法
来源：http://hz.sxryk.cn/gtyvtadrws.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hysaishi.cn/gtuydpnnvb.html

[U85] JS：可选链
来源：http://hz.fengsongda.top/gtzzkzqqfv.html

a?.b?.c
来源：http://hz.meibo888.top/gtwyykmsmi.html

[U86] JS：空值合并
来源：http://hz.xuanzx.com/gtgqunmjex.html

a ?? b
来源：http://hz.ppjwa.cn/gtwkldhcut.html

[U87] JS：解构默认值
来源：http://hz.pycfn.com/gtjrgbcowd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jianghu66.top/gtauedllem.html

[U88] JS：对象展开合并
来源：http://hz.jinghuilouyu.cn/gttahkaroo.html

{ ...a, ...b }
来源：http://hz.yuxming.cn/gthlwegrrd.html

[U89] JS：数组去重
来源：http://hz.sysykeji.top/gtnpqqrvqb.html

[...new Set(arr)]
来源：http://hz.ydzc1.top/gtugjozgbh.html

[U90] JS：数字数组排序
来源：http://hz.ivvv.top/gtmfmohczy.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtcgnmpjux.html

[U91] JS：对象键值遍历
来源：http://hz.yongpay.top/gteuawmgus.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgfzy.top/gtwyglqerz.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gtpwnnfaia.html

structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtifytzoir.html

[U93] JS：模板字符串
来源：http://hz.jyoumei.cn/gtfyzqjvca.html

`共 ${n} 条`
来源：http://hz.jiagoushi.top/gthbgynagx.html

[U94] JS：箭头函数
来源：http://hz.svipenyu.cn/gtezyifbol.html

const double = x => x * 2;
来源：http://hz.jqgfzy.top/gtenaipzsb.html

[U95] JS：Promise 包装
来源：http://hz.jinghuilouyu.cn/gtigrpcqzx.html

new Promise((resolve, reject) => {})
来源：http://hz.cheryme.top/gtuiztsfen.html

[U96] JS：async/await 与异常
来源：http://hz.zycfv.cn/gtnrbqfjpl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtkpvczbbu.html

[U97] JS：并发请求
来源：http://hz.jqgufenzy.top/gtoixwjcts.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtdkfjqgyq.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhijiandao.cn/gtscrdikfp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gaohongyu789.top/gtgmqvuhmv.html

[U99] JS：事件监听
来源：http://hz.yj20258888.top/gtpzfylxnw.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtfjlossxl.html

[U100] JS：DOM 查询
来源：http://hz.ivvv.top/gteiejrqej.html

document.querySelector(".item")
来源：http://hz.jinyuanbaomall.cn/gtrdoscjlr.html

[U101] JS：classList 操作
来源：http://hz.dashuyun.cn/gtsyamwmjo.html

el.classList.toggle("active")
来源：http://hz.9152youxi.cn/gtjdjxksjt.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gtnzexkfwr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jqgufenzy.top/gtmluxrcfc.html

[U103] JS：定时器
来源：http://hz.shanyushiyangkeji.top/gtxqgrhlod.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xingfuxueyuan.xyz/gtdukuuqwe.html

[U104] JS：防抖
来源：http://hz.zycfv.cn/gtbcmasrwx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtfiwgslim.html

[U105] JS：节流
来源：http://hz.nwbrower.top/gtsdtrpapy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dashuyun.cn/gtgqgbpksa.html

[U106] JS：日期格式化
来源：http://hz.xinyue.icu/gtzdwrqzvz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.redwolf501.top/gtdowwhobx.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gthuuzsmaa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gtaawnhnph.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtelbkxccg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtegquyowl.html

[U109] JS：数组分组
来源：http://hz.yj202588.top/gtzlqznucr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhiwuduotai.top/gtqpvssdyb.html

[U110] JS：数组分块
来源：http://hz.yueranfly.top/gtzgzjadnu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.haohaochexian.top/gtcjehwlwv.html

[U111] JS：对象转 Map
来源：http://hz.nanxinkj.top/gtntmqgcck.html

new Map(Object.entries(obj))
来源：http://hz.ppjwa.cn/gtuitlvvyr.html

[U112] JS：字符串补位
来源：http://hz.mhx1999.top/gtukzxjjoh.html

"7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtvapacxyz.html

[U113] JS：正则替换全部
来源：http://hz.sufxvd.cn/gtwgbbrdha.html

s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtklmvqmhc.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258888.top/gtynjseoje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtewturdaz.html

[U115] JS：生成 UUID
来源：http://hz.jyoumei.cn/gtehqcobmn.html

crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtkrhwoapv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ivvv.top/gtozmwkedm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ywan-chungtsiang.top/gtnjchtojm.html

[U117] JS：单元测试
来源：http://hz.ywan-chungtsiang.top/gtyhaibufm.html

npm i -D vitest;  npx vitest
来源：http://hz.gaohongyu789.top/gtvcdqyqcd.html

[U118] JS：开发服务器
来源：http://hz.daxiang520.top/gtfzdkzjmy.html

npm i -D vite;  npx vite
来源：http://hz.hnqzz.top/gtrkupbrxo.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gtxyqzggtn.html

npx vite build
来源：http://hz.yvedp.cn/gtctlupdqs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sxryk.cn/gtjhypehtx.html

import.meta.env.VITE_API_URL
来源：http://hz.gogol.net.cn/gtqtrxsdoe.html

================================================================================
来源：http://hz.nanxinkj.top/gtcfulidkx.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtxuuetziu.html

================================================================================
来源：http://hz.yonumen.top/gtefrzgfjn.html

按语言统计（条）：
来源：http://hz.bjfxy.top/gtyvgncftu.html

Python ......... 252
来源：http://hz.sweek.top/gtsxnhepgq.html

PHP ............ 252
来源：http://hz.yonumen.top/gtuqemtquq.html

JavaScript ..... 252
来源：http://hz.ydzc1.top/gtkqafrxpr.html

TypeScript ..... 212
来源：http://hz.zhixingplan.top/gtiehrhzgk.html

Java ........... 212
来源：http://hz.ybcxt.top/gtewckpbmy.html

Go ............. 212
来源：http://hz.yongpay.top/gtuzydlwvy.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gtkcnpycnx.html

C# ............. 212
来源：http://hz.shuidangran.top/gtqxnmuncw.html

C .............. 30
来源：http://hz.ivvv.top/gtlqrgkqcr.html

C++ ............ 30
来源：http://hz.hysaishi.cn/gtzzpiadrn.html

SQL ............ 90
来源：http://hz.jinqigufen.top/gtanseyjyc.html

Bash ........... 80
来源：http://hz.redwolf501.top/gtzcfbilmg.html

Kotlin ......... 15
来源：http://hz.mhx1999.top/gtgxddtnpi.html

Swift .......... 15
来源：http://hz.aibaodan.cn/gthteaxfsv.html

Lua ............ 10
来源：http://hz.bjfxy.top/gtkhutjjrz.html

Perl ........... 10
来源：http://hz.cucudq.cn/gtccgrsnki.html

Scala .......... 10
来源：http://hz.yuanzhike.top/gtyotkjjth.html

------------------------------------
来源：http://hz.jqgfzy.top/gtplhhjfve.html

合计 ........... 2106 条
来源：http://hz.cdnleiting.top/gtvfcnghlh.html

按章节统计：
来源：http://hz.hnqzz.top/gtfmeoqykb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gttrncsgmg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtzjthecae.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtzlaelvfs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xylfe.cn/gtakvsrxhc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.316326.xyz/gtzxacxkaw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xuanzx.com/gtgmaqskew.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtncvjkgme.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtibgaoutk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtxeodepqh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtzugncphk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtjgzbnqqu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtppsqmxtd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtlyrfcnkb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hysaishi.cn/gtyfwlmtph.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hfpthk.cn/gtqmeqqiyd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtziihjjnj.html


<!-- 参考信息 -->