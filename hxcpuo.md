代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cashguo.top/gtizriwyoh.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtfgmzigsf.html

awk '{print $1, $3}' a.txt
来源：http://hz.haohaochexian.top/gtwbsscbst.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtziofeuky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtnzixhakj.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtraykceuu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gtftvvuwsb.html

[R51] 排序去重取前几
来源：http://hz.shangyingyoupin.top/gtcbdqgpij.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtzjfjqkja.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtvwexiyag.html

wc -l a.txt
来源：http://hz.chenlongwang.top/gtzqmeuzdx.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtcdqmokvo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtesoawaeu.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtgstnwbjc.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gtvablmdqs.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtydoixkgy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtgymgxquh.html

[R56] 远程拷贝
来源：http://hz.ppjwa.cn/gtflhsrdii.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtcclwupdh.html

[R57] 远程执行命令
来源：http://hz.zhixingplan.top/gtjrffpdqm.html

ssh user@host 'uptime'
来源：http://hz.zhoulong.xyz/gtwasubugq.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gteuwhkrlr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhongyouzk.top/gtkddqhnux.html

[R59] 发 POST JSON
来源：http://hz.cucudq.cn/gttrnyrlxg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtadiufirt.html

[R60] 只看 HTTP 状态码
来源：http://hz.jianghu66.top/gthbgnuxkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pycfn.com/gtwyuuczvd.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtkycyceyo.html

df -h;  du -sh *
来源：http://hz.daxiang520.top/gtkpvlftbc.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtkuywxhfv.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gtibspuoyt.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtbwgvmhep.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtiejhhbwv.html

[R64] 结束进程
来源：http://hz.sufxvd.cn/gthuaawcka.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtpmzwpotk.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtkalydtzk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gtfiruljvn.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtdrpvnphu.html

crontab -e;  crontab -l
来源：http://hz.guannengcc.top/gtyjxdynpi.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtqmgdnwlr.html

openssl rand -hex 16
来源：http://hz.kuanghao11.cn/gtyvuinaeb.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtpbwvpqju.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtwbxbvnbu.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gthnzxwxdm.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtoweoaibi.html

[R70] 时间戳与互转
来源：http://hz.yanxiufei.cn/gtenecvzvk.html

date +%s;  date -d @1700000000
来源：http://hz.redwolf501.top/gtiebguyhn.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtauajcouc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtwdhasnfi.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtxpjkriep.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yangfankeji.com/gtxkwjlvsb.html

[R73] 分割大日志
来源：http://hz.gogol.net.cn/gtrjyzdhnj.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtcifzuwya.html

[R74] 批量重命名
来源：http://hz.xylfe.cn/gtiyoutzdh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtbimipcoi.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtiqjbypty.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.9152youxi.cn/gtkwyzppmt.html

[R76] 使用临时文件
来源：http://hz.daria6918.cn/gtmhzehnpc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtuvixsszw.html

[R77] 读取用户输入
来源：http://hz.jiagoushi.top/gtsubfwrat.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtvqoepmlk.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtcfierpze.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gtynozokzd.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtosdgbqsl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtenynftsm.html

[R80] 查看脚本执行耗时
来源：http://hz.jinyuanbaomall.cn/gtmnelsotp.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gthfcwyylb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtgivcxvap.html

S. C / C++ 专题
来源：http://hz.redwolf501.top/gtkejwswph.html

================================================================================
来源：http://hz.zhengqikj.top/gtvamhgiul.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gtqcpebyxo.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtegelcgfc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtrkyucuwz.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gtxjfvzbce.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtarfxhijf.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gthpkeaski.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtlfbkrwbr.html

[S04] C：字符串复制
来源：http://hz.chenlongwang.top/gtsblzmgmt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtolvkqxib.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangkeji.top/gthdumyhoh.html

strlen(s)
来源：http://hz.yongpay.top/gtdpqvihtu.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtzlnidgll.html

strcmp(a, b) == 0
来源：http://hz.yanxiufei.cn/gtdtogpwmp.html

[S07] C：数组遍历求和
来源：http://hz.gogol.net.cn/gtibypipap.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtohcidqfz.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtxwtnbsat.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gtztdwgacd.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtdmhboboa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnqzz.top/gtajutrhbk.html

[S10] C：指针与解引用
来源：http://hz.52xcode.cn/gttezgdsyu.html

int *p = &a;  *p = 5;
来源：http://hz.dashuyun.cn/gteelmwnil.html

[S11] C：逐行读文件
来源：http://hz.haohaochexian.top/gtefykdoxz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxinkj.top/gtwfhaornn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtveepysev.html

fclose(f);
来源：http://hz.yanxiufei.cn/gtrtlwxcps.html

[S12] C：写文件
来源：http://hz.chenjidiqi.icu/gtkncytfuu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.vqdsnc.cn/gtixzblaov.html

[S13] C：宏定义
来源：http://hz.zhixingplan.top/gtcrjhcsyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gtevunwwbw.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtavlfgkpm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sysykeji.top/gtipuwnmre.html

[S15] C：类型转换
来源：http://hz.pycfn.com/gtvfsriejd.html

(double) a / b
来源：http://hz.hysaishi.cn/gtusnrctsf.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gtoaeyxkmj.html

x |= (1 << 3);
来源：http://hz.bjfxy.top/gtfuqgjgvu.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtbwhhktpm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtsvpfpmfz.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtablufiha.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gtkyuiwznp.html

[S19] C：快速排序
来源：http://hz.shangyingyoupin.top/gtrjfbigeg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtmmaxmtev.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtmrrviclc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gttkponkas.html

[S21] C：字符类别判断
来源：http://hz.smart0.xyz/gtdzqrnloo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtyyfchyrq.html

[S22] C：字符串转数字
来源：http://hz.birdmap.top/gtflvlbijt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gtfzdedrzz.html

[S23] C：随机数
来源：http://hz.haohaochexian.top/gtdvekwlvl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gttvnohcuy.html

[S24] C：获取本地时间
来源：http://hz.sysykeji.top/gtnnfqcqiu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtcdrlkcqb.html

[S25] C：内存拷贝
来源：http://hz.yuanzhike.top/gtyselpfct.html

memcpy(dst, src, n);
来源：http://hz.xingfuxueyuan.xyz/gtsxdumuqc.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gteourkmqw.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtmqkjehew.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gtqpwylcrc.html

const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtazufpdvc.html

[S28] C：静态变量
来源：http://hz.zycfv.cn/gtszcvutwf.html

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gtjxuehonw.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtvopiuhfi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gttdaeogba.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gthyubovma.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtwirvqsqj.html

#define X_H
来源：http://hz.yj20258.top/gtuzffrzru.html

#endif
来源：http://hz.jinqigufen.top/gtbjsxfbga.html

[S31] C++：Hello World
来源：http://hz.xuetiantiany.cn/gtnqztljug.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtjnabwigl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gtyuaazghn.html

[S32] C++：字符串
来源：http://hz.gotoacloud.top/gtbctfhljq.html

std::string s = "hi";  s += "!";
来源：http://hz.iojbl.cn/gtvzwscntw.html

[S33] C++：vector 增删
来源：http://hz.chenzaomai.com/gthhhjxyfw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtfqrbvqux.html

[S34] C++：遍历 vector
来源：http://hz.zycfv.cn/gtpgdzgzof.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtkeeatltb.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtvvpouuiv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtakpayfwo.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gtsuobpsrz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gttxgnnsgm.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtbzdtdxtp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtnptocpiw.html

[S38] C++：排序
来源：http://hz.xingfuxueyuan.xyz/gtrwwttenr.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gttiimabti.html

[S39] C++：自定义比较器排序
来源：http://hz.mhx1999.top/gtglsnozvv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtrtfubnsj.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtpdobfxqs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.wangdashe.top/gtgkhhfdzp.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtcxmwqdde.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtglpijlcv.html

[S42] C++：继承与虚函数
来源：http://hz.guannengcc.top/gtrxrkhwbf.html

class B : public Base { public: void f() override {} };
来源：http://hz.shzxlz.cn/gttgffzugf.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtqoxqaygh.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtsbictivg.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtciviuqfe.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gthijnfxcp.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtbxxbemkm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtkucvtcgr.html

[S46] C++：函数模板
来源：http://hz.cheryme.top/gtthbftsae.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinghuilouyu.cn/gtmsseywcv.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gtovmjneeb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtcvbhdsrw.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gthglvahep.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnxiangtu.top/gtqpkzbpjr.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtleaswumg.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtapepbegc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gtnvrqkfky.html

[S50] C++：格式化数字
来源：http://hz.xingfuxueyuan.xyz/gtrxrsrtal.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtlmkcimou.html

[S51] C++：显式类型转换
来源：http://hz.jiagoushi.top/gthzxyawds.html

static_cast<double>(a) / b
来源：http://hz.hongshengwenyu.top/gtziysqteg.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtzezsyzgk.html

int size() const noexcept { return n_; }
来源：http://hz.9152youxi.cn/gtrplvlece.html

[S53] C++：移动语义
来源：http://hz.cheryme.top/gtjvkmderx.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtqezzztav.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtbckhjwfh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtavsfiqjr.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtkjemfonm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxinkj.top/gthyqrblpx.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gtftcfrjcz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtfgmdrvxq.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gtcbtlusig.html

constexpr int N = 10;
来源：http://hz.guowangkeji.top/gthybbjrwb.html

[S58] C++：命名空间
来源：http://hz.jqgfzy.top/gtfntwesvo.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtitnazmlt.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtdaxpdxmu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cheryme.top/gtagfwmfha.html

[S60] C++：遍历并删除元素
来源：http://hz.sysykeji.top/gtrpzrjrgo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtkrafhptp.html

================================================================================
来源：http://hz.birdmap.top/gtkmglgqtx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtjdvmlfbs.html

================================================================================
来源：http://hz.yj202588.top/gtnxkxgvpn.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gtrajhggod.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtuzublkbj.html

[T02] Kotlin：变量
来源：http://hz.hysaishi.cn/gttzbesvsg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.kuanghao11.cn/gtolzdmkyo.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gttjutifxr.html

"值: $b"
来源：http://hz.hywenlv.cn/gtumgriici.html

[T04] Kotlin：空安全
来源：http://hz.9152youxi.cn/gtftehgtiy.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gtsazmwnqh.html

[T05] Kotlin：when 表达式
来源：http://hz.gogol.net.cn/gtwnguioys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnxiangtu.top/gteecxvzbd.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtvsmcaawa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sxryk.cn/gtvmcyvfaa.html

[T07] Kotlin：集合过滤
来源：http://hz.tian-w.cn/gtggusdmiq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.c1oappe.top/gtralybjnv.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtbkdjidbt.html

data class User(val name: String, val age: Int)
来源：http://hz.gogol.net.cn/gtafhcljtq.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gtwrulvppd.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtimhepscc.html

[T10] Kotlin：默认参数
来源：http://hz.meibo888.top/gtfowjkbdu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gogol.net.cn/gtsztbdvpe.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtrahpmxmj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtvndgtrbo.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtttyqsmaq.html

val (a, b) = Pair(1, 2)
来源：http://hz.feifeiyinyue.top/gtytrhxlqd.html

[T13] Kotlin：只读 Map
来源：http://hz.hnqzz.top/gtiiezqnum.html

val m = mapOf("a" to 1)
来源：http://hz.redwolf501.top/gtrmzxtopr.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtllhrdtjc.html

for (i in 1..10) println(i)
来源：http://hz.cdnleiting.top/gtmeczfssv.html

[T15] Kotlin：接口
来源：http://hz.vqdsnc.cn/gtczdbwfcu.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtywefjxvs.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtzgsrksqi.html

print("Hello")
来源：http://hz.sufxvd.cn/gtvgxdomyy.html

[T17] Swift：变量与常量
来源：http://hz.cdnleiting.top/gticxoreef.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtbrydsedy.html

[T18] Swift：字符串插值
来源：http://hz.nanxinkj.top/gtlmxjscfs.html

"值: \(b)"
来源：http://hz.tianlin.xyz/gthwnndczs.html

[T19] Swift：可选绑定
来源：http://hz.guowangkeji.top/gtfqrocwtw.html

if let n = opt { print(n) }
来源：http://hz.cqqwz.cn/gtlzrsgqlt.html

[T20] Swift：数组操作
来源：http://hz.cucudq.cn/gtkmwwhnzc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gtozcryptr.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtzfwuptac.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtpiawsear.html

[T22] Swift：字典
来源：http://hz.yuanzhike.top/gtlogqxuni.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtvhzydzzh.html

[T23] Swift：函数
来源：http://hz.zhijiandao.cn/gtzvvsmrgf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shzxlz.cn/gttxjxogwt.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtutrftldx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gtvzfmjyfc.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtxjtoefvs.html

struct P { var x: Int }
来源：http://hz.cdnleiting.top/gtdavcziyk.html

[T26] Swift：类与重写
来源：http://hz.gotoacloud.top/gtohnaqzhn.html

class A: Base { override func f() {} }
来源：http://hz.jlsjyb.cn/gtscrkjeke.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtimnoaetk.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtopxlamhe.html

[T28] Swift：枚举
来源：http://hz.yj20258888.top/gticznkscn.html

enum Color { case red, green }
来源：http://hz.dianchejie.cn/gtzjgtxonp.html

[T29] Swift：guard 提前返回
来源：http://hz.xuanzx.com/gttlwxzhpr.html

guard let x = opt else { return }
来源：http://hz.jiagoushi.top/gtvgipdtig.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtewmdqbrn.html

protocol Shape { func area() -> Double }
来源：http://hz.0kj1m.cn/gtlilfiunz.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangtech.top/gtswnueesw.html

print("Hello")
来源：http://hz.birdmap.top/gtrdyrajul.html

[T32] Lua：局部变量
来源：http://hz.bjfxy.top/gtvyjfvyyw.html

local a = 1
来源：http://hz.gaohongyu789.top/gtdvbgppxw.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gtggnoszfc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xingfuxueyuan.xyz/gtjcrurujy.html

[T34] Lua：遍历表
来源：http://hz.sweek.top/gttbxjfzrv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shanyushiyangkeji.top/gtbnjdvwne.html

[T35] Lua：字典表
来源：http://hz.jlsjyb.cn/gttsutalpn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtdqnqskyx.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtstbizfgo.html

function add(a, b) return a + b end
来源：http://hz.vqdsnc.cn/gtpbyvukzi.html

[T37] Lua：字符串拼接
来源：http://hz.feifeiyinyue.top/gtijiexpxe.html

"a" .. "b"
来源：http://hz.ppjwa.cn/gtqrphfhcu.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtoadfpyvq.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtcwvqmisu.html

[T39] Lua：模式匹配
来源：http://hz.nanxinkj.top/gtnaomudvp.html

string.find(s, "%d+")
来源：http://hz.mhx1999.top/gtwayocszx.html

[T40] Lua：元表
来源：http://hz.guowangkeji.top/gtswvmevvc.html

setmetatable({}, { __index = base })
来源：http://hz.gaohongyu789.top/gtcvpxgapj.html

[T41] Perl：Hello World
来源：http://hz.pengpengdd.cyou/gtqkjjqwor.html

print "Hello\n";
来源：http://hz.yuxming.cn/gtjqgsqyjr.html

[T42] Perl：变量类型
来源：http://hz.cdnleiting.top/gtbtvxojrm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtqokfqdtt.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangkeji.top/gthbautvjr.html

"值: $a"
来源：http://hz.ywan-chungtsiang.top/gtzuopkxtm.html

[T44] Perl：条件
来源：http://hz.ybcxt.top/gtwaubxhvy.html

if ($a > 0) { print "正"; }
来源：http://hz.zhixingplan.top/gttkuhfujs.html

[T45] Perl：数组遍历
来源：http://hz.sufxvd.cn/gtaifnepkm.html

for my $x (@arr) { print $x; }
来源：http://hz.xylfe.cn/gttqppmvfb.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gttwuaoysm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.mhx1999.top/gtneqpbmcw.html

[T47] Perl：正则捕获
来源：http://hz.ydzc1.top/gtlcxahcvm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhongyouzk.top/gtwsizztmu.html

[T48] Perl：正则替换
来源：http://hz.xuanzx.com/gtvloqibgs.html

$s =~ s/old/new/g;
来源：http://hz.xuanzx.com/gtzppfiseo.html

[T49] Perl：函数
来源：http://hz.wangdashe.top/gtnpdovdjo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xziqi.cn/gtuixcxije.html

[T50] Perl：逐行读文件
来源：http://hz.quarkkingdee.top/gtaypcwajz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hnqzz.top/gtgurijcxo.html


<!-- 参考信息 -->