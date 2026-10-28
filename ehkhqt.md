代发 wailian999

[U09] Py：字典取最大值的键
来源：http://hz.hnqzz.top/gtyliupfpg.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtzmygkapf.html

[U10] Py：按值排序字典
来源：http://hz.dashuyun.cn/gtkzuxklfx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jianghu66.top/gtdkvqqrpt.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtfxffyozp.html

(x * 2 for x in arr)
来源：http://hz.sysykeji.top/gttbthnwep.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shangyingyoupin.top/gthzraiopb.html

Counter(arr).most_common(3)
来源：http://hz.guannengcc.top/gtlpstcfyv.html

[U13] Py：固定长度队列
来源：http://hz.iojbl.cn/gtbudoncdp.html

deque(maxlen=10)
来源：http://hz.tianlin.xyz/gtszipfzrp.html

[U14] Py：分组收集到列表
来源：http://hz.sufxvd.cn/gtakukjawf.html

defaultdict(list)
来源：http://hz.guowangkeji.top/gtzehancik.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtpwwsfqmq.html

t = time.perf_counter()
来源：http://hz.jyoumei.cn/gtzudxqebl.html

[U16] Py：命令行参数解析
来源：http://hz.gaohongyu789.top/gtytovxmen.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinyuanbaomall.cn/gtgoecemgq.html

[U17] Py：初始化日志
来源：http://hz.meibo888.top/gtuaprsfwk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sysykeji.top/gtwzgerras.html

[U18] Py：预编译正则
来源：http://hz.shzxlz.cn/gtbmwsguoy.html

pat = re.compile(r"\d+")
来源：http://hz.hnqzz.top/gtfdqqzncm.html

[U19] Py：正则替换带回调
来源：http://hz.hongshengwenyu.top/gtoybgudxe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guowangkeji.top/gtwruerunc.html

[U20] Py：缓存函数结果
来源：http://hz.ivvv.top/gtyeaodhxk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258888.top/gtepycqjzr.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gteogflgyk.html

@contextlib.contextmanager
来源：http://hz.mhx1999.top/gtmepfbykx.html

[U22] Py：矩阵转置
来源：http://hz.shanyushiyangtech.top/gtvrxwongu.html

list(zip(*m))
来源：http://hz.sxryk.cn/gtemyrnvrl.html

[U23] Py：分块读取大文件
来源：http://hz.redwolf501.top/gtgoaaimoe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yvedp.cn/gtdcavycdg.html

[U24] Py：路径操作
来源：http://hz.daria6918.cn/gtnzdrjqhk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtbaokgsiw.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtivlpqork.html

csv.DictReader(f)
来源：http://hz.nanxinkj.top/gtsvinjdpj.html

[U26] Py：并发下载
来源：http://hz.ydzc1.top/gtbdngwngq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtgdexvmmv.html

[U27] Py：异步 HTTP
来源：http://hz.wangshuangyany.cn/gtcacappcm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dashuyun.cn/gtcsltgsdk.html

[U28] Py：类型别名
来源：http://hz.shanyushiyangkeji.top/gteibqgioi.html

UserId = int
来源：http://hz.yonumen.top/gtjkvjpuvl.html

[U29] Py：属性校验
来源：http://hz.cheryme.top/gttzpmeqki.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtsqptnswv.html

[U30] Py：数据类
来源：http://hz.snrcjt.cn/gtievjcndp.html

@dataclass(slots=True)
来源：http://hz.jinqigufen.top/gtbsqbrrme.html

[U31] Py：单测
来源：http://hz.xylfe.cn/gtdiqkfygd.html

python -m pytest -q
来源：http://hz.dianchejie.cn/gtoqnzsemn.html

[U32] Py：代码格式化
来源：http://hz.zhongyouzk.top/gtqypckljk.html

ruff format . && ruff check --fix .
来源：http://hz.guowangkeji.top/gtqvdgbtyf.html

[U33] Py：打包发布
来源：http://hz.sweek.top/gtguxzhkcu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtiyeobftg.html

[U34] Py：判断编码
来源：http://hz.tian-w.cn/gtffahmayq.html

chardet.detect(raw)
来源：http://hz.yongpay.top/gtpglvtvkw.html

[U35] Py：发送邮件
来源：http://hz.yangfankeji.com/gtbyfkjsho.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dashuyun.cn/gtvrftenhx.html

[U36] Py：定时任务
来源：http://hz.sxryk.cn/gthgpjrdsn.html

schedule.every(10).minutes.do(job)
来源：http://hz.xinyue.icu/gtbucsyddg.html

[U37] Py：读写 Excel
来源：http://hz.yongpay.top/gtehgpvrkg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hnxiangtu.top/gthsnlruko.html

[U38] Py：获取脚本所在目录
来源：http://hz.xinyue.icu/gtmnuithgs.html

Path(__file__).resolve().parent
来源：http://hz.shangyingyoupin.top/gtccmzzptm.html

[U39] Py：判断是否在交互环境
来源：http://hz.ehwqpu.com/gtcywxfydw.html

sys.stdout.isatty()
来源：http://hz.jinqigufen.top/gtuuswuxly.html

[U40] Py：打印到标准错误
来源：http://hz.aibaodan.cn/gtcpodwwio.html

print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtpxezrllh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xuanzx.com/gtkzbbqhda.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhaomingkeji.xyz/gtjwbqrgrw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinghuilouyu.cn/gtrftoieze.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jlsjyb.cn/gtwwbulkma.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gteigpvlmc.html

namespace App\Http;
来源：http://hz.sxryk.cn/gtraxgatoe.html

[U44] PHP：开启严格类型
来源：http://hz.mhx1999.top/gtaggmyiwi.html

declare(strict_types=1);
来源：http://hz.yueranfly.top/gtuuvkaagy.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xinyue.icu/gtrntqfshf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtkbvtickb.html

[U46] PHP：可空类型
来源：http://hz.wangdashe.top/gtcpxskija.html

?string $name = null
来源：http://hz.smart0.xyz/gtwigqdsse.html

[U47] PHP：联合类型
来源：http://hz.zhongyouzk.top/gtjqphqdvo.html

int|string $id
来源：http://hz.sxryk.cn/gtoaalxcem.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gtulojdfiu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtwcldnaqo.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gtrmuofctt.html

public readonly string $name
来源：http://hz.zhixingplan.top/gtuwjnsmpe.html

[U50] PHP：构造器属性提升
来源：http://hz.zhaomingkeji.xyz/gtabbiiqle.html

public function __construct(private int $id) {}
来源：http://hz.daxiang520.top/gtuwjkrrqb.html

[U51] PHP：数组解构
来源：http://hz.hysaishi.cn/gtqjjrygnb.html

[$a, $b] = $arr;
来源：http://hz.gotoacloud.top/gtkyncmkso.html

[U52] PHP：箭头函数
来源：http://hz.shangyingyoupin.top/gtigdyfysa.html

$double = fn($x) => $x * 2;
来源：http://hz.hfpthk.cn/gtffxntkma.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gtruoyjvwj.html

$v = $a ?? $b ?? "default";
来源：http://hz.quarkkingdee.top/gthgnuztdd.html

[U54] PHP：空安全调用
来源：http://hz.zhongyouzk.top/gtgtocezwr.html

$obj?->method()
来源：http://hz.cheryme.top/gtbwyezhnp.html

[U55] PHP：match 表达式
来源：http://hz.yongpay.top/gtgnzhaxgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hammf.cn/gtbclhqvjr.html

[U56] PHP：命名参数
来源：http://hz.cucudq.cn/gtajsenkkc.html

f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtpuzokykp.html

[U57] PHP：字符串插值
来源：http://hz.snrcjt.cn/gtnkokzbfh.html

"值: {$a}"
来源：http://hz.hywenlv.cn/gtyeusnmmh.html

[U58] PHP：数组三件套
来源：http://hz.xziqi.cn/gtnikkjgon.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj20258888.top/gtspyxldsm.html

[U59] PHP：自定义排序
来源：http://hz.dashuyun.cn/gtuedrgzny.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gtxrgrdptq.html

[U60] PHP：JSON 编解码
来源：http://hz.birdmap.top/gtylxwsyss.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zdqjudy.top/gtqrjvwpfl.html

[U61] PHP：正则
来源：http://hz.zdqjudy.top/gtlthoesmm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtftcgcmec.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtbyoyiena.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sysykeji.top/gtmgmegumv.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtfuqgumgz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigfzy.top/gtbjwoyyzk.html

[U64] PHP：目录遍历
来源：http://hz.yj20258.top/gtbwdcvgbc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.havefunace.top/gtbfgqicjn.html

[U65] PHP：会话
来源：http://hz.gzhubu.top/gtnqkcjjjg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtrsmtuwph.html

[U66] PHP：设置 Cookie
来源：http://hz.zhiwuduotai.top/gttznjqaqc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zdqjudy.top/gttznvgznh.html

[U67] PHP：处理文件上传
来源：http://hz.cqqwz.cn/gtpkfvuryu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ybcxt.top/gtfnxxoikm.html

[U68] PHP：PDO 连接
来源：http://hz.quarkkingdee.top/gtzerhcmnn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aizwys.cn/gtrvawkjhh.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtsecddirq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gtmharmaar.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gttrgaxvnd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinyuanbaomall.cn/gtiyjcedmy.html

[U71] PHP：抛出异常
来源：http://hz.dashuyun.cn/gtyqimnkna.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj20258888.top/gtavobqkse.html

[U72] PHP：写错误日志
来源：http://hz.tian-w.cn/gtjgawhcwg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.fzhhl.top/gtoepqwssn.html

[U73] PHP：读取 ini 配置
来源：http://hz.shzxlz.cn/gtzargebtd.html

parse_ini_file("config.ini", true)
来源：http://hz.hnqzz.top/gtrtvdhhvr.html

[U74] PHP：读取环境变量
来源：http://hz.guowangkeji.top/gtfmdwruxh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.andypj.xyz/gthspeetxx.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gthrrueonu.html

composer require psr/container
来源：http://hz.sufxvd.cn/gtbqppmzpo.html

[U76] PHP：简单路由
来源：http://hz.ydjk.org.cn/gtkvcrsmdu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gogol.net.cn/gtdqidsvqm.html

[U77] PHP：模板渲染
来源：http://hz.jiagoushi.top/gtfgxzihnf.html

composer require twig/twig
来源：http://hz.yonumen.top/gtxgnspvgz.html

[U78] PHP：单元测试
来源：http://hz.ydjk.org.cn/gttludhnmp.html

composer require --dev phpunit/phpunit
来源：http://hz.ywan-chungtsiang.top/gtinoenhiq.html

[U79] PHP：静态分析
来源：http://hz.hfpthk.cn/gtximchfir.html

composer require --dev phpstan/phpstan
来源：http://hz.wangdashe.top/gtpovrfuas.html

[U80] PHP：代码规范修复
来源：http://hz.ybcxt.top/gtqiyjctcw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.iojbl.cn/gtdovqstdd.html

[U81] JS：初始化项目
来源：http://hz.jinyuanbaomall.cn/gtwqaxgair.html

npm init -y;  npm i express
来源：http://hz.snrcjt.cn/gtjeueumnd.html

[U82] JS：package.json 脚本
来源：http://hz.ehwqpu.com/gtvkcyxqms.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinghuilouyu.cn/gttuszmlph.html

[U83] JS：ES Module 导入导出
来源：http://hz.hfpthk.cn/gtqnxhdxwz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gtgjjfkmfr.html

[U84] JS：CommonJS 写法
来源：http://hz.yonumen.top/gtjohjsxeh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.andypj.xyz/gtxtcovlyh.html

[U85] JS：可选链
来源：http://hz.guannengcc.top/gtdnluwfhq.html

a?.b?.c
来源：http://hz.xingfuxueyuan.xyz/gtgjypmpyg.html

[U86] JS：空值合并
来源：http://hz.cashguo.top/gtoaklnbka.html

a ?? b
来源：http://hz.hfpthk.cn/gtfqisbtkf.html

[U87] JS：解构默认值
来源：http://hz.yonumen.top/gtcwieqryc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yonumen.top/gtustlpzkn.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtenfbajbb.html

{ ...a, ...b }
来源：http://hz.nanxinkj.top/gtpuhbjcqh.html

[U89] JS：数组去重
来源：http://hz.nwbrower.top/gtvrsjubtb.html

[...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtbvqpbbap.html

[U90] JS：数字数组排序
来源：http://hz.havefunace.top/gtoxwudyrs.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtnpgobrbg.html

[U91] JS：对象键值遍历
来源：http://hz.xuetiantiany.cn/gtnbpmfwod.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ivvv.top/gtjfttmyyz.html

[U92] JS：深拷贝
来源：http://hz.ivvv.top/gtsiaddlxh.html

structuredClone(obj)
来源：http://hz.cqqwz.cn/gtmmhjgpxj.html

[U93] JS：模板字符串
来源：http://hz.quarkkingdee.top/gtivnrbdjn.html

`共 ${n} 条`
来源：http://hz.jinyuanbaomall.cn/gtctbkgjtf.html

[U94] JS：箭头函数
来源：http://hz.jinyuanbaomall.cn/gtpfmutuzy.html

const double = x => x * 2;
来源：http://hz.yj202588.top/gtmmhiuxop.html

[U95] JS：Promise 包装
来源：http://hz.nanxinkj.top/gtwncmhcsa.html

new Promise((resolve, reject) => {})
来源：http://hz.birdmap.top/gtsgrrgrrk.html

[U96] JS：async/await 与异常
来源：http://hz.hnqzz.top/gterrydfoz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtnbbtpbgk.html

[U97] JS：并发请求
来源：http://hz.haohaochexian.top/gtsnhaihvo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtsbovzdmk.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangshuangyany.cn/gtzqyazwqt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jlsjyb.cn/gthykutoyb.html

[U99] JS：事件监听
来源：http://hz.svipenyu.cn/gthwdvatmk.html

el.addEventListener("click", e => {})
来源：http://hz.yj20258888.top/gttvkkbqtp.html

[U100] JS：DOM 查询
来源：http://hz.zhaomingkeji.xyz/gtpftpabee.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gtfhoadsrm.html

[U101] JS：classList 操作
来源：http://hz.tianlin.xyz/gtizelsgkf.html

el.classList.toggle("active")
来源：http://hz.yj202588.top/gtwsqfmrae.html

[U102] JS：本地存储
来源：http://hz.jqgfzy.top/gtestbdmmh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuxming.cn/gtdqbtggdf.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtbhhkarwc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sxryk.cn/gtzevtuxkl.html

[U104] JS：防抖
来源：http://hz.ydzc1.top/gtjtqmnntq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtxnyjlodi.html

[U105] JS：节流
来源：http://hz.birdmap.top/gtmgncjcba.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtxoinfugk.html

[U106] JS：日期格式化
来源：http://hz.ydjk.org.cn/gtdmrgrizr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj202588.top/gtztnyoehj.html

[U107] JS：数字千分位
来源：http://hz.shangyingyoupin.top/gtdwxyfvxm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangdashe.top/gtdgxjnupb.html

[U108] JS：随机整数
来源：http://hz.cucudq.cn/gttlqnlmgk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hfpthk.cn/gtzwuzibvl.html

[U109] JS：数组分组
来源：http://hz.sysykeji.top/gtazznadym.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtbtxzstpz.html

[U110] JS：数组分块
来源：http://hz.shanyushiyangkeji.top/gtyiwwtynh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258.top/gtxojcaswm.html

[U111] JS：对象转 Map
来源：http://hz.jianghu66.top/gtacecgkqs.html

new Map(Object.entries(obj))
来源：http://hz.yonumen.top/gtzsbzmeds.html

[U112] JS：字符串补位
来源：http://hz.c1oappe.top/gttwfylyse.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtpibmnefe.html

[U113] JS：正则替换全部
来源：http://hz.dianchejie.cn/gtyuzdrlra.html

s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtjnohsacn.html

[U114] JS：JSON 深比较
来源：http://hz.dianchejie.cn/gtdmwlrhky.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtdoapzdfm.html

[U115] JS：生成 UUID
来源：http://hz.sysykeji.top/gtfyazvivt.html

crypto.randomUUID()
来源：http://hz.c1oappe.top/gtmjyegdan.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gtrtgskbxy.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cdnleiting.top/gtqcxbwdkk.html

[U117] JS：单元测试
来源：http://hz.cdnleiting.top/gtzanolkbp.html

npm i -D vitest;  npx vitest
来源：http://hz.zycfv.cn/gtakjvxtde.html

[U118] JS：开发服务器
来源：http://hz.yuxming.cn/gtvusbrzbz.html

npm i -D vite;  npx vite
来源：http://hz.vqdsnc.cn/gtjlptziit.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtwnhqgpge.html

npx vite build
来源：http://hz.52xcode.cn/gtyxzypkbs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.andypj.xyz/gtmsmpdwwl.html

import.meta.env.VITE_API_URL
来源：http://hz.jinghuilouyu.cn/gtlcntenty.html

================================================================================
来源：http://hz.yuxming.cn/gtzbeclvxs.html

统计汇总
来源：http://hz.kuanghao11.cn/gtqifhosiy.html

================================================================================
来源：http://hz.hfpthk.cn/gtlcrvxtrb.html

按语言统计（条）：
来源：http://hz.hongshengwenyu.top/gtslfwryjy.html

Python ......... 252
来源：http://hz.nanxinkj.top/gtlysshdti.html

PHP ............ 252
来源：http://hz.svipenyu.cn/gtnbppvvxz.html

JavaScript ..... 252
来源：http://hz.andypj.xyz/gtiyazubkz.html

TypeScript ..... 212
来源：http://hz.daxiang520.top/gtrbyussgy.html

Java ........... 212
来源：http://hz.haohaochexian.top/gtzyxnjamu.html

Go ............. 212
来源：http://hz.xziqi.cn/gttecqhpqh.html

Ruby ........... 212
来源：http://hz.daxiang520.top/gtqzfazhjy.html

C# ............. 212
来源：http://hz.xziqi.cn/gtvsrfedgs.html

C .............. 30
来源：http://hz.hywenlv.cn/gtlngafrtx.html

C++ ............ 30
来源：http://hz.jinqigfzy.top/gtkbppwzht.html

SQL ............ 90
来源：http://hz.sufxvd.cn/gtvchwicdt.html

Bash ........... 80
来源：http://hz.wangshuangyany.cn/gtjorqvzhs.html

Kotlin ......... 15
来源：http://hz.jinqigfzy.top/gtdkhysdym.html

Swift .......... 15
来源：http://hz.sysykeji.top/gtrszrgidc.html

Lua ............ 10
来源：http://hz.aibaodan.cn/gtibpodshc.html

Perl ........... 10
来源：http://hz.chenjidiqi.icu/gtskrhxdlr.html

Scala .......... 10
来源：http://hz.mhx1999.top/gtvmgpqpgb.html

------------------------------------
来源：http://hz.andypj.xyz/gtvszxoguv.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtxqnlgpkf.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtozvovskb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtqlwclvkl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtbjdpjztg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtljaenidu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtkpuzghhz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shangyingyoupin.top/gtiafpitxb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yanxiufei.cn/gtqwpeweyk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtowqsoafa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gotoacloud.top/gtqaikbqlq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtxtpbhdiu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtqcpjvxze.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtqbeazjqj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtfhxygqal.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtbtttzzup.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhoulong.xyz/gttyengnxt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sxryk.cn/gtkekhkvji.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtgwirasgq.html

Q SQL 专题                              90
来源：http://hz.aizwys.cn/gtxmildano.html

R Bash 专题                             80
来源：http://hz.jqgfzy.top/gtyhlymeku.html

S C / C++ 专题                          60
来源：http://hz.sysykeji.top/gtwdjlymow.html

T 其他语言补充                          60
来源：http://hz.gogol.net.cn/gteswenoah.html

U 高频实用片段                         120
来源：http://hz.haohaochexian.top/gtjtkfsnim.html

------------------------------------
来源：http://hz.yuanzhike.top/gtqiuamgyj.html

合计                                  2106 条
来源：http://hz.hfpthk.cn/gtuzhqocce.html

--------------------------------------------------------------------------------
来源：http://hz.zhongyouzk.top/gtvwqwdsmr.html

使用提醒
来源：http://hz.aizwys.cn/gtobemmays.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtxitknlzx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nanxinkj.top/gtijonqzol.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.dashuyun.cn/gtfbxzxtkt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tian-w.cn/gttxtmzhqp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenlongwang.top/gtaqmsegqq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.sysykeji.top/gttxmrobjt.html

—— 文件结束 ——
来源：http://hz.zhoulong.xyz/gtssailezf.html

================================================================================
来源：http://hz.redwolf501.top/gtngumsndp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yueranfly.top/gtduihihya.html

Common Programming Examples Cheat Book
来源：http://hz.quarkkingdee.top/gtutgwptti.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgzfboxkb.html

【收录内容】
来源：http://hz.nanxinkj.top/gtxwlcydur.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.andypj.xyz/gtmxxixkik.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.dashuyun.cn/gtqfcnvatn.html

SQL · Bash · C · C++
来源：http://hz.gogol.net.cn/gtfbsfmpnr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.316326.xyz/gtwjfqkayy.html

【使用说明】
来源：http://hz.daria6918.cn/gtllvdvgja.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hongshengwenyu.top/gtuwlxieim.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cqqwz.cn/gtcoizfeay.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinyuanbaomall.cn/gtutntyham.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yangfankeji.com/gtvbuvxdsq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jlsjyb.cn/gtfvcalrqf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hysaishi.cn/gtkwwwfrxp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hfpthk.cn/gtmkoczcdm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yanxiufei.cn/gtkbquglyq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenzaomai.com/gtveukljyd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.52xcode.cn/gtadhifnog.html


<!-- 参考信息 -->