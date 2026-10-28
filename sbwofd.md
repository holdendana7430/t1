代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.xylfe.cn/gtcudfpuqv.html

[T57] Scala：模式匹配
来源：http://hz.wangshuangyany.cn/gthfqdfmlh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhoulong.xyz/gtmmdqtpyz.html

[T58] Scala：函数定义
来源：http://hz.c1oappe.top/gtkpbzmeux.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ivvv.top/gtcaxowezf.html

[T59] Scala：循环
来源：http://hz.hammf.cn/gtuwizkwgk.html

for (i <- 1 to 10) println(i)
来源：http://hz.jianghu66.top/gtpibciict.html

[T60] Scala：折叠
来源：http://hz.haohaochexian.top/gthgpdiupy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nwbrower.top/gtqhnghwuc.html

================================================================================
来源：http://hz.cqqwz.cn/gtnevtzjtw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtvrlkewwt.html

================================================================================
来源：http://hz.smart0.xyz/gtmjacbcqu.html

[U01] Py：创建虚拟环境
来源：http://hz.fengsongda.top/gtiqhruwwg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.meibo888.top/gtmxtflmfw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jianghu66.top/gtgockjucu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtbibtkykd.html

[U03] Py：加载 .env 配置
来源：http://hz.birdmap.top/gtndohiskj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydjk.org.cn/gtpowrdalb.html

[U04] Py：变量调试打印
来源：http://hz.hfpthk.cn/gtufsdxwpx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtxjsialcv.html

[U05] Py：列表去重且保序
来源：http://hz.guowangkeji.top/gthumbwfvm.html

list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtzhzmuvfy.html

[U06] Py：合并两个字典
来源：http://hz.nanxuanxn.top/gtdixoilty.html

{**a, **b}
来源：http://hz.andypj.xyz/gtpmqidvwv.html

[U07] Py：反转字典键值
来源：http://hz.jyoumei.cn/gtcvurjuom.html

{v: k for k, v in d.items()}
来源：http://hz.smart0.xyz/gtidrdchqt.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtuhbdeqca.html

[y for x in nested for y in x]
来源：http://hz.fengsongda.top/gtjozvsthk.html

[U09] Py：字典取最大值的键
来源：http://hz.birdmap.top/gtlxdfcoom.html

max(d, key=d.get)
来源：http://hz.fzhhl.top/gtzsxnvdij.html

[U10] Py：按值排序字典
来源：http://hz.wangshuangyany.cn/gtncqndnzw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shanyushiyangtech.top/gtlauxyrst.html

[U11] Py：生成器表达式
来源：http://hz.yongpay.top/gttqrwpubp.html

(x * 2 for x in arr)
来源：http://hz.yvedp.cn/gtvyzkbbxg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yonumen.top/gtvpvjuzvk.html

Counter(arr).most_common(3)
来源：http://hz.jyoumei.cn/gtiwatgroi.html

[U13] Py：固定长度队列
来源：http://hz.vqdsnc.cn/gtenzexusz.html

deque(maxlen=10)
来源：http://hz.dashuyun.cn/gtfnwblbbt.html

[U14] Py：分组收集到列表
来源：http://hz.xingfuxueyuan.xyz/gtvrvbygfl.html

defaultdict(list)
来源：http://hz.wangdashe.top/gtiiyjvmak.html

[U15] Py：高精度计时
来源：http://hz.nwbrower.top/gtyrzllthr.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gttkcmskpq.html

[U16] Py：命令行参数解析
来源：http://hz.hywenlv.cn/gtnxpixvpv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shangyingyoupin.top/gtoxfjogws.html

[U17] Py：初始化日志
来源：http://hz.hongshengwenyu.top/gtsfdunhuh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cdnleiting.top/gtwswjobya.html

[U18] Py：预编译正则
来源：http://hz.dianchejie.cn/gtjorotwer.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtatrzcklx.html

[U19] Py：正则替换带回调
来源：http://hz.9152youxi.cn/gthqbawofg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj20258888.top/gttilxtdyd.html

[U20] Py：缓存函数结果
来源：http://hz.jinghuilouyu.cn/gtnarszvuv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtbopamoia.html

[U21] Py：自定义上下文管理器
来源：http://hz.zycfv.cn/gtaaikyfza.html

@contextlib.contextmanager
来源：http://hz.wangdashe.top/gtmblnuxgn.html

[U22] Py：矩阵转置
来源：http://hz.yj20258888.top/gtvtxrjhwl.html

list(zip(*m))
来源：http://hz.hfpthk.cn/gtokijyqwb.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258.top/gtdjapzyrd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hammf.cn/gtkrsljkux.html

[U24] Py：路径操作
来源：http://hz.jlsjyb.cn/gtvxqxfjmw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yongpay.top/gtajpdfkbd.html

[U25] Py：CSV 按字典读
来源：http://hz.cdnleiting.top/gtpanngbju.html

csv.DictReader(f)
来源：http://hz.jlsjyb.cn/gtdflmuher.html

[U26] Py：并发下载
来源：http://hz.ydzc1.top/gteaapwula.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtaaxtbkmy.html

[U27] Py：异步 HTTP
来源：http://hz.zhijiandao.cn/gtexpngqwn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtaxuvhfkn.html

[U28] Py：类型别名
来源：http://hz.quarkkingdee.top/gtzvalqqub.html

UserId = int
来源：http://hz.daria6918.cn/gtwbzizqjo.html

[U29] Py：属性校验
来源：http://hz.zycfv.cn/gtikifngxz.html

@property 与 @x.setter 配合
来源：http://hz.zhoulong.xyz/gtecdijqzd.html

[U30] Py：数据类
来源：http://hz.redwolf501.top/gtzksobcgy.html

@dataclass(slots=True)
来源：http://hz.ydjk.org.cn/gtvimurolj.html

[U31] Py：单测
来源：http://hz.ydzc1.top/gttqrpzbru.html

python -m pytest -q
来源：http://hz.cucudq.cn/gtcztwkotd.html

[U32] Py：代码格式化
来源：http://hz.gotoacloud.top/gtbwqrxfco.html

ruff format . && ruff check --fix .
来源：http://hz.tanke756.top/gtfmxpldgu.html

[U33] Py：打包发布
来源：http://hz.hnqzz.top/gtajqfziwy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xziqi.cn/gtyckcytxs.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtpvppissx.html

chardet.detect(raw)
来源：http://hz.iojbl.cn/gtrmcjrwvq.html

[U35] Py：发送邮件
来源：http://hz.ybcxt.top/gtaezxqnut.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shanyushiyangkeji.top/gtwaucfaje.html

[U36] Py：定时任务
来源：http://hz.jianghu66.top/gtkucssyuf.html

schedule.every(10).minutes.do(job)
来源：http://hz.havefunace.top/gtipaezfgz.html

[U37] Py：读写 Excel
来源：http://hz.xziqi.cn/gtqxyheizx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gtnwcblwzh.html

[U38] Py：获取脚本所在目录
来源：http://hz.316326.xyz/gtvuonpggv.html

Path(__file__).resolve().parent
来源：http://hz.yueranfly.top/gtdknoumsr.html

[U39] Py：判断是否在交互环境
来源：http://hz.fengsongda.top/gtuxfzvsza.html

sys.stdout.isatty()
来源：http://hz.yj20258888.top/gtwowwsnjw.html

[U40] Py：打印到标准错误
来源：http://hz.gaohongyu789.top/gtsaovlhyg.html

print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtanhgylul.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sufxvd.cn/gtsatlgigz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jyoumei.cn/gtemvdfzdh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ivvv.top/gtkncvpowi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.c1oappe.top/gtbvbszvse.html

[U43] PHP：声明命名空间
来源：http://hz.jianghu66.top/gtlbfettww.html

namespace App\Http;
来源：http://hz.jiagoushi.top/gtmremgmou.html

[U44] PHP：开启严格类型
来源：http://hz.zhengqikj.top/gtxnzelimf.html

declare(strict_types=1);
来源：http://hz.vqdsnc.cn/gtlraxhvwn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhijiandao.cn/gtcfypsucq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtpjzvqvft.html

[U46] PHP：可空类型
来源：http://hz.52xcode.cn/gtzfqoyiyo.html

?string $name = null
来源：http://hz.shanyushiyangkeji.top/gthqvwnpag.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtvlmihvue.html

int|string $id
来源：http://hz.ydjk.org.cn/gthbzqgyjn.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtgopihufn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aizwys.cn/gtfguoryyd.html

[U49] PHP：只读属性
来源：http://hz.kuanghao11.cn/gtmypfoyzr.html

public readonly string $name
来源：http://hz.xuetiantiany.cn/gthgznptuq.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtpfbwbqzt.html

public function __construct(private int $id) {}
来源：http://hz.xylfe.cn/gtakfxdpta.html

[U51] PHP：数组解构
来源：http://hz.chenzaomai.com/gtlmndynqz.html

[$a, $b] = $arr;
来源：http://hz.316326.xyz/gtcjqdbpjs.html

[U52] PHP：箭头函数
来源：http://hz.jqgfzy.top/gtdskvzvoz.html

$double = fn($x) => $x * 2;
来源：http://hz.tanke756.top/gtkmdjptya.html

[U53] PHP：空合并运算符
来源：http://hz.bjfxy.top/gtqkkyeixv.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydzc1.top/gtomoygtfq.html

[U54] PHP：空安全调用
来源：http://hz.redwolf501.top/gtslzbilqt.html

$obj?->method()
来源：http://hz.zhengqikj.top/gtxqkpzhva.html

[U55] PHP：match 表达式
来源：http://hz.ydzc1.top/gtboqdqjbh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhixingplan.top/gthhjkbytj.html

[U56] PHP：命名参数
来源：http://hz.ybcxt.top/gtfwkwnlgq.html

f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gttmdmytzz.html

[U57] PHP：字符串插值
来源：http://hz.sxryk.cn/gtsgjbjfnp.html

"值: {$a}"
来源：http://hz.wangdashe.top/gtfsywmuqg.html

[U58] PHP：数组三件套
来源：http://hz.yvedp.cn/gtzdhmeorn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yanxiufei.cn/gtupvijizf.html

[U59] PHP：自定义排序
来源：http://hz.ydjk.org.cn/gtcabifxny.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtsmqrdyzr.html

[U60] PHP：JSON 编解码
来源：http://hz.9152youxi.cn/gteugbjdnn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhaomingkeji.xyz/gtcotyiniy.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtzrtnpbdf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtdkrqxmhq.html

[U62] PHP：日期对象
来源：http://hz.yuanzhike.top/gtliottaww.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yueranfly.top/gtihawanae.html

[U63] PHP：文件读写
来源：http://hz.svipenyu.cn/gtjtwhewkw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnxiangtu.top/gtrhcsyjel.html

[U64] PHP：目录遍历
来源：http://hz.shanyushiyangtech.top/gtgxsmysrx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhixingplan.top/gtihdalnup.html

[U65] PHP：会话
来源：http://hz.ehwqpu.com/gtiaqperdz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yanxiufei.cn/gtkqujxckw.html

[U66] PHP：设置 Cookie
来源：http://hz.jinqigfzy.top/gtizhjwrtt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aibaodan.cn/gtabrvyxjq.html

[U67] PHP：处理文件上传
来源：http://hz.vqdsnc.cn/gtupepqfdv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.guowangkeji.top/gtsjjnfzib.html

[U68] PHP：PDO 连接
来源：http://hz.hammf.cn/gtncaypjwk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jlsjyb.cn/gtvwquqsae.html

[U69] PHP：PDO 预处理
来源：http://hz.nwbrower.top/gtkqxrnaev.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.redwolf501.top/gtttiooijh.html

[U70] PHP：PDO 事务
来源：http://hz.fengsongda.top/gtbtphdosr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tian-w.cn/gtuokeepam.html

[U71] PHP：抛出异常
来源：http://hz.gaohongyu789.top/gtrdjqjvcz.html

throw new RuntimeException("失败", 500);
来源：http://hz.yongpay.top/gtnblrczme.html

[U72] PHP：写错误日志
来源：http://hz.9152youxi.cn/gtprvvxuoy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhijiandao.cn/gtwalwnyyp.html

[U73] PHP：读取 ini 配置
来源：http://hz.smart0.xyz/gtybhmtjsv.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtevdndakh.html

[U74] PHP：读取环境变量
来源：http://hz.ydjk.org.cn/gtgpmrnghl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gotoacloud.top/gtidirvnmw.html

[U75] PHP：依赖注入
来源：http://hz.kuanghao11.cn/gthukwwpfi.html

composer require psr/container
来源：http://hz.yvedp.cn/gtovheaken.html

[U76] PHP：简单路由
来源：http://hz.yueranfly.top/gtxvnzfubt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangtech.top/gtvxhaqhpl.html

[U77] PHP：模板渲染
来源：http://hz.yuxming.cn/gtcgdkbdrv.html

composer require twig/twig
来源：http://hz.jinqigfzy.top/gtysbpmjxd.html

[U78] PHP：单元测试
来源：http://hz.smart0.xyz/gtwetoehvn.html

composer require --dev phpunit/phpunit
来源：http://hz.52xcode.cn/gtqdsfvlyc.html

[U79] PHP：静态分析
来源：http://hz.zhijiandao.cn/gtdttxazfz.html

composer require --dev phpstan/phpstan
来源：http://hz.zhixingplan.top/gtvrpxzkdr.html

[U80] PHP：代码规范修复
来源：http://hz.yvedp.cn/gtkkhxlaln.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhengqikj.top/gttkfwmegx.html

[U81] JS：初始化项目
来源：http://hz.jlsjyb.cn/gthfhoczuy.html

npm init -y;  npm i express
来源：http://hz.mhx1999.top/gtilqlifcl.html

[U82] JS：package.json 脚本
来源：http://hz.ywan-chungtsiang.top/gtclwxezdq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhixingplan.top/gtyatqddav.html

[U83] JS：ES Module 导入导出
来源：http://hz.xuetiantiany.cn/gtppikkkde.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xingfuxueyuan.xyz/gtoliavimd.html

[U84] JS：CommonJS 写法
来源：http://hz.xuanzx.com/gtpaktuhpe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yanxiufei.cn/gtbparsswg.html

[U85] JS：可选链
来源：http://hz.iojbl.cn/gtkkhoeqgx.html

a?.b?.c
来源：http://hz.sufxvd.cn/gtkocbqgoi.html

[U86] JS：空值合并
来源：http://hz.jyoumei.cn/gtwitydqsn.html

a ?? b
来源：http://hz.yanxiufei.cn/gteqvzimfs.html

[U87] JS：解构默认值
来源：http://hz.xuetiantiany.cn/gtezqnpeuf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinqigfzy.top/gtrsqxiybj.html

[U88] JS：对象展开合并
来源：http://hz.tianlin.xyz/gtmdvtpnqg.html

{ ...a, ...b }
来源：http://hz.jlsjyb.cn/gtaskjxrgd.html

[U89] JS：数组去重
来源：http://hz.hnxiangtu.top/gtmyonvdsu.html

[...new Set(arr)]
来源：http://hz.daria6918.cn/gtknsctbgf.html

[U90] JS：数字数组排序
来源：http://hz.zhoulong.xyz/gtqmsjqbli.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtvkmtducv.html

[U91] JS：对象键值遍历
来源：http://hz.tanke756.top/gtadqzpldg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtqtgbhddd.html

[U92] JS：深拷贝
来源：http://hz.iojbl.cn/gtqcllznos.html

structuredClone(obj)
来源：http://hz.jyoumei.cn/gtthycwvlp.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtvxxcsdsi.html

`共 ${n} 条`
来源：http://hz.ppjwa.cn/gtcvrkzxuy.html

[U94] JS：箭头函数
来源：http://hz.yanxiufei.cn/gtdwfwyjkj.html

const double = x => x * 2;
来源：http://hz.jinqigufen.top/gtaplnhcqe.html

[U95] JS：Promise 包装
来源：http://hz.fzhhl.top/gtlxqdkcab.html

new Promise((resolve, reject) => {})
来源：http://hz.gzhubu.top/gtgnjmlelx.html

[U96] JS：async/await 与异常
来源：http://hz.shzxlz.cn/gthyhurubh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtpdgxpyik.html

[U97] JS：并发请求
来源：http://hz.aibaodan.cn/gtccunqoqu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtvcwppymu.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangdashe.top/gtvztzhgqt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhaomingkeji.xyz/gtvxvbpgvu.html

[U99] JS：事件监听
来源：http://hz.yuxming.cn/gtmldjrnvk.html

el.addEventListener("click", e => {})
来源：http://hz.hnqzz.top/gtpsadwgca.html

[U100] JS：DOM 查询
来源：http://hz.316326.xyz/gtnhndivkg.html

document.querySelector(".item")
来源：http://hz.zycfv.cn/gtqygmlzzt.html

[U101] JS：classList 操作
来源：http://hz.xylfe.cn/gtyxwwzhop.html

el.classList.toggle("active")
来源：http://hz.birdmap.top/gtuibufzga.html

[U102] JS：本地存储
来源：http://hz.sxryk.cn/gtizdsfabv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenlongwang.top/gtnddbmvio.html

[U103] JS：定时器
来源：http://hz.gogol.net.cn/gtbdomsxuu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigfzy.top/gtijerldkp.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gteghsjufa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtkxmrcukt.html

[U105] JS：节流
来源：http://hz.hongshengwenyu.top/gturqvshrl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tian-w.cn/gtijalmewq.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtlzpzodzm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuanzx.com/gtjczyexou.html

[U107] JS：数字千分位
来源：http://hz.zhengqikj.top/gtpulcqjrs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gthanmdkno.html

[U108] JS：随机整数
来源：http://hz.dianchejie.cn/gtcodrpodp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigfzy.top/gtlishmqbn.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtechvyzfc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtkvxlfxad.html

[U110] JS：数组分块
来源：http://hz.svipenyu.cn/gtjieqsudh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xingfuxueyuan.xyz/gtbtvmmyhh.html

[U111] JS：对象转 Map
来源：http://hz.dashuyun.cn/gtrvyvycgf.html

new Map(Object.entries(obj))
来源：http://hz.tanke756.top/gtflxtzzhc.html

[U112] JS：字符串补位
来源：http://hz.tian-w.cn/gtneowhvoy.html

"7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtkquvzeqv.html

[U113] JS：正则替换全部
来源：http://hz.vqdsnc.cn/gtortcarjz.html

s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtnzgcuspg.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gthsqptbfa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gtkrvuecoe.html

[U115] JS：生成 UUID
来源：http://hz.hongshengwenyu.top/gtcruavvab.html

crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtxserfrcm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sweek.top/gtdnhdlvng.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tianlin.xyz/gtqnwaaaay.html

[U117] JS：单元测试
来源：http://hz.pycfn.com/gtdjitnmsw.html

npm i -D vitest;  npx vitest
来源：http://hz.jinghuilouyu.cn/gthfgsljkb.html

[U118] JS：开发服务器
来源：http://hz.sweek.top/gtkpvddlkv.html

npm i -D vite;  npx vite
来源：http://hz.jlsjyb.cn/gtmulcxopz.html

[U119] JS：生产构建
来源：http://hz.ywan-chungtsiang.top/gtvgeyqebm.html

npx vite build
来源：http://hz.yonumen.top/gtxyhchhms.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ywan-chungtsiang.top/gtlohbubgs.html

import.meta.env.VITE_API_URL
来源：http://hz.svipenyu.cn/gtorowslci.html

================================================================================
来源：http://hz.hysaishi.cn/gtzecijcsn.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtvhvwtbgw.html

================================================================================
来源：http://hz.xinyue.icu/gtawubgnez.html

按语言统计（条）：
来源：http://hz.hfpthk.cn/gtcxplqcju.html

Python ......... 252
来源：http://hz.c1oappe.top/gtqlzbkghg.html

PHP ............ 252
来源：http://hz.snrcjt.cn/gtbgqxrrbz.html

JavaScript ..... 252
来源：http://hz.meibo888.top/gtfznojyrv.html

TypeScript ..... 212
来源：http://hz.daxiang520.top/gtrpgobepm.html

Java ........... 212
来源：http://hz.yj202588.top/gtdyzwkbir.html

Go ............. 212
来源：http://hz.zhixingplan.top/gtnjptyioi.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gtqueogsfh.html

C# ............. 212
来源：http://hz.316326.xyz/gtxjltrbuy.html

C .............. 30
来源：http://hz.hammf.cn/gtghhiwlfm.html

C++ ............ 30
来源：http://hz.xuetiantiany.cn/gtaveeuyag.html

SQL ............ 90
来源：http://hz.aibaodan.cn/gtxnhuyjzu.html

Bash ........... 80
来源：http://hz.tanke756.top/gtppcwwqbk.html

Kotlin ......... 15
来源：http://hz.sweek.top/gtobphvvep.html

Swift .......... 15
来源：http://hz.yanxiufei.cn/gtpqwfyftl.html

Lua ............ 10
来源：http://hz.zdqjudy.top/gteosmoisu.html

Perl ........... 10
来源：http://hz.zhengqikj.top/gtkgvclneb.html

Scala .......... 10
来源：http://hz.sweek.top/gtpaxvxxhe.html

------------------------------------
来源：http://hz.birdmap.top/gtcgavaafw.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gtuozlwdud.html

按章节统计：
来源：http://hz.hysaishi.cn/gttzhkhlxa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gttopzvnqd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtyaztphwv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtkxnwubwc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtctzzjacw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yvedp.cn/gtsemqujqi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.birdmap.top/gtbpuxdejn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtmpmvkypx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cheryme.top/gtecnjlgal.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtlmnaxzcu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jlsjyb.cn/gtkqijcsza.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtyldpqabn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtwwzvelij.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gttgnlelne.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtoeebttry.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.aizwys.cn/gtakqwjdkh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtfsbayjpw.html

Q SQL 专题                              90
来源：http://hz.shuidangran.top/gtletpifzh.html

R Bash 专题                             80
来源：http://hz.ydjk.org.cn/gtswrudvkb.html

S C / C++ 专题                          60
来源：http://hz.shangyingyoupin.top/gtgmpgakik.html

T 其他语言补充                          60
来源：http://hz.xinyue.icu/gtfctadmkr.html

U 高频实用片段                         120
来源：http://hz.yanxiufei.cn/gtpeqlmdrh.html

------------------------------------
来源：http://hz.hnqzz.top/gtjjpjbiwv.html

合计                                  2106 条
来源：http://hz.aibaodan.cn/gtmjiqktnq.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gtyfskisfj.html


<!-- 参考信息 -->