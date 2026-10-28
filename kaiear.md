代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gttbucfwgo.html

================================================================================
来源：http://hz.jiagoushi.top/gthylybviu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gtlqkupezb.html

================================================================================
来源：http://hz.cheryme.top/gtnilxruzo.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxuanxn.top/gtadvfxkiw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnxiangtu.top/gtwvgowuhu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.feifeiyinyue.top/gtcujvecty.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shangyingyoupin.top/gtswwagzpk.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtamhgoodr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangdashe.top/gtozbvgolv.html

[U04] Py：变量调试打印
来源：http://hz.xingfuxueyuan.xyz/gtwknuvhfx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.aizwys.cn/gtknwajhwr.html

[U05] Py：列表去重且保序
来源：http://hz.zycfv.cn/gtqtxwkrdx.html

list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtqrfsgtaa.html

[U06] Py：合并两个字典
来源：http://hz.shangyingyoupin.top/gttpgfdlbx.html

{**a, **b}
来源：http://hz.zhaomingkeji.xyz/gtbdgqgdzw.html

[U07] Py：反转字典键值
来源：http://hz.hongshengwenyu.top/gtgjtcvykg.html

{v: k for k, v in d.items()}
来源：http://hz.xylfe.cn/gtmjjwofow.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtuzltfpyi.html

[y for x in nested for y in x]
来源：http://hz.chenlongwang.top/gtnqhwohsh.html

[U09] Py：字典取最大值的键
来源：http://hz.daxiang520.top/gttnqqcmwc.html

max(d, key=d.get)
来源：http://hz.jinyuanbaomall.cn/gtomhamhxy.html

[U10] Py：按值排序字典
来源：http://hz.vqdsnc.cn/gtpexizlkz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.birdmap.top/gtaakiumzk.html

[U11] Py：生成器表达式
来源：http://hz.yueranfly.top/gtssrsqlrk.html

(x * 2 for x in arr)
来源：http://hz.wangshuangyany.cn/gtpqbksqza.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cucudq.cn/gttqeuoefl.html

Counter(arr).most_common(3)
来源：http://hz.ehwqpu.com/gtijpitxws.html

[U13] Py：固定长度队列
来源：http://hz.sweek.top/gtbnriwafg.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtkpepvwjm.html

[U14] Py：分组收集到列表
来源：http://hz.9152youxi.cn/gtympsnmiq.html

defaultdict(list)
来源：http://hz.hnqzz.top/gtyspskwve.html

[U15] Py：高精度计时
来源：http://hz.cucudq.cn/gtjotlxrci.html

t = time.perf_counter()
来源：http://hz.yj202588.top/gtlthcvjkj.html

[U16] Py：命令行参数解析
来源：http://hz.yanxiufei.cn/gtcfwmmtkx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hongshengwenyu.top/gthdxmzqcl.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gtabarqkmz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinghuilouyu.cn/gteqnjhtfc.html

[U18] Py：预编译正则
来源：http://hz.guowangkeji.top/gtfuquppqc.html

pat = re.compile(r"\d+")
来源：http://hz.chenlongwang.top/gtvmripejm.html

[U19] Py：正则替换带回调
来源：http://hz.shzxlz.cn/gtcfhrdjic.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yueranfly.top/gtfearthie.html

[U20] Py：缓存函数结果
来源：http://hz.hnxiangtu.top/gtifsuprvv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.quarkkingdee.top/gturtlcjnt.html

[U21] Py：自定义上下文管理器
来源：http://hz.mhx1999.top/gtehqxmkpp.html

@contextlib.contextmanager
来源：http://hz.fzhhl.top/gtmbcfgrea.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtiqacmyqu.html

list(zip(*m))
来源：http://hz.nanxuanxn.top/gtbsyvmbmm.html

[U23] Py：分块读取大文件
来源：http://hz.bjfxy.top/gtkzizpkej.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cucudq.cn/gtqgkuonku.html

[U24] Py：路径操作
来源：http://hz.nanxinkj.top/gtsqairztr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtptnbimrg.html

[U25] Py：CSV 按字典读
来源：http://hz.chenzaomai.com/gtaqcdvczn.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtrkjujqkc.html

[U26] Py：并发下载
来源：http://hz.chenlongwang.top/gtxwmjtzhi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zycfv.cn/gtiksddmrp.html

[U27] Py：异步 HTTP
来源：http://hz.tian-w.cn/gtktjiuerx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pycfn.com/gtdttlhgnm.html

[U28] Py：类型别名
来源：http://hz.shzxlz.cn/gthnnqjryf.html

UserId = int
来源：http://hz.zhongyouzk.top/gtlyjxkvmj.html

[U29] Py：属性校验
来源：http://hz.yj20258888.top/gtfwpqgxrh.html

@property 与 @x.setter 配合
来源：http://hz.chenjidiqi.icu/gtnjcjlgbd.html

[U30] Py：数据类
来源：http://hz.sufxvd.cn/gtjjisgnfe.html

@dataclass(slots=True)
来源：http://hz.fengsongda.top/gtvsyihpdr.html

[U31] Py：单测
来源：http://hz.yueranfly.top/gtjjnyjwzx.html

python -m pytest -q
来源：http://hz.jianghu66.top/gttefczqez.html

[U32] Py：代码格式化
来源：http://hz.zhijiandao.cn/gtxgjnpnpc.html

ruff format . && ruff check --fix .
来源：http://hz.c1oappe.top/gtcuczrern.html

[U33] Py：打包发布
来源：http://hz.zhixingplan.top/gtrgvskxzi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cucudq.cn/gtwyufotoo.html

[U34] Py：判断编码
来源：http://hz.daria6918.cn/gtkacmycfq.html

chardet.detect(raw)
来源：http://hz.yuanzhike.top/gtstwknrfj.html

[U35] Py：发送邮件
来源：http://hz.ehwqpu.com/gtvpyorcec.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuetiantiany.cn/gtqlgtrini.html

[U36] Py：定时任务
来源：http://hz.shangyingyoupin.top/gtfzkmpord.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtlepbpmjr.html

[U37] Py：读写 Excel
来源：http://hz.cheryme.top/gtypmthczf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.meibo888.top/gtnblbatpx.html

[U38] Py：获取脚本所在目录
来源：http://hz.9152youxi.cn/gtnkfooosc.html

Path(__file__).resolve().parent
来源：http://hz.ehwqpu.com/gtngyvdwii.html

[U39] Py：判断是否在交互环境
来源：http://hz.yj20258.top/gtczoglbcs.html

sys.stdout.isatty()
来源：http://hz.hysaishi.cn/gtjyipprrh.html

[U40] Py：打印到标准错误
来源：http://hz.chenzaomai.com/gtsbpevort.html

print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtcsisygbs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cucudq.cn/gtwemnsrjd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinyuanbaomall.cn/gtdpzirtfv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.svipenyu.cn/gtfsqqnkgk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gogol.net.cn/gtksyipdhd.html

[U43] PHP：声明命名空间
来源：http://hz.cqqwz.cn/gtuxcydeet.html

namespace App\Http;
来源：http://hz.ydjk.org.cn/gtpuuwdtcw.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigufen.top/gtiwlamkuo.html

declare(strict_types=1);
来源：http://hz.shanyushiyangkeji.top/gtnmxcvbyj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xylfe.cn/gtqkxxtztq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtbnfwcbdo.html

[U46] PHP：可空类型
来源：http://hz.cashguo.top/gtbbhuapfz.html

?string $name = null
来源：http://hz.c1oappe.top/gtaeiarbnl.html

[U47] PHP：联合类型
来源：http://hz.yonumen.top/gtdxrkajdn.html

int|string $id
来源：http://hz.xuanzx.com/gtexfzxrwk.html

[U48] PHP：纯枚举
来源：http://hz.meibo888.top/gtetvouvbr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuanzx.com/gtulklbqes.html

[U49] PHP：只读属性
来源：http://hz.nanxinkj.top/gtbzsbpyzi.html

public readonly string $name
来源：http://hz.bjfxy.top/gttsdaokxo.html

[U50] PHP：构造器属性提升
来源：http://hz.xylfe.cn/gtsgkohoak.html

public function __construct(private int $id) {}
来源：http://hz.mhx1999.top/gtqgxpmkkx.html

[U51] PHP：数组解构
来源：http://hz.jqgfzy.top/gtybtlktzm.html

[$a, $b] = $arr;
来源：http://hz.aibaodan.cn/gtfjmevgvm.html

[U52] PHP：箭头函数
来源：http://hz.tianlin.xyz/gtlmqqdzcv.html

$double = fn($x) => $x * 2;
来源：http://hz.yangfankeji.com/gtutinsamo.html

[U53] PHP：空合并运算符
来源：http://hz.316326.xyz/gtrwtsyutn.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtctysghox.html

[U54] PHP：空安全调用
来源：http://hz.jqgfzy.top/gtfdzozxqi.html

$obj?->method()
来源：http://hz.c1oappe.top/gthkoerknz.html

[U55] PHP：match 表达式
来源：http://hz.ivvv.top/gtxpdqeuil.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtoiovxvpr.html

[U56] PHP：命名参数
来源：http://hz.gaohongyu789.top/gtvfzjhqxp.html

f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtwjsnctmx.html

[U57] PHP：字符串插值
来源：http://hz.52xcode.cn/gtnjudtnwz.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtcrwodhlc.html

[U58] PHP：数组三件套
来源：http://hz.shzxlz.cn/gtkutqeyor.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gzhubu.top/gtxoktlsru.html

[U59] PHP：自定义排序
来源：http://hz.smart0.xyz/gtmisyiojm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtnrmctdvc.html

[U60] PHP：JSON 编解码
来源：http://hz.chenzaomai.com/gtzvemwydc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shangyingyoupin.top/gtidvdhzqo.html

[U61] PHP：正则
来源：http://hz.yueranfly.top/gtxjnkmrvi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtdavdzlco.html

[U62] PHP：日期对象
来源：http://hz.tianlin.xyz/gtbrsxtrgc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ywan-chungtsiang.top/gtsokeejss.html

[U63] PHP：文件读写
来源：http://hz.gzhubu.top/gthrlcrnho.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hywenlv.cn/gtoutpbbim.html

[U64] PHP：目录遍历
来源：http://hz.zhijiandao.cn/gtgqvbdoun.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.havefunace.top/gtgunteajh.html

[U65] PHP：会话
来源：http://hz.yongpay.top/gtrvlqxrsz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gteozpizmz.html

[U66] PHP：设置 Cookie
来源：http://hz.yangfankeji.com/gthiiptmyf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhoulong.xyz/gthendbxny.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtgqqaiise.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.daria6918.cn/gtwmwprzjo.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigufen.top/gtrfltnbpg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuetiantiany.cn/gtuuzgxlzb.html

[U69] PHP：PDO 预处理
来源：http://hz.nwbrower.top/gtdsazzkum.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nwbrower.top/gthhjfyoln.html

[U70] PHP：PDO 事务
来源：http://hz.dashuyun.cn/gtrrrcmcoa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.aizwys.cn/gtgyvmrjus.html

[U71] PHP：抛出异常
来源：http://hz.cashguo.top/gtvydginmc.html

throw new RuntimeException("失败", 500);
来源：http://hz.shanyushiyangtech.top/gtstlesbkv.html

[U72] PHP：写错误日志
来源：http://hz.jqgfzy.top/gtcnsyvtyv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangkeji.top/gtsimwzleo.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gtrxjvvrpl.html

parse_ini_file("config.ini", true)
来源：http://hz.tian-w.cn/gtktjhdscr.html

[U74] PHP：读取环境变量
来源：http://hz.zhengqikj.top/gtqtmcqwff.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenjidiqi.icu/gteablbldc.html

[U75] PHP：依赖注入
来源：http://hz.nanxuanxn.top/gtvpgxfaoq.html

composer require psr/container
来源：http://hz.gaohongyu789.top/gtswroyvwq.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangkeji.top/gtoysjspmw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xingfuxueyuan.xyz/gtemjfqxnb.html

[U77] PHP：模板渲染
来源：http://hz.nwbrower.top/gtubwniugm.html

composer require twig/twig
来源：http://hz.cashguo.top/gtxrdbwxdl.html

[U78] PHP：单元测试
来源：http://hz.pengpengdd.cyou/gtwapzggxu.html

composer require --dev phpunit/phpunit
来源：http://hz.redwolf501.top/gtljxnrauq.html

[U79] PHP：静态分析
来源：http://hz.meibo888.top/gtjkwlpedo.html

composer require --dev phpstan/phpstan
来源：http://hz.andypj.xyz/gtvdkszply.html

[U80] PHP：代码规范修复
来源：http://hz.hnqzz.top/gtsmpfkbae.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xingfuxueyuan.xyz/gtrfhtuhcr.html

[U81] JS：初始化项目
来源：http://hz.shangyingyoupin.top/gtnacsqzpu.html

npm init -y;  npm i express
来源：http://hz.cheryme.top/gtgmkmwump.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangkeji.top/gtodbgfymq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guowangkeji.top/gtfjdzdwxh.html

[U83] JS：ES Module 导入导出
来源：http://hz.9152youxi.cn/gtpyqwbovg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ydjk.org.cn/gtjfqfkbcg.html

[U84] JS：CommonJS 写法
来源：http://hz.hammf.cn/gtobqecsef.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nwbrower.top/gtsfkixzje.html

[U85] JS：可选链
来源：http://hz.52xcode.cn/gtknvbtrxb.html

a?.b?.c
来源：http://hz.c1oappe.top/gtojtweivl.html

[U86] JS：空值合并
来源：http://hz.snrcjt.cn/gtwkfxtnqp.html

a ?? b
来源：http://hz.hywenlv.cn/gtglnmkzuz.html

[U87] JS：解构默认值
来源：http://hz.aibaodan.cn/gtltunpyot.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinqigufen.top/gtrkngmdyy.html

[U88] JS：对象展开合并
来源：http://hz.jyoumei.cn/gtejftspgz.html

{ ...a, ...b }
来源：http://hz.shangyingyoupin.top/gtmywkvkbb.html

[U89] JS：数组去重
来源：http://hz.hnxiangtu.top/gteznfcbuj.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtcnyboggz.html

[U90] JS：数字数组排序
来源：http://hz.shuidangran.top/gtfbmtyxwj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtolhwhvrr.html

[U91] JS：对象键值遍历
来源：http://hz.feifeiyinyue.top/gtpbcvixzl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sysykeji.top/gtuqisstsx.html

[U92] JS：深拷贝
来源：http://hz.aibaodan.cn/gtbimixczx.html

structuredClone(obj)
来源：http://hz.andypj.xyz/gttvlwsuve.html

[U93] JS：模板字符串
来源：http://hz.hnqzz.top/gtroztbxai.html

`共 ${n} 条`
来源：http://hz.jqgufenzy.top/gtodqaozjj.html

[U94] JS：箭头函数
来源：http://hz.yangfankeji.com/gtmsmczfpw.html

const double = x => x * 2;
来源：http://hz.smart0.xyz/gtbldbggey.html

[U95] JS：Promise 包装
来源：http://hz.jlsjyb.cn/gtrswcdxsx.html

new Promise((resolve, reject) => {})
来源：http://hz.cucudq.cn/gtyoueayrv.html

[U96] JS：async/await 与异常
来源：http://hz.hnqzz.top/gtdbjyolex.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtgdhusiul.html

[U97] JS：并发请求
来源：http://hz.sysykeji.top/gtzibljehf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtmrweuafm.html

[U98] JS：fetch 带 JSON
来源：http://hz.hammf.cn/gtfaflesju.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxinkj.top/gtywcwvamr.html

[U99] JS：事件监听
来源：http://hz.xuetiantiany.cn/gtvhjapfce.html

el.addEventListener("click", e => {})
来源：http://hz.jinyuanbaomall.cn/gtquybxbbp.html

[U100] JS：DOM 查询
来源：http://hz.yj202588.top/gttdgtfssi.html

document.querySelector(".item")
来源：http://hz.sufxvd.cn/gtubrxqcdw.html

[U101] JS：classList 操作
来源：http://hz.feifeiyinyue.top/gtnjdwtxtn.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangkeji.top/gtkwvbyjdb.html

[U102] JS：本地存储
来源：http://hz.jiagoushi.top/gttjzaavmk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhongyouzk.top/gtlwvyubem.html

[U103] JS：定时器
来源：http://hz.cdnleiting.top/gtrxjqnaxf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.andypj.xyz/gtgrwkrvec.html

[U104] JS：防抖
来源：http://hz.ivvv.top/gtkcryekak.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtddfugzry.html

[U105] JS：节流
来源：http://hz.ybcxt.top/gtdgynroiu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhiwuduotai.top/gttnbjnhap.html

[U106] JS：日期格式化
来源：http://hz.guannengcc.top/gthcabwxqr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gotoacloud.top/gtcnguxwtr.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtaddbpxdo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.feifeiyinyue.top/gtygjtsgpv.html

[U108] JS：随机整数
来源：http://hz.yj202588.top/gtosteyaaj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.birdmap.top/gtsmtjpwdl.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtorgvurfg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtfggcxdfk.html

[U110] JS：数组分块
来源：http://hz.pycfn.com/gtkhrxjdpb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.pycfn.com/gtgrjnwceo.html

[U111] JS：对象转 Map
来源：http://hz.jianghu66.top/gtljbouvbs.html

new Map(Object.entries(obj))
来源：http://hz.ybcxt.top/gtzbtgfjom.html

[U112] JS：字符串补位
来源：http://hz.zhixingplan.top/gtasjcasts.html

"7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtiowwtaah.html

[U113] JS：正则替换全部
来源：http://hz.hywenlv.cn/gtcvjkjxnp.html

s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtefkezrkh.html

[U114] JS：JSON 深比较
来源：http://hz.jyoumei.cn/gtmrwrqezm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtuxtxsdfu.html

[U115] JS：生成 UUID
来源：http://hz.xylfe.cn/gtclinsncn.html

crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtfqdibapg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yangfankeji.com/gtiykfgxpi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtdvbsbisd.html

[U117] JS：单元测试
来源：http://hz.yuxming.cn/gtftkfwfbf.html

npm i -D vitest;  npx vitest
来源：http://hz.feifeiyinyue.top/gtydadfloh.html

[U118] JS：开发服务器
来源：http://hz.c1oappe.top/gtishyqvrl.html

npm i -D vite;  npx vite
来源：http://hz.hnxiangtu.top/gtcotdhrll.html

[U119] JS：生产构建
来源：http://hz.tian-w.cn/gtdbwprewv.html

npx vite build
来源：http://hz.xingfuxueyuan.xyz/gtikdzpgcf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinyuanbaomall.cn/gtfxknopem.html

import.meta.env.VITE_API_URL
来源：http://hz.snrcjt.cn/gtivcqlrii.html

================================================================================
来源：http://hz.haohaochexian.top/gttwikimgb.html

统计汇总
来源：http://hz.gaohongyu789.top/gtjcuragsd.html

================================================================================
来源：http://hz.316326.xyz/gtkgxppdim.html

按语言统计（条）：
来源：http://hz.jiagoushi.top/gtamafdcsk.html

Python ......... 252
来源：http://hz.gotoacloud.top/gtymqbkdap.html

PHP ............ 252
来源：http://hz.fengsongda.top/gtknmqbbgx.html

JavaScript ..... 252
来源：http://hz.yongpay.top/gtklyrpvnf.html

TypeScript ..... 212
来源：http://hz.52xcode.cn/gtqhejbauv.html

Java ........... 212
来源：http://hz.316326.xyz/gtflhhmkoc.html

Go ............. 212
来源：http://hz.gzhubu.top/gtacffizzx.html

Ruby ........... 212
来源：http://hz.gzhubu.top/gtibiufowx.html

C# ............. 212
来源：http://hz.meibo888.top/gtfmhsavec.html

C .............. 30
来源：http://hz.hnxiangtu.top/gtksvrbsss.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtjptnkkpo.html

SQL ............ 90
来源：http://hz.yongpay.top/gtxavgtkwt.html

Bash ........... 80
来源：http://hz.yuxming.cn/gtscqmtmme.html

Kotlin ......... 15
来源：http://hz.zhengqikj.top/gtsvmmshvq.html

Swift .......... 15
来源：http://hz.bjfxy.top/gtkidiiovv.html

Lua ............ 10
来源：http://hz.zycfv.cn/gtxzhcwcxr.html

Perl ........... 10
来源：http://hz.yonumen.top/gtsihzfrxh.html

Scala .......... 10
来源：http://hz.xylfe.cn/gtfdlrwopj.html

------------------------------------
来源：http://hz.xylfe.cn/gtwbccfekw.html

合计 ........... 2106 条
来源：http://hz.xuanzx.com/gtdjegjbrt.html

按章节统计：
来源：http://hz.shangyingyoupin.top/gtzcwothnx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtadhdzshx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnqzz.top/gtcxwdcpdv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtrkoaskjt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtkmtfcqsb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhijiandao.cn/gtfnpvcife.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xylfe.cn/gtzrrhcjnt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtjayxdrpq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gthfnbtpty.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtcdavcqxk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtezismxet.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtswgddrdw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtdegxzqmf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtpkwxfmfh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gaohongyu789.top/gtxungucwv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ppjwa.cn/gtbcmjnuhd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtluvjyndm.html

Q SQL 专题                              90
来源：http://hz.cqqwz.cn/gtifosutas.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gthioccisk.html

S C / C++ 专题                          60
来源：http://hz.yj202588.top/gtbquiphcf.html

T 其他语言补充                          60
来源：http://hz.52xcode.cn/gtoyubfszp.html

U 高频实用片段                         120
来源：http://hz.jinqigfzy.top/gthsqglxdm.html

------------------------------------
来源：http://hz.hnqzz.top/gtttohtvoe.html

合计                                  2106 条
来源：http://hz.aizwys.cn/gtzxmrzbmm.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtkxtgnsvq.html

使用提醒
来源：http://hz.daria6918.cn/gtholirzdc.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtibfoosev.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cashguo.top/gttxtnadej.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ybcxt.top/gthkddkfox.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xziqi.cn/gtgocstkzh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinqigufen.top/gtqilajtjo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yueranfly.top/gtkyvewubt.html

—— 文件结束 ——
来源：http://hz.smart0.xyz/gtuuxfjdld.html


<!-- 参考信息 -->