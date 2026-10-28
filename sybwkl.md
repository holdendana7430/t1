代发 wailian999

val a = 1;  var b = 2
来源：http://hz.cdnleiting.top/gtnmubfrqt.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtaukfpihh.html

s"值: $b"
来源：http://hz.vqdsnc.cn/gtspwmefyr.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gttltwhhno.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.9152youxi.cn/gtlcvxglcs.html

[T55] Scala：集合过滤
来源：http://hz.0kj1m.cn/gtjeevrpum.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.redwolf501.top/gtfqfsgipd.html

[T56] Scala：样例类
来源：http://hz.chenzaomai.com/gtmnroydnp.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtdlibvwww.html

[T57] Scala：模式匹配
来源：http://hz.zhijiandao.cn/gthgvosadr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cdnleiting.top/gtxmvrymzv.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtksdhykgb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtqemgnmpv.html

[T59] Scala：循环
来源：http://hz.redwolf501.top/gtrbiponzz.html

for (i <- 1 to 10) println(i)
来源：http://hz.svipenyu.cn/gtzaciqwbn.html

[T60] Scala：折叠
来源：http://hz.redwolf501.top/gtrwqqlvzg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhengqikj.top/gtnbggvmee.html

================================================================================
来源：http://hz.kuanghao11.cn/gtulpnwmuj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtxpxdxcbc.html

================================================================================
来源：http://hz.ppjwa.cn/gtgivtsclo.html

[U01] Py：创建虚拟环境
来源：http://hz.sufxvd.cn/gthjvoiafg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shuidangran.top/gtiwjlowhv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xingfuxueyuan.xyz/gtaqlpwxnc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gturzopeuv.html

[U03] Py：加载 .env 配置
来源：http://hz.wangdashe.top/gtrnfgkodf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gtwiohfjhh.html

[U04] Py：变量调试打印
来源：http://hz.jyoumei.cn/gtmhrdrhxl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhixingplan.top/gtxwlyokpv.html

[U05] Py：列表去重且保序
来源：http://hz.52xcode.cn/gtmzvglwhd.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gthhalwluw.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gtypbjieds.html

{**a, **b}
来源：http://hz.bjfxy.top/gtmthzjfrg.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gttyhqwswp.html

{v: k for k, v in d.items()}
来源：http://hz.zdqjudy.top/gtkotamizb.html

[U08] Py：展平二维列表
来源：http://hz.yvedp.cn/gtyxwjqdpq.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtqziepiic.html

[U09] Py：字典取最大值的键
来源：http://hz.havefunace.top/gtuhbrqyug.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gtfunnpgre.html

[U10] Py：按值排序字典
来源：http://hz.hysaishi.cn/gtwlookhfj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sxryk.cn/gtucepburn.html

[U11] Py：生成器表达式
来源：http://hz.cheryme.top/gtdsdttuxu.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtkwmffnnv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.c1oappe.top/gtszfthovl.html

Counter(arr).most_common(3)
来源：http://hz.zycfv.cn/gtwtyctqbn.html

[U13] Py：固定长度队列
来源：http://hz.zhongyouzk.top/gthhgizyek.html

deque(maxlen=10)
来源：http://hz.yuxming.cn/gtcrxhdcjk.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtuocxserm.html

defaultdict(list)
来源：http://hz.zhijiandao.cn/gtersmrcem.html

[U15] Py：高精度计时
来源：http://hz.ywan-chungtsiang.top/gtwlwqvibp.html

t = time.perf_counter()
来源：http://hz.daria6918.cn/gtpxcetfog.html

[U16] Py：命令行参数解析
来源：http://hz.jiagoushi.top/gtqnocutpc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigufen.top/gtxvrcznmz.html

[U17] Py：初始化日志
来源：http://hz.xinyue.icu/gtogjvzyya.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ppjwa.cn/gtiroetmfd.html

[U18] Py：预编译正则
来源：http://hz.yvedp.cn/gtlielibuw.html

pat = re.compile(r"\d+")
来源：http://hz.ivvv.top/gtfmtdjrkn.html

[U19] Py：正则替换带回调
来源：http://hz.hfpthk.cn/gtnroambzy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yuanzhike.top/gtgzjskjnn.html

[U20] Py：缓存函数结果
来源：http://hz.nwbrower.top/gtquqfieom.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hammf.cn/gtmdwmatte.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydzc1.top/gtuteistct.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangkeji.top/gtvrivrtgv.html

[U22] Py：矩阵转置
来源：http://hz.tian-w.cn/gtzcsdowev.html

list(zip(*m))
来源：http://hz.snrcjt.cn/gtyxokzhwi.html

[U23] Py：分块读取大文件
来源：http://hz.pengpengdd.cyou/gtabfkjzus.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnxiangtu.top/gtvbgdwmol.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtsubbkjfn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigufen.top/gtjvnigwor.html

[U25] Py：CSV 按字典读
来源：http://hz.316326.xyz/gtfsvtyyut.html

csv.DictReader(f)
来源：http://hz.sufxvd.cn/gtlvabmjqo.html

[U26] Py：并发下载
来源：http://hz.hnqzz.top/gtdpgukcsx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtfdraxloc.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gtyocznzdi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.52xcode.cn/gtphtjlttx.html

[U28] Py：类型别名
来源：http://hz.jinyuanbaomall.cn/gtweubnupg.html

UserId = int
来源：http://hz.cdnleiting.top/gtbomwfpro.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gthmupchpz.html

@property 与 @x.setter 配合
来源：http://hz.bjfxy.top/gtybjpyrhq.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtfobpdjdl.html

@dataclass(slots=True)
来源：http://hz.nanxinkj.top/gtmyovqpic.html

[U31] Py：单测
来源：http://hz.shanyushiyangkeji.top/gthyeggpbv.html

python -m pytest -q
来源：http://hz.nanxuanxn.top/gttuzvsonf.html

[U32] Py：代码格式化
来源：http://hz.yongpay.top/gtlqsiykab.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258888.top/gtqudnpyty.html

[U33] Py：打包发布
来源：http://hz.guannengcc.top/gtzzjntjua.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangdashe.top/gtgkdbmffh.html

[U34] Py：判断编码
来源：http://hz.zhijiandao.cn/gtzeninxla.html

chardet.detect(raw)
来源：http://hz.pengpengdd.cyou/gtdkruotht.html

[U35] Py：发送邮件
来源：http://hz.bjfxy.top/gtuvnwzyng.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hfpthk.cn/gtnackllwu.html

[U36] Py：定时任务
来源：http://hz.zhaomingkeji.xyz/gtdabwyviu.html

schedule.every(10).minutes.do(job)
来源：http://hz.jyoumei.cn/gtkmwguwgn.html

[U37] Py：读写 Excel
来源：http://hz.kuanghao11.cn/gtppbmkouu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtadxhxqzp.html

[U38] Py：获取脚本所在目录
来源：http://hz.c1oappe.top/gtrfaqpnjq.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gteovnvnry.html

[U39] Py：判断是否在交互环境
来源：http://hz.tanke756.top/gtdiegfgak.html

sys.stdout.isatty()
来源：http://hz.sxryk.cn/gtmhqfzqej.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtzhlbhqzi.html

print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gttuzsvmjj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shangyingyoupin.top/gtnrmtqfnn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhijiandao.cn/gtejpldyms.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aibaodan.cn/gtybqvuokx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jianghu66.top/gtwcksqzyb.html

[U43] PHP：声明命名空间
来源：http://hz.yuxming.cn/gtleubtdjl.html

namespace App\Http;
来源：http://hz.yonumen.top/gtxaoipjth.html

[U44] PHP：开启严格类型
来源：http://hz.zhixingplan.top/gtfseobttd.html

declare(strict_types=1);
来源：http://hz.zhengqikj.top/gtseflstnh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangkeji.top/gtxdybfvos.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtpllwzjxu.html

[U46] PHP：可空类型
来源：http://hz.yanxiufei.cn/gtbxxtmgbu.html

?string $name = null
来源：http://hz.zycfv.cn/gthbtlyldw.html

[U47] PHP：联合类型
来源：http://hz.xinyue.icu/gtohwyeiat.html

int|string $id
来源：http://hz.gotoacloud.top/gtlazubdyw.html

[U48] PHP：纯枚举
来源：http://hz.tanke756.top/gtwrxkvssd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jqgufenzy.top/gthpwlizam.html

[U49] PHP：只读属性
来源：http://hz.jianghu66.top/gtfbhipnbq.html

public readonly string $name
来源：http://hz.mhx1999.top/gtispkmqve.html

[U50] PHP：构造器属性提升
来源：http://hz.cashguo.top/gtnxkfeghs.html

public function __construct(private int $id) {}
来源：http://hz.zhongyouzk.top/gtrscpirka.html

[U51] PHP：数组解构
来源：http://hz.xuetiantiany.cn/gtxvaehhpm.html

[$a, $b] = $arr;
来源：http://hz.xuetiantiany.cn/gtxaqcyukc.html

[U52] PHP：箭头函数
来源：http://hz.mhx1999.top/gtidhwkscf.html

$double = fn($x) => $x * 2;
来源：http://hz.yj202588.top/gtyeyjdufx.html

[U53] PHP：空合并运算符
来源：http://hz.gzhubu.top/gtisrvjkzq.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtbpkyogpy.html

[U54] PHP：空安全调用
来源：http://hz.redwolf501.top/gtldwimbop.html

$obj?->method()
来源：http://hz.ywan-chungtsiang.top/gtfwxejyrr.html

[U55] PHP：match 表达式
来源：http://hz.daxiang520.top/gttfbgyzxf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yanxiufei.cn/gtefwerylc.html

[U56] PHP：命名参数
来源：http://hz.ybcxt.top/gtgxjahwgy.html

f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtfpoxkeib.html

[U57] PHP：字符串插值
来源：http://hz.mhx1999.top/gtvcfnefey.html

"值: {$a}"
来源：http://hz.redwolf501.top/gtsdadgdxn.html

[U58] PHP：数组三件套
来源：http://hz.pengpengdd.cyou/gtrlbsunkn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cheryme.top/gtkqdaloxk.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtymvyuqch.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gthqyvqtnn.html

[U60] PHP：JSON 编解码
来源：http://hz.guannengcc.top/gtdqtwvwyn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cashguo.top/gtsutfrfwc.html

[U61] PHP：正则
来源：http://hz.ydjk.org.cn/gttgqopxei.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtnkytzhpo.html

[U62] PHP：日期对象
来源：http://hz.gaohongyu789.top/gtmhwnlfms.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghu66.top/gtwpmlvhfm.html

[U63] PHP：文件读写
来源：http://hz.iojbl.cn/gtwjiuhrmh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhijiandao.cn/gtwmznpwgr.html

[U64] PHP：目录遍历
来源：http://hz.hongshengwenyu.top/gtifjdxwdi.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yangfankeji.com/gttciurrpr.html

[U65] PHP：会话
来源：http://hz.snrcjt.cn/gtuuaokhrb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnxiangtu.top/gtwixhazyv.html

[U66] PHP：设置 Cookie
来源：http://hz.cheryme.top/gttpkqojzr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xylfe.cn/gtizgmkufb.html

[U67] PHP：处理文件上传
来源：http://hz.guowangkeji.top/gtncptcvgt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ywan-chungtsiang.top/gtfkbdgqzu.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gttsjkwwpj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.iojbl.cn/gtosayuszz.html

[U69] PHP：PDO 预处理
来源：http://hz.guannengcc.top/gtfotaabca.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dashuyun.cn/gtxtbjkpxm.html

[U70] PHP：PDO 事务
来源：http://hz.yangfankeji.com/gtpatwdhzo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.vqdsnc.cn/gtpalvvioy.html

[U71] PHP：抛出异常
来源：http://hz.snrcjt.cn/gtgjkpdubd.html

throw new RuntimeException("失败", 500);
来源：http://hz.hnqzz.top/gtfcibarhk.html

[U72] PHP：写错误日志
来源：http://hz.wangshuangyany.cn/gtfxskwqzx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jqgfzy.top/gtvxkgdicd.html

[U73] PHP：读取 ini 配置
来源：http://hz.shuidangran.top/gtzblgocue.html

parse_ini_file("config.ini", true)
来源：http://hz.ybcxt.top/gtlcwjxanr.html

[U74] PHP：读取环境变量
来源：http://hz.tianlin.xyz/gtfyxzvkkb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.havefunace.top/gtmzlaskta.html

[U75] PHP：依赖注入
来源：http://hz.birdmap.top/gtqaygubuc.html

composer require psr/container
来源：http://hz.birdmap.top/gtzqpmghop.html

[U76] PHP：简单路由
来源：http://hz.hammf.cn/gtemuefppc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jyoumei.cn/gtoasfujoi.html

[U77] PHP：模板渲染
来源：http://hz.sweek.top/gthvrmapqo.html

composer require twig/twig
来源：http://hz.andypj.xyz/gtnswlvusl.html

[U78] PHP：单元测试
来源：http://hz.redwolf501.top/gtsdzstdup.html

composer require --dev phpunit/phpunit
来源：http://hz.hammf.cn/gtobkuqtoz.html

[U79] PHP：静态分析
来源：http://hz.nwbrower.top/gtqfmvzurg.html

composer require --dev phpstan/phpstan
来源：http://hz.mhx1999.top/gtkofrpzmt.html

[U80] PHP：代码规范修复
来源：http://hz.smart0.xyz/gtrrxvzurg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangshuangyany.cn/gtbuistwsp.html

[U81] JS：初始化项目
来源：http://hz.xinyue.icu/gtlcrjuaoq.html

npm init -y;  npm i express
来源：http://hz.nanxuanxn.top/gtrqkylohh.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258888.top/gtkzcplgma.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hammf.cn/gtzxdpqfzw.html

[U83] JS：ES Module 导入导出
来源：http://hz.hfpthk.cn/gtoxtnwmtc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.wangshuangyany.cn/gtgmsxfjiw.html

[U84] JS：CommonJS 写法
来源：http://hz.shzxlz.cn/gtgougvpwf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gzhubu.top/gtcjvvpuzx.html

[U85] JS：可选链
来源：http://hz.jinqigufen.top/gtctxbnaie.html

a?.b?.c
来源：http://hz.ppjwa.cn/gtoelipnud.html

[U86] JS：空值合并
来源：http://hz.svipenyu.cn/gtrkcxwxui.html

a ?? b
来源：http://hz.cucudq.cn/gtjdqwfnsn.html

[U87] JS：解构默认值
来源：http://hz.ppjwa.cn/gtqaztdarv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jiagoushi.top/gtqtqirjqt.html

[U88] JS：对象展开合并
来源：http://hz.feifeiyinyue.top/gtjejgnpbg.html

{ ...a, ...b }
来源：http://hz.yongpay.top/gtcelnhdbh.html

[U89] JS：数组去重
来源：http://hz.gzhubu.top/gticoncyuu.html

[...new Set(arr)]
来源：http://hz.jiagoushi.top/gtzlcnsgal.html

[U90] JS：数字数组排序
来源：http://hz.quarkkingdee.top/gtksmblvwg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtlscmsszy.html

[U91] JS：对象键值遍历
来源：http://hz.ydjk.org.cn/gtwncubfuu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258.top/gtlkknjovq.html

[U92] JS：深拷贝
来源：http://hz.dianchejie.cn/gtnxpgvkcv.html

structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtvxgxnyzb.html

[U93] JS：模板字符串
来源：http://hz.birdmap.top/gtyxhssjpi.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtezsivvgg.html

[U94] JS：箭头函数
来源：http://hz.sweek.top/gtbfrnieig.html

const double = x => x * 2;
来源：http://hz.jlsjyb.cn/gtjefmmenc.html

[U95] JS：Promise 包装
来源：http://hz.nanxinkj.top/gtaoqplqcs.html

new Promise((resolve, reject) => {})
来源：http://hz.gotoacloud.top/gtzyuqmllx.html

[U96] JS：async/await 与异常
来源：http://hz.xinyue.icu/gtuqdzljrb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gttmneefza.html

[U97] JS：并发请求
来源：http://hz.yj20258.top/gtaikwwywa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtcyyjehvm.html

[U98] JS：fetch 带 JSON
来源：http://hz.sweek.top/gtkxekcggn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ydzc1.top/gtioqeotwj.html

[U99] JS：事件监听
来源：http://hz.zhijiandao.cn/gtxkmvxwqv.html

el.addEventListener("click", e => {})
来源：http://hz.guowangkeji.top/gtiztqhvfw.html

[U100] JS：DOM 查询
来源：http://hz.yuanzhike.top/gtcutdozhn.html

document.querySelector(".item")
来源：http://hz.zhiwuduotai.top/gtwjucttek.html

[U101] JS：classList 操作
来源：http://hz.nanxuanxn.top/gtwctrcyji.html

el.classList.toggle("active")
来源：http://hz.vqdsnc.cn/gtstotyjxq.html

[U102] JS：本地存储
来源：http://hz.yanxiufei.cn/gttatqqfoz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhiwuduotai.top/gtdarbfayt.html

[U103] JS：定时器
来源：http://hz.yuanzhike.top/gtujjmgbiq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xingfuxueyuan.xyz/gtoxlnuozt.html

[U104] JS：防抖
来源：http://hz.kuanghao11.cn/gtzylhqzmy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtlmqztale.html

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtjmxkdgky.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yvedp.cn/gtnlsegxrp.html

[U106] JS：日期格式化
来源：http://hz.gotoacloud.top/gtoygtdyrx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jyoumei.cn/gtlpuwntee.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtlfrovuvu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ppjwa.cn/gtehnfjqkb.html

[U108] JS：随机整数
来源：http://hz.c1oappe.top/gtrtqcdjzh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.quarkkingdee.top/gtmjinfril.html

[U109] JS：数组分组
来源：http://hz.zhaomingkeji.xyz/gtfpxsiega.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtjevyscft.html

[U110] JS：数组分块
来源：http://hz.yuanzhike.top/gtdekttuwo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.andypj.xyz/gtakaxzgii.html

[U111] JS：对象转 Map
来源：http://hz.quarkkingdee.top/gtuddrktel.html

new Map(Object.entries(obj))
来源：http://hz.shzxlz.cn/gtmnfdsfsi.html

[U112] JS：字符串补位
来源：http://hz.xingfuxueyuan.xyz/gthnnpgkgz.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtijlrqkwt.html

[U113] JS：正则替换全部
来源：http://hz.yvedp.cn/gtpznutnba.html

s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtdtuzoyxp.html

[U114] JS：JSON 深比较
来源：http://hz.zhijiandao.cn/gtoddvzwzs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtqlubduld.html

[U115] JS：生成 UUID
来源：http://hz.andypj.xyz/gtlxprhnvt.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtcbuhjjrp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.316326.xyz/gtrahibgeu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cashguo.top/gtxosatmah.html

[U117] JS：单元测试
来源：http://hz.birdmap.top/gtzidtlvcz.html

npm i -D vitest;  npx vitest
来源：http://hz.yj20258.top/gtxperqqno.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtgoovdcpy.html

npm i -D vite;  npx vite
来源：http://hz.ppjwa.cn/gttonudwke.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gtprllcxew.html

npx vite build
来源：http://hz.dianchejie.cn/gthnjfzbhy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtitvbdnyu.html

import.meta.env.VITE_API_URL
来源：http://hz.sysykeji.top/gttqbpjctq.html

================================================================================
来源：http://hz.daxiang520.top/gtsytgrxhl.html

统计汇总
来源：http://hz.wangdashe.top/gtczfnpiyl.html

================================================================================
来源：http://hz.ppjwa.cn/gtsnxdjnfu.html

按语言统计（条）：
来源：http://hz.shanyushiyangtech.top/gtqrckknzh.html

Python ......... 252
来源：http://hz.yonumen.top/gtfmjkzepu.html

PHP ............ 252
来源：http://hz.cashguo.top/gtxjlsqnno.html

JavaScript ..... 252
来源：http://hz.mhx1999.top/gtvkstsdsp.html

TypeScript ..... 212
来源：http://hz.yj20258888.top/gtvkkqcmdr.html

Java ........... 212
来源：http://hz.havefunace.top/gtiqctomvr.html

Go ............. 212
来源：http://hz.zhijiandao.cn/gtegtrpvkv.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtnrpfbybp.html

C# ............. 212
来源：http://hz.xuetiantiany.cn/gteqocgvwm.html

C .............. 30
来源：http://hz.hywenlv.cn/gtlttzkuon.html

C++ ............ 30
来源：http://hz.cheryme.top/gtafmvdoxs.html

SQL ............ 90
来源：http://hz.cheryme.top/gtbtypoqiz.html

Bash ........... 80
来源：http://hz.9152youxi.cn/gtndoscion.html

Kotlin ......... 15
来源：http://hz.nanxinkj.top/gtowywinql.html

Swift .......... 15
来源：http://hz.aibaodan.cn/gtwolzslos.html

Lua ............ 10
来源：http://hz.sweek.top/gtoqmsoqun.html

Perl ........... 10
来源：http://hz.jqgfzy.top/gtdpzpqnqe.html

Scala .......... 10
来源：http://hz.chenlongwang.top/gtvmlrlfvz.html

------------------------------------
来源：http://hz.tianlin.xyz/gtxhidqkmb.html

合计 ........... 2106 条
来源：http://hz.sweek.top/gtynhcfybl.html

按章节统计：
来源：http://hz.xylfe.cn/gtjupgrklu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtoslqvyeg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gtzbyqaqmr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtrjoeraua.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.tian-w.cn/gtghnwkqhh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.svipenyu.cn/gtxrtbcaxg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtudyktcmk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtcamrohqc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtqkhqvtur.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtgiqapsdn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.pycfn.com/gtohyfjcqn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtibvikpin.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtmyemsvse.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gteutlzugt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtgygjnsgj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.0kj1m.cn/gtibisawrm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtybarwzpf.html


<!-- 参考信息 -->