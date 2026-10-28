代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtxoaovqtp.html

[R50] awk 求和
来源：http://hz.gzhubu.top/gtcayhfvdg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtjjpsioph.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gthxfgzfnd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnqzz.top/gtaliqqhpt.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtkrbsjzsc.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtwkhjmitt.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtwjueebtw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtfeehqkma.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtmihgexgx.html

diff a.txt b.txt
来源：http://hz.jlsjyb.cn/gthsvapohe.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtjaqjzuvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtqqmezeuo.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtcbgorabk.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtiuegkztt.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtvvstbwdp.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtatppfbxs.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtzeuvjsad.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhongyouzk.top/gtfhxuyfxf.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtfmzqdset.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fzhhl.top/gtailfqeyn.html

[R60] 只看 HTTP 状态码
来源：http://hz.yangfankeji.com/gtnjkemtwf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.redwolf501.top/gtxkhppfnb.html

[R61] 磁盘占用
来源：http://hz.ywan-chungtsiang.top/gtnnmbfamd.html

df -h;  du -sh *
来源：http://hz.aibaodan.cn/gtwhllvckx.html

[R62] 找最占空间的文件
来源：http://hz.zhengqikj.top/gtfeiuwkpr.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtyqbfdxnp.html

[R63] 内存与进程
来源：http://hz.iojbl.cn/gtwafufwfq.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtocgqnklb.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gtzmjjbyct.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtmvtnfehj.html

[R65] 查看端口占用
来源：http://hz.yj202588.top/gtonlzrlrr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtljxsrwyf.html

[R66] 定时任务
来源：http://hz.shanyushiyangkeji.top/gttwsfpnae.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gtqfeeisxz.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtmgaiqbbh.html

openssl rand -hex 16
来源：http://hz.zhijiandao.cn/gtwdpsaiqr.html

[R68] 计算文件校验值
来源：http://hz.yangfankeji.com/gtjeownbjb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtzdiaaoso.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtxlilarpy.html

head -c 16 /dev/urandom | base64
来源：http://hz.zycfv.cn/gtomuomcow.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtqnodtxrj.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtnjocxnll.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtbfbxyqla.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xziqi.cn/gtrevjvdmo.html

[R72] 等待端口就绪
来源：http://hz.chenzaomai.com/gtmkotxxls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtugkagqvn.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtgguctret.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtlxjjjwid.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gtkxfdrqno.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtedcibtlo.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtdxmfrpxr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hongshengwenyu.top/gthaatdbxh.html

[R76] 使用临时文件
来源：http://hz.zhijiandao.cn/gtgjgmceeu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtwlnmizuk.html

[R77] 读取用户输入
来源：http://hz.ybcxt.top/gtvpdkwsgv.html

read -rp "请输入: " ans
来源：http://hz.yongpay.top/gtvdidzpgn.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtusykirkb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtvidwautx.html

[R79] 解析命令行选项
来源：http://hz.haohaochexian.top/gtfwmmkvut.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtlxkrcrip.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgufenzy.top/gtwmmczhjd.html

time ./run.sh
来源：http://hz.shuidangran.top/gtkmjnnejg.html

================================================================================
来源：http://hz.xuanzx.com/gtfbzxfjkw.html

S. C / C++ 专题
来源：http://hz.gogol.net.cn/gtdtgegwpo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqtsjtaji.html

[S01] C：Hello World
来源：http://hz.kuanghao11.cn/gtflkiersy.html

#include <stdio.h>
来源：http://hz.tian-w.cn/gtxjyaoulx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigfzy.top/gtpxdutihn.html

[S02] C：变量与格式化输出
来源：http://hz.gzhubu.top/gtunlgywzf.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtfbncyair.html

[S03] C：读入整数
来源：http://hz.guannengcc.top/gtuysbytah.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtujtewwji.html

[S04] C：字符串复制
来源：http://hz.dashuyun.cn/gtujkijpss.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gtfnidubnr.html

[S05] C：字符串长度
来源：http://hz.andypj.xyz/gtphxgmmir.html

strlen(s)
来源：http://hz.xinyue.icu/gtjizuzbgu.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtjrahvjqb.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtgehzbitx.html

[S07] C：数组遍历求和
来源：http://hz.jianghu66.top/gtanqktdvz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtukzhtoaa.html

[S08] C：动态内存分配与释放
来源：http://hz.zycfv.cn/gtogookepb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daria6918.cn/gtjytbsrhm.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtlnxwydhs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtjrkhptvh.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtdzaxcpbh.html

int *p = &a;  *p = 5;
来源：http://hz.jqgfzy.top/gtpjkicnrr.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtqrwtpuwk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yanxiufei.cn/gttttkivii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.c1oappe.top/gtunrrdhrp.html

fclose(f);
来源：http://hz.jqgufenzy.top/gtakujowro.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtslmntjhr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtuhiehymm.html

[S13] C：宏定义
来源：http://hz.yuxming.cn/gtgxqcrone.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtmezwcrdn.html

[S14] C：枚举
来源：http://hz.yanxiufei.cn/gtlrogwirs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtcrlxwpis.html

[S15] C：类型转换
来源：http://hz.vqdsnc.cn/gtyhrtteok.html

(double) a / b
来源：http://hz.yj202588.top/gtfiuarjkf.html

[S16] C：位操作置位
来源：http://hz.kuanghao11.cn/gtwvbdegqf.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtjvhxjftl.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtaqhplznk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nwbrower.top/gtgicesjmy.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtdoxtnqna.html

int main(int argc, char **argv)
来源：http://hz.cheryme.top/gtsyvfdmqk.html

[S19] C：快速排序
来源：http://hz.jyoumei.cn/gtswyehlbw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtfxmgkova.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtkqxukfzk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtszulhlye.html

[S21] C：字符类别判断
来源：http://hz.ppjwa.cn/gtkeauhkrz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtyurwjudd.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtpbhkdkui.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtpzvzvktw.html

[S23] C：随机数
来源：http://hz.9152youxi.cn/gtgkujnvuq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.snrcjt.cn/gtroumesbs.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtfivxnjrq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtelhztwim.html

[S25] C：内存拷贝
来源：http://hz.andypj.xyz/gtckglxtal.html

memcpy(dst, src, n);
来源：http://hz.zhengqikj.top/gtdnfsrmnq.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtabfcmioo.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gtivdfqong.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtrjqhhtso.html

const double PI = 3.14159;
来源：http://hz.haohaochexian.top/gthydqaddy.html

[S28] C：静态变量
来源：http://hz.9152youxi.cn/gttygssdcq.html

static int counter = 0;
来源：http://hz.jyoumei.cn/gtnpptpgol.html

[S29] C：变参函数
来源：http://hz.nwbrower.top/gtoiuxmlwn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jianghu66.top/gtloycxtvm.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtpbiyvapj.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtwsxxqpdq.html

#define X_H
来源：http://hz.xziqi.cn/gtmtwfbcjd.html

#endif
来源：http://hz.jinghuilouyu.cn/gtanpbvvpl.html

[S31] C++：Hello World
来源：http://hz.yanxiufei.cn/gtmzkbgmsy.html

#include <iostream>
来源：http://hz.jinghuilouyu.cn/gtooiqlfia.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gttkfobgzj.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtciifjssv.html

std::string s = "hi";  s += "!";
来源：http://hz.nwbrower.top/gtdokbiglb.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtabwdfzni.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.birdmap.top/gtsrhnihdh.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtmvkxwato.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtqmsrlkmx.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtkisfvyqa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtrfvzsryw.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gterbvjwuw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtuhcaeinm.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtheworbpv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtawvgmnfs.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtkfmicaxx.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtwfetklim.html

[S39] C++：自定义比较器排序
来源：http://hz.jianghu66.top/gttbiomgjo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtlcbvgmhm.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtqezjfgok.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtmjflofkc.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gteiusdfif.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtxvshyzky.html

[S42] C++：继承与虚函数
来源：http://hz.sufxvd.cn/gtjhsigjec.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangshuangyany.cn/gtxzcukggl.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gthzgkwszq.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtbdvoxzwq.html

[S44] C++：引用传参
来源：http://hz.yvedp.cn/gtykuvbivn.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtzxnzeuba.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtjawsrmng.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xziqi.cn/gteyswulgv.html

[S46] C++：函数模板
来源：http://hz.dianchejie.cn/gteesuejzb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenjidiqi.icu/gtmbchwlep.html

[S47] C++：结构化绑定遍历
来源：http://hz.yongpay.top/gtxfxfpvki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangtech.top/gtjodiflav.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gttwfjyuzj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtpkxliwzz.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtxtcaimjq.html

[S49] C++：写文件
来源：http://hz.ppjwa.cn/gtrsihbzye.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtrsbcdila.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gteyssuiaa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenzaomai.com/gtmzfxauqo.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtvwkajgff.html

static_cast<double>(a) / b
来源：http://hz.zhoulong.xyz/gtisafyzct.html

[S52] C++：const 与 noexcept
来源：http://hz.hongshengwenyu.top/gtckmjmvxr.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtuzjoxpqd.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtedhzejjo.html

std::vector<int> w = std::move(v);
来源：http://hz.chenlongwang.top/gtcznetvhz.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gtexzydtcs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yvedp.cn/gthwcmuark.html

[S55] C++：结构化绑定
来源：http://hz.hnqzz.top/gtjetpvgfq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhoulong.xyz/gtbyuuklho.html

[S56] C++：optional
来源：http://hz.ybcxt.top/gtpoulwncr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.svipenyu.cn/gtolffslea.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gttvjtwntg.html

constexpr int N = 10;
来源：http://hz.jinghuilouyu.cn/gtvchceefk.html

[S58] C++：命名空间
来源：http://hz.c1oappe.top/gtmftbqsmb.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhengqikj.top/gtkyremrbk.html

[S59] C++：静态断言
来源：http://hz.jqgfzy.top/gtgomllyba.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.52xcode.cn/gtqjltrovg.html

[S60] C++：遍历并删除元素
来源：http://hz.jyoumei.cn/gtyuzicrlt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.bjfxy.top/gtphfdhuid.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtswqtvksu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtswlxfyfv.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmgzxlgsq.html

[T01] Kotlin：Hello World
来源：http://hz.ydzc1.top/gtfefoesvg.html

println("Hello")
来源：http://hz.zhixingplan.top/gtszwpcqej.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtbnbuejxq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtfqdjihvt.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtykxzexvw.html

"值: $b"
来源：http://hz.zhixingplan.top/gtumdmiivw.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtllartrdi.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangtech.top/gtstgiwsru.html

[T05] Kotlin：when 表达式
来源：http://hz.yuanzhike.top/gttgoytmta.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtdbhxiekb.html

[T06] Kotlin：集合映射
来源：http://hz.hongshengwenyu.top/gttzkqjvbt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ywan-chungtsiang.top/gtkvkgjxyd.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtycfkdhwo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgfzy.top/gtiipcobwa.html

[T08] Kotlin：数据类
来源：http://hz.cucudq.cn/gtebnhdino.html

data class User(val name: String, val age: Int)
来源：http://hz.hysaishi.cn/gtuekeepxh.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigufen.top/gtuoaswics.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtdyunbssj.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtiaimuskm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtjqubwwpi.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtkeqnzgze.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gaohongyu789.top/gtarrrvwch.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gtmykeyctz.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258.top/gtdchtvusa.html

[T13] Kotlin：只读 Map
来源：http://hz.ybcxt.top/gtpctkaash.html

val m = mapOf("a" to 1)
来源：http://hz.aibaodan.cn/gthpsugzgu.html

[T14] Kotlin：循环
来源：http://hz.xylfe.cn/gttpcuxmtm.html

for (i in 1..10) println(i)
来源：http://hz.iojbl.cn/gtaqrvunir.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gtfmqhynzw.html

interface Shape { fun area(): Double }
来源：http://hz.jiagoushi.top/gtzzypfxig.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtkbstsgif.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtnvsrbqnq.html

[T17] Swift：变量与常量
来源：http://hz.yueranfly.top/gtgmrudsut.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtryybcktx.html

[T18] Swift：字符串插值
来源：http://hz.jianghu66.top/gtftffhtel.html

"值: \(b)"
来源：http://hz.wangshuangyany.cn/gtddkrynpm.html

[T19] Swift：可选绑定
来源：http://hz.cashguo.top/gtoashxwwc.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtavtairqi.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gttypxatgb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xylfe.cn/gtzwlnvyrw.html

[T21] Swift：遍历
来源：http://hz.hywenlv.cn/gtzabafxvo.html

for x in a { print(x) }
来源：http://hz.yj20258.top/gtocapyzkc.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtnvtpkmad.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtoyecmxkb.html

[T23] Swift：函数
来源：http://hz.havefunace.top/gtijquzjzl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jiagoushi.top/gtdgvbpbmh.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtekywrzqj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gtakqsprfn.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtsjiqicoy.html

struct P { var x: Int }
来源：http://hz.zdqjudy.top/gtcmhpxtjy.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtzjtmfoqg.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtjglnnbvr.html

[T27] Swift：错误处理
来源：http://hz.jlsjyb.cn/gtvifrcnci.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gttwvpeyin.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gttunxniza.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtkvmsnztq.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtpazxocbe.html

guard let x = opt else { return }
来源：http://hz.guowangkeji.top/gtsfsxlvyc.html

[T30] Swift：协议
来源：http://hz.yuanzhike.top/gtzpcgxgdr.html

protocol Shape { func area() -> Double }
来源：http://hz.feifeiyinyue.top/gtuupvrlzx.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtrqjhgbiq.html

print("Hello")
来源：http://hz.52xcode.cn/gtmwftkmvm.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtzihsnsnm.html

local a = 1
来源：http://hz.hammf.cn/gttcbplxig.html

[T33] Lua：表（数组）
来源：http://hz.hysaishi.cn/gtzivgsvds.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258.top/gtnjwkvjza.html

[T34] Lua：遍历表
来源：http://hz.birdmap.top/gtvlyjlehv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.quarkkingdee.top/gthappaomj.html

[T35] Lua：字典表
来源：http://hz.havefunace.top/gtszcwbiuh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.havefunace.top/gtzcixgcrk.html

[T36] Lua：函数
来源：http://hz.quarkkingdee.top/gtsavompaq.html

function add(a, b) return a + b end
来源：http://hz.pengpengdd.cyou/gtskmkvxsh.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gtertuopkl.html

"a" .. "b"
来源：http://hz.svipenyu.cn/gtavmohctn.html

[T38] Lua：条件
来源：http://hz.jiagoushi.top/gtemnsfdxm.html

if x > 0 then print("正") end
来源：http://hz.pengpengdd.cyou/gtgplsisln.html

[T39] Lua：模式匹配
来源：http://hz.tianlin.xyz/gtjzoyiofd.html

string.find(s, "%d+")
来源：http://hz.chenjidiqi.icu/gtvjccscbz.html

[T40] Lua：元表
来源：http://hz.zhengqikj.top/gtmbrwyogx.html

setmetatable({}, { __index = base })
来源：http://hz.yueranfly.top/gtkndodzla.html

[T41] Perl：Hello World
来源：http://hz.chenlongwang.top/gtfivbntqi.html

print "Hello\n";
来源：http://hz.tian-w.cn/gtxezwhqoy.html

[T42] Perl：变量类型
来源：http://hz.smart0.xyz/gtragwyjom.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gtgxhbevsi.html

[T43] Perl：字符串插值
来源：http://hz.xuanzx.com/gtfgbtwxnw.html

"值: $a"
来源：http://hz.ybcxt.top/gtsloiivni.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtdzosxdmx.html

if ($a > 0) { print "正"; }
来源：http://hz.mhx1999.top/gtjfnyyinw.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtsmaejiiv.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtvciebhmk.html

[T46] Perl：哈希操作
来源：http://hz.fzhhl.top/gtugupebxk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.haohaochexian.top/gthrikmmhy.html

[T47] Perl：正则捕获
来源：http://hz.hnqzz.top/gtfhjuayay.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxuanxn.top/gtfudmbpue.html

[T48] Perl：正则替换
来源：http://hz.jyoumei.cn/gthwlxkzdj.html

$s =~ s/old/new/g;
来源：http://hz.ehwqpu.com/gtfbibbavb.html

[T49] Perl：函数
来源：http://hz.shanyushiyangtech.top/gtwonjcxgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtqkqogqyg.html

[T50] Perl：逐行读文件
来源：http://hz.nanxinkj.top/gthnnpasdb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.c1oappe.top/gtjusrcceh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yonumen.top/gtuprsctqq.html

[T51] Scala：Hello World
来源：http://hz.guannengcc.top/gtqhzhwzzh.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtiieuppgo.html

[T52] Scala：变量
来源：http://hz.yj20258.top/gthqtvbdet.html


<!-- 参考信息 -->