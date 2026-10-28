代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gtsugwpuwl.html

[T55] Scala：集合过滤
来源：http://hz.wangdashe.top/gtsvevwxpv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangshuangyany.cn/gtvkvvxwvs.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtpctiqgwv.html

case class User(name: String, age: Int)
来源：http://hz.fzhhl.top/gtkgfqzyzp.html

[T57] Scala：模式匹配
来源：http://hz.gotoacloud.top/gtrpqkedad.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gogol.net.cn/gteikyxeyi.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtnsvohhqr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guannengcc.top/gtfjltdqhc.html

[T59] Scala：循环
来源：http://hz.xingfuxueyuan.xyz/gtbxmusrgf.html

for (i <- 1 to 10) println(i)
来源：http://hz.tianlin.xyz/gtacznvqzd.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtdvjnqdsv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ywan-chungtsiang.top/gtdidesjoe.html

================================================================================
来源：http://hz.daria6918.cn/gtjmdbfclj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jianghu66.top/gtrqycjnxa.html

================================================================================
来源：http://hz.sysykeji.top/gtovdcxwmg.html

[U01] Py：创建虚拟环境
来源：http://hz.zhaomingkeji.xyz/gtxpwwaaey.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yanxiufei.cn/gtngefbjeu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnqzz.top/gtklvpdphr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.mhx1999.top/gtzobrezai.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtixjlmvog.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.feifeiyinyue.top/gtkaogrwyt.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gtzyziztjg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangkeji.top/gtsslaisqz.html

[U05] Py：列表去重且保序
来源：http://hz.meibo888.top/gtleyigmxm.html

list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtqpsvbepo.html

[U06] Py：合并两个字典
来源：http://hz.ppjwa.cn/gtiezychjh.html

{**a, **b}
来源：http://hz.hongshengwenyu.top/gtthuboapf.html

[U07] Py：反转字典键值
来源：http://hz.ybcxt.top/gtaxnwzaja.html

{v: k for k, v in d.items()}
来源：http://hz.gotoacloud.top/gtcgbkklyx.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gtfdjqnaht.html

[y for x in nested for y in x]
来源：http://hz.ehwqpu.com/gthylgnfcp.html

[U09] Py：字典取最大值的键
来源：http://hz.sufxvd.cn/gtsarnmnks.html

max(d, key=d.get)
来源：http://hz.cqqwz.cn/gthmwawscw.html

[U10] Py：按值排序字典
来源：http://hz.gogol.net.cn/gtoxpxgnyp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenjidiqi.icu/gtxysgqhgo.html

[U11] Py：生成器表达式
来源：http://hz.tian-w.cn/gtuyfbzlwh.html

(x * 2 for x in arr)
来源：http://hz.9152youxi.cn/gtwadhbyao.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zycfv.cn/gttxrsdwoa.html

Counter(arr).most_common(3)
来源：http://hz.guannengcc.top/gtyvgwofjs.html

[U13] Py：固定长度队列
来源：http://hz.xuanzx.com/gttpjdrimh.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtsgqidlod.html

[U14] Py：分组收集到列表
来源：http://hz.jinyuanbaomall.cn/gtqjtrwqwv.html

defaultdict(list)
来源：http://hz.hywenlv.cn/gtyplsrupi.html

[U15] Py：高精度计时
来源：http://hz.hnqzz.top/gthctuskkb.html

t = time.perf_counter()
来源：http://hz.guannengcc.top/gtzumlstod.html

[U16] Py：命令行参数解析
来源：http://hz.bjfxy.top/gtzzpusgjr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yangfankeji.com/gtsfpzdqxr.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gtpthbjeuy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daxiang520.top/gtqfdearxa.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtovzmtlnb.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtwwlhrmue.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gtsviyinrp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.316326.xyz/gthrsjiukg.html

[U20] Py：缓存函数结果
来源：http://hz.zhijiandao.cn/gtqdjpuxeh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gtaxaewvat.html

[U21] Py：自定义上下文管理器
来源：http://hz.cucudq.cn/gtiegeknwd.html

@contextlib.contextmanager
来源：http://hz.zdqjudy.top/gtevclkdmh.html

[U22] Py：矩阵转置
来源：http://hz.feifeiyinyue.top/gtytimnume.html

list(zip(*m))
来源：http://hz.yvedp.cn/gtqtjpxnsk.html

[U23] Py：分块读取大文件
来源：http://hz.smart0.xyz/gtjjdzkpau.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.quarkkingdee.top/gtnhvxpqzo.html

[U24] Py：路径操作
来源：http://hz.dianchejie.cn/gtuqghhobl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tanke756.top/gtnxsgdlps.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gtttvdhgtf.html

csv.DictReader(f)
来源：http://hz.shangyingyoupin.top/gtoixcnkxd.html

[U26] Py：并发下载
来源：http://hz.gogol.net.cn/gtxedkgjjj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtqrztayxd.html

[U27] Py：异步 HTTP
来源：http://hz.dianchejie.cn/gtxqjkxhgc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenjidiqi.icu/gtadykzshz.html

[U28] Py：类型别名
来源：http://hz.yueranfly.top/gtqbqtklrh.html

UserId = int
来源：http://hz.cashguo.top/gtnskxvshe.html

[U29] Py：属性校验
来源：http://hz.yvedp.cn/gtopqwrsun.html

@property 与 @x.setter 配合
来源：http://hz.ybcxt.top/gtqhsvabew.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtewfvqxvp.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gthpqgbmbs.html

[U31] Py：单测
来源：http://hz.jlsjyb.cn/gtjjtgxdgk.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtunqjnieg.html

[U32] Py：代码格式化
来源：http://hz.redwolf501.top/gtcepgfoca.html

ruff format . && ruff check --fix .
来源：http://hz.wangshuangyany.cn/gttrndlhrm.html

[U33] Py：打包发布
来源：http://hz.yvedp.cn/gtraaunsdt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gtvlkljmvw.html

[U34] Py：判断编码
来源：http://hz.hnqzz.top/gttcjowybx.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtrpxsoplu.html

[U35] Py：发送邮件
来源：http://hz.cheryme.top/gtqhysyfvm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sweek.top/gtucxscsxx.html

[U36] Py：定时任务
来源：http://hz.guannengcc.top/gtqlexujyh.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinyuanbaomall.cn/gtdixjbwan.html

[U37] Py：读写 Excel
来源：http://hz.pengpengdd.cyou/gtzsbrgcwg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj202588.top/gtgfdonqmv.html

[U38] Py：获取脚本所在目录
来源：http://hz.cheryme.top/gtdpfznanm.html

Path(__file__).resolve().parent
来源：http://hz.jqgfzy.top/gtygolhqvy.html

[U39] Py：判断是否在交互环境
来源：http://hz.hammf.cn/gtgfvnaoou.html

sys.stdout.isatty()
来源：http://hz.hnqzz.top/gtuayvnrzf.html

[U40] Py：打印到标准错误
来源：http://hz.kuanghao11.cn/gtygytxkcm.html

print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gtwvlqgyrz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.dashuyun.cn/gtvksxaafd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.wangshuangyany.cn/gtdfodbnap.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pycfn.com/gtsykmwkou.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgufenzy.top/gttahdjnvh.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gtjoizzqkw.html

namespace App\Http;
来源：http://hz.jiagoushi.top/gtlyndxtei.html

[U44] PHP：开启严格类型
来源：http://hz.jianghu66.top/gtuacwexbk.html

declare(strict_types=1);
来源：http://hz.daria6918.cn/gtbqosjlbs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhijiandao.cn/gtdggnbypy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtrcodezkz.html

[U46] PHP：可空类型
来源：http://hz.pycfn.com/gtprvokmpw.html

?string $name = null
来源：http://hz.zhijiandao.cn/gtefyftuma.html

[U47] PHP：联合类型
来源：http://hz.daria6918.cn/gthansummg.html

int|string $id
来源：http://hz.meibo888.top/gtjrygqamr.html

[U48] PHP：纯枚举
来源：http://hz.wangshuangyany.cn/gtptjrfnwc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hysaishi.cn/gthnzultxm.html

[U49] PHP：只读属性
来源：http://hz.yj202588.top/gtzhfmjkfy.html

public readonly string $name
来源：http://hz.wangdashe.top/gtaycjxpsx.html

[U50] PHP：构造器属性提升
来源：http://hz.yongpay.top/gtkjyxzbbg.html

public function __construct(private int $id) {}
来源：http://hz.ybcxt.top/gtawnrfyol.html

[U51] PHP：数组解构
来源：http://hz.wangdashe.top/gtbedbazlr.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtdymloeex.html

[U52] PHP：箭头函数
来源：http://hz.quarkkingdee.top/gtknptoweh.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxinkj.top/gtanbdbxju.html

[U53] PHP：空合并运算符
来源：http://hz.ehwqpu.com/gtnszptprh.html

$v = $a ?? $b ?? "default";
来源：http://hz.sweek.top/gtkwzttrtr.html

[U54] PHP：空安全调用
来源：http://hz.zhiwuduotai.top/gtxeajyhwy.html

$obj?->method()
来源：http://hz.jiagoushi.top/gthdxckklo.html

[U55] PHP：match 表达式
来源：http://hz.daria6918.cn/gtosrtnhse.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ppjwa.cn/gtdwebqzxp.html

[U56] PHP：命名参数
来源：http://hz.yangfankeji.com/gtwmhatfmm.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtuhreahpc.html

[U57] PHP：字符串插值
来源：http://hz.kuanghao11.cn/gttvxnzfgm.html

"值: {$a}"
来源：http://hz.tanke756.top/gttierrpuf.html

[U58] PHP：数组三件套
来源：http://hz.shangyingyoupin.top/gtznnsqhrx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yonumen.top/gtilasjope.html

[U59] PHP：自定义排序
来源：http://hz.sufxvd.cn/gtfvpqmasi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtvkuwycqp.html

[U60] PHP：JSON 编解码
来源：http://hz.316326.xyz/gtvaycdiss.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hongshengwenyu.top/gtqhioabgu.html

[U61] PHP：正则
来源：http://hz.xylfe.cn/gtvrzdmxfv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtaptdiobx.html

[U62] PHP：日期对象
来源：http://hz.xziqi.cn/gtrbavewda.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sufxvd.cn/gtzkxcbqcf.html

[U63] PHP：文件读写
来源：http://hz.andypj.xyz/gtrcljkdre.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gotoacloud.top/gtwzstcfhu.html

[U64] PHP：目录遍历
来源：http://hz.gogol.net.cn/gttnaomzvj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jlsjyb.cn/gtefhhwelm.html

[U65] PHP：会话
来源：http://hz.sysykeji.top/gtemwvsyog.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shzxlz.cn/gtzqnjncbx.html

[U66] PHP：设置 Cookie
来源：http://hz.xuetiantiany.cn/gtllqnfsil.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aibaodan.cn/gttysohviq.html

[U67] PHP：处理文件上传
来源：http://hz.chenjidiqi.icu/gtfxltrfjg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zycfv.cn/gtdcxdswsp.html

[U68] PHP：PDO 连接
来源：http://hz.tian-w.cn/gtjzmjttvi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258.top/gtqinwcxra.html

[U69] PHP：PDO 预处理
来源：http://hz.xuanzx.com/gtmucfxrly.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.andypj.xyz/gtfaqkdqqg.html

[U70] PHP：PDO 事务
来源：http://hz.ppjwa.cn/gtvnqluono.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gtrwwvlblj.html

[U71] PHP：抛出异常
来源：http://hz.hammf.cn/gthpnfjfje.html

throw new RuntimeException("失败", 500);
来源：http://hz.ydjk.org.cn/gtmrghebgk.html

[U72] PHP：写错误日志
来源：http://hz.aibaodan.cn/gtlxoweuus.html

error_log("失败: " . $e->getMessage());
来源：http://hz.0kj1m.cn/gttoqvvguq.html

[U73] PHP：读取 ini 配置
来源：http://hz.shanyushiyangtech.top/gtulyycdri.html

parse_ini_file("config.ini", true)
来源：http://hz.tian-w.cn/gtkqbjhyad.html

[U74] PHP：读取环境变量
来源：http://hz.aizwys.cn/gthhpkgwka.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hywenlv.cn/gtdxlmcold.html

[U75] PHP：依赖注入
来源：http://hz.zhiwuduotai.top/gtqocxcihk.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtwvnuxupi.html

[U76] PHP：简单路由
来源：http://hz.shangyingyoupin.top/gtzjkmnthv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.c1oappe.top/gthzudmufz.html

[U77] PHP：模板渲染
来源：http://hz.jlsjyb.cn/gtjlpuehsw.html

composer require twig/twig
来源：http://hz.gzhubu.top/gtlvknsotp.html

[U78] PHP：单元测试
来源：http://hz.yanxiufei.cn/gthziibecb.html

composer require --dev phpunit/phpunit
来源：http://hz.gotoacloud.top/gtrkztygjh.html

[U79] PHP：静态分析
来源：http://hz.52xcode.cn/gtydouxewh.html

composer require --dev phpstan/phpstan
来源：http://hz.feifeiyinyue.top/gtnxbnhfki.html

[U80] PHP：代码规范修复
来源：http://hz.xinyue.icu/gtchoehqfu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nanxuanxn.top/gtgtujggzv.html

[U81] JS：初始化项目
来源：http://hz.hfpthk.cn/gtrpvppixv.html

npm init -y;  npm i express
来源：http://hz.zhixingplan.top/gtfaefdbfr.html

[U82] JS：package.json 脚本
来源：http://hz.cucudq.cn/gtijfxorxx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yueranfly.top/gtkkpgjczq.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhixingplan.top/gtgghwtjap.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtnpjzqccn.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangtech.top/gtnkkxlayw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtuogygpsr.html

[U85] JS：可选链
来源：http://hz.hfpthk.cn/gtnkfdonfy.html

a?.b?.c
来源：http://hz.xziqi.cn/gtqbsdcygr.html

[U86] JS：空值合并
来源：http://hz.chenzaomai.com/gtvwbwztvd.html

a ?? b
来源：http://hz.zhixingplan.top/gtgzvjmpiq.html

[U87] JS：解构默认值
来源：http://hz.52xcode.cn/gthatvukbk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yvedp.cn/gtwfwswpdj.html

[U88] JS：对象展开合并
来源：http://hz.zhongyouzk.top/gticcymuop.html

{ ...a, ...b }
来源：http://hz.smart0.xyz/gtlkriymxh.html

[U89] JS：数组去重
来源：http://hz.shzxlz.cn/gtbpssyegq.html

[...new Set(arr)]
来源：http://hz.aizwys.cn/gtlseelejf.html

[U90] JS：数字数组排序
来源：http://hz.redwolf501.top/gteqmvuimn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtlmwftsyo.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtfdvaqcxr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pycfn.com/gtuaqwwtml.html

[U92] JS：深拷贝
来源：http://hz.jianghu66.top/gtzjnjrtic.html

structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtkxbwmvvz.html

[U93] JS：模板字符串
来源：http://hz.tanke756.top/gtbxeyobwz.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gtvbivxsrm.html

[U94] JS：箭头函数
来源：http://hz.shanyushiyangtech.top/gtgridvook.html

const double = x => x * 2;
来源：http://hz.bjfxy.top/gtauusrpgf.html

[U95] JS：Promise 包装
来源：http://hz.birdmap.top/gtbsasyobj.html

new Promise((resolve, reject) => {})
来源：http://hz.cheryme.top/gthqjyzxpp.html

[U96] JS：async/await 与异常
来源：http://hz.ydzc1.top/gteegafkqk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtdztnttdl.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtadasgkgh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtwqlskfdw.html

[U98] JS：fetch 带 JSON
来源：http://hz.ydjk.org.cn/gtplhhbxxg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cheryme.top/gtisixdahr.html

[U99] JS：事件监听
来源：http://hz.kuanghao11.cn/gtycqoxlxd.html

el.addEventListener("click", e => {})
来源：http://hz.hysaishi.cn/gtcyoelexx.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtqtmurczq.html

document.querySelector(".item")
来源：http://hz.quarkkingdee.top/gtbbgnzgus.html

[U101] JS：classList 操作
来源：http://hz.xziqi.cn/gtouygcgjg.html

el.classList.toggle("active")
来源：http://hz.smart0.xyz/gtjepbuuaf.html

[U102] JS：本地存储
来源：http://hz.zhixingplan.top/gtwbybtltn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.0kj1m.cn/gtxbkesmcn.html

[U103] JS：定时器
来源：http://hz.guannengcc.top/gtuejbrvcs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cashguo.top/gtsawqfwin.html

[U104] JS：防抖
来源：http://hz.chenjidiqi.icu/gtfgzklzxk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtxorlxqpm.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gtpbwmmlxz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cashguo.top/gtfezvhull.html

[U106] JS：日期格式化
来源：http://hz.ybcxt.top/gtpymlfnvd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.9152youxi.cn/gtmhupzcgl.html

[U107] JS：数字千分位
来源：http://hz.shanyushiyangtech.top/gtjlhljzwd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pengpengdd.cyou/gtdnjpwfdi.html

[U108] JS：随机整数
来源：http://hz.jinqigufen.top/gtqntktfhx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zdqjudy.top/gtyjhdetkf.html

[U109] JS：数组分组
来源：http://hz.shangyingyoupin.top/gtsuzpzcgq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xylfe.cn/gtuuvciguj.html

[U110] JS：数组分块
来源：http://hz.cucudq.cn/gtqlyimvuq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xziqi.cn/gthwzogpvv.html

[U111] JS：对象转 Map
来源：http://hz.iojbl.cn/gtkjokfepv.html

new Map(Object.entries(obj))
来源：http://hz.jyoumei.cn/gtqgjpqrzq.html

[U112] JS：字符串补位
来源：http://hz.0kj1m.cn/gtfhbmnefn.html

"7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtvvsxfrja.html

[U113] JS：正则替换全部
来源：http://hz.svipenyu.cn/gtqgsijmkj.html

s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtmclzoitn.html

[U114] JS：JSON 深比较
来源：http://hz.birdmap.top/gtgiisggok.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtkjkyrjhu.html

[U115] JS：生成 UUID
来源：http://hz.gogol.net.cn/gtnmqmmpth.html

crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtdvlmajzm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangshuangyany.cn/gtcxsxnbxi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhoulong.xyz/gtpiwpnesm.html

[U117] JS：单元测试
来源：http://hz.sxryk.cn/gtwatywycx.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtevgbnntw.html

[U118] JS：开发服务器
来源：http://hz.shuidangran.top/gtjrgxmmdj.html

npm i -D vite;  npx vite
来源：http://hz.yuanzhike.top/gtryqcltua.html

[U119] JS：生产构建
来源：http://hz.snrcjt.cn/gtrpilnfoy.html

npx vite build
来源：http://hz.cheryme.top/gtezqpuouh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yonumen.top/gtjbewmjth.html

import.meta.env.VITE_API_URL
来源：http://hz.chenzaomai.com/gtlnycofua.html

================================================================================
来源：http://hz.tianlin.xyz/gttvnassul.html

统计汇总
来源：http://hz.dianchejie.cn/gtvzbjwfkg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtbsdvrrgk.html

按语言统计（条）：
来源：http://hz.sxryk.cn/gtwtcoaapd.html

Python ......... 252
来源：http://hz.fengsongda.top/gtddiizbdx.html

PHP ............ 252
来源：http://hz.ydzc1.top/gtvveftkeo.html

JavaScript ..... 252
来源：http://hz.cheryme.top/gtittdejkn.html

TypeScript ..... 212
来源：http://hz.wangdashe.top/gtsjojzdnd.html

Java ........... 212
来源：http://hz.yangfankeji.com/gtjbbkxyvi.html

Go ............. 212
来源：http://hz.ehwqpu.com/gtuxtedejf.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gtiaoeafba.html

C# ............. 212
来源：http://hz.feifeiyinyue.top/gtbwrytvjs.html

C .............. 30
来源：http://hz.zhoulong.xyz/gtokivpyfy.html

C++ ............ 30
来源：http://hz.yongpay.top/gtbnddjmhi.html

SQL ............ 90
来源：http://hz.zhiwuduotai.top/gtldglepmg.html

Bash ........... 80
来源：http://hz.ppjwa.cn/gtkjeigoql.html

Kotlin ......... 15
来源：http://hz.ydjk.org.cn/gtxblpcjux.html

Swift .......... 15
来源：http://hz.aibaodan.cn/gtkopwzxcx.html

Lua ............ 10
来源：http://hz.fengsongda.top/gtqxcfwqoo.html

Perl ........... 10
来源：http://hz.jinyuanbaomall.cn/gtmmegrrhu.html

Scala .......... 10
来源：http://hz.vqdsnc.cn/gtgnivslxd.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtkyfonynv.html

合计 ........... 2106 条
来源：http://hz.fzhhl.top/gtnbkcphsa.html

按章节统计：
来源：http://hz.gzhubu.top/gtwzxpcmje.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtmwfvszty.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtmwzorpbt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtxokxtovl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtoygsrfrs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sweek.top/gtgrvtglcb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtyqbobolm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtocnlnchg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.dianchejie.cn/gtobftcanl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtekdcvowc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gthgbrveci.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtrswsceap.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtsgqdpctc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtygasfxpc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtxmweuswu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhiwuduotai.top/gtmlptrtmp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtqjumdmxq.html

Q SQL 专题                              90
来源：http://hz.jqgfzy.top/gtticxtroq.html

R Bash 专题                             80
来源：http://hz.jyoumei.cn/gtzclcqdcr.html

S C / C++ 专题                          60
来源：http://hz.xuetiantiany.cn/gtlrwdmhvu.html

T 其他语言补充                          60
来源：http://hz.xingfuxueyuan.xyz/gtprihseqp.html


<!-- 参考信息 -->