代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.smart0.xyz/gtrzeygwzd.html

[R46] 递归替换文件内容
来源：http://hz.guowangkeji.top/gtgwgjpahg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtyajauyjq.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gtrhrxiexs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gthvnalvmz.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtevepplwy.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtrikmnrsu.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtyeobcgii.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtacffazcq.html

[R50] awk 求和
来源：http://hz.yuxming.cn/gtphegzzmk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daxiang520.top/gtylipqery.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtjvulgpgh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtdvmrdpvt.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtvrhgwiyq.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtrjecfdxu.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtjkvmlzbv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtzvvzvhal.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtkmqkfnix.html

diff a.txt b.txt
来源：http://hz.zycfv.cn/gtgjgloffx.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtkfaigzqz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtvmscdyeu.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtxzumbhod.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtayffaxmz.html

[R57] 远程执行命令
来源：http://hz.pengpengdd.cyou/gtmypbfvxx.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtcnyvfrbi.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtghaujmdx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cheryme.top/gtnztyxlmx.html

[R59] 发 POST JSON
来源：http://hz.yueranfly.top/gtcvbpmzcv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtnyoktwbk.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gttdrzrmew.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cucudq.cn/gtpvgemlrm.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtybffnnqd.html

df -h;  du -sh *
来源：http://hz.0kj1m.cn/gtvxunuvze.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gthkcbxwkp.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gtowmqauqw.html

[R63] 内存与进程
来源：http://hz.gotoacloud.top/gtwylwxpku.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtjfarmafg.html

[R64] 结束进程
来源：http://hz.aizwys.cn/gtpuxxevgi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtrygnzqhk.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtaiuuqgdr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinyuanbaomall.cn/gtcpszdqvj.html

[R66] 定时任务
来源：http://hz.yvedp.cn/gtugrrqvzq.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtgpmmclrs.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigfzy.top/gtzgllfpgn.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtcmxqhcey.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gtytctonaq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtwkxqstba.html

[R69] 生成随机密码
来源：http://hz.tianlin.xyz/gtcucenarz.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtncbmewth.html

[R70] 时间戳与互转
来源：http://hz.52xcode.cn/gtdfbeubsg.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtozaadmdc.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtnxwwocmi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtwvlbxydn.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gthfkypuzo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sysykeji.top/gtcxmkrxob.html

[R73] 分割大日志
来源：http://hz.jiagoushi.top/gtsqmhqopp.html

split -l 1000 big.log part_
来源：http://hz.shangyingyoupin.top/gtqoowelse.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtcfugihde.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtviabucfy.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtnxzyzmok.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtdjznzbgm.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gtzjkqzuci.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtlhsxacma.html

[R77] 读取用户输入
来源：http://hz.cdnleiting.top/gtihhvqafl.html

read -rp "请输入: " ans
来源：http://hz.0kj1m.cn/gtxgspfcqp.html

[R78] 交互式菜单
来源：http://hz.zdqjudy.top/gtunebxhrt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dashuyun.cn/gtujinpozn.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtrwgpmmer.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinghuilouyu.cn/gtcmrsefqf.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtjojxhfvf.html

time ./run.sh
来源：http://hz.zhengqikj.top/gtakyqanyq.html

================================================================================
来源：http://hz.sufxvd.cn/gtkxgalugg.html

S. C / C++ 专题
来源：http://hz.zhongyouzk.top/gtafgayvqw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwbskhztp.html

[S01] C：Hello World
来源：http://hz.pengpengdd.cyou/gtktwpftgn.html

#include <stdio.h>
来源：http://hz.birdmap.top/gttbdacpsi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hfpthk.cn/gtetabsaza.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gttnamhxqq.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtyarvbbrj.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtiiwxnfwx.html

int x; scanf("%d", &x);
来源：http://hz.xuanzx.com/gtwpqwrujv.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtepumkwsn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.mhx1999.top/gtaglmmaqp.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtdcdlkklj.html

strlen(s)
来源：http://hz.0kj1m.cn/gtcqgsysgu.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtcduwqffw.html

strcmp(a, b) == 0
来源：http://hz.52xcode.cn/gtaxamgrlc.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtgimmojcu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtmxnwtvxe.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtygwyeurx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gtzuijxuya.html

[S09] C：结构体定义与初始化
来源：http://hz.xziqi.cn/gtjmwksxgy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinghuilouyu.cn/gtpmwoclpd.html

[S10] C：指针与解引用
来源：http://hz.aibaodan.cn/gtjrmyozdw.html

int *p = &a;  *p = 5;
来源：http://hz.jlsjyb.cn/gtcbjboqkd.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtqpccswyp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gtjboxqycf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtflsfnjua.html

fclose(f);
来源：http://hz.chenjidiqi.icu/gthjoawpek.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtzdbqdpyj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuanzhike.top/gtenwgutth.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtodrzbpkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtiincnbpx.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtlmsgprfk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtzuqlgslu.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtnwocwfxk.html

(double) a / b
来源：http://hz.dianchejie.cn/gtyzwgpcdo.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtqarlnixz.html

x |= (1 << 3);
来源：http://hz.9152youxi.cn/gthcpvasqy.html

[S17] C：安全拼接字符串
来源：http://hz.jyoumei.cn/gtqvkcezbn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gthuidxrqe.html

[S18] C：命令行参数
来源：http://hz.sufxvd.cn/gtjwjyeost.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtaoezmzpm.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtauttswhk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtvtxksduk.html

[S20] C：二分查找
来源：http://hz.chenzaomai.com/gteguigykw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtejvhygbg.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtbwwqetih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dashuyun.cn/gtotzexloa.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtceiukldy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtmzexhcxa.html

[S23] C：随机数
来源：http://hz.zhiwuduotai.top/gtfmhhbgoj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtqjgsikoe.html

[S24] C：获取本地时间
来源：http://hz.mhx1999.top/gtbofeyope.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gtoivyhhnf.html

[S25] C：内存拷贝
来源：http://hz.nwbrower.top/gtljarxikc.html

memcpy(dst, src, n);
来源：http://hz.guannengcc.top/gtnwkjyitf.html

[S26] C：内存清零
来源：http://hz.ywan-chungtsiang.top/gtwrppymvh.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtrdzrafbq.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtdtqvddha.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtzspkrkia.html

[S28] C：静态变量
来源：http://hz.shzxlz.cn/gtyvowinnw.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtxtssitjo.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gtxujlklya.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtsjehrsdd.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtovhhleug.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtdnvzngsr.html

#define X_H
来源：http://hz.snrcjt.cn/gtjvimplfn.html

#endif
来源：http://hz.ydjk.org.cn/gtfmmygrez.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtxhwhbxoq.html

#include <iostream>
来源：http://hz.birdmap.top/gtzitsaieb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gttlnqvshi.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtkjcnutxa.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtvpjuechn.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtdixjobih.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.mhx1999.top/gtdnjngqlf.html

[S34] C++：遍历 vector
来源：http://hz.ybcxt.top/gtiwpfrzxk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shzxlz.cn/gtrdwmwwpb.html

[S35] C++：map
来源：http://hz.daxiang520.top/gtjftwbeym.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtffokbftb.html

[S36] C++：unordered_map
来源：http://hz.pengpengdd.cyou/gtjazzzese.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtfojkpfab.html

[S37] C++：set
来源：http://hz.shzxlz.cn/gtwrbzsecb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangtech.top/gtvfnlyfmg.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtycwbcrum.html

std::sort(v.begin(), v.end());
来源：http://hz.shangyingyoupin.top/gtqfefcrys.html

[S39] C++：自定义比较器排序
来源：http://hz.pycfn.com/gtjaltximw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtmpvrqilf.html

[S40] C++：查找元素
来源：http://hz.9152youxi.cn/gtrldbiqbi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtjrjrwntp.html

[S41] C++：类与构造函数
来源：http://hz.sysykeji.top/gtfgdhznqo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtxtwrvcss.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtcforxdwz.html

class B : public Base { public: void f() override {} };
来源：http://hz.shzxlz.cn/gtirldjqxv.html

[S43] C++：智能指针
来源：http://hz.jlsjyb.cn/gtipdjpkex.html

auto p = std::make_unique<int>(5);
来源：http://hz.fengsongda.top/gtugtwiugs.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gtnpjhumlp.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtulvkibir.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtnywyzkue.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtljvtenyz.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtllyidida.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtzlhuybrx.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtwjoogssb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj202588.top/gtwxdaqhvy.html

[S48] C++：逐行读文件
来源：http://hz.meibo888.top/gtmpuyioyz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtumomkyst.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtgfwbibqv.html

[S49] C++：写文件
来源：http://hz.dianchejie.cn/gtutwfrknf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtunkfdhog.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtdswowgjd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtevrwucnk.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtxsadvaht.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtyupxifar.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtdbmjqyeg.html

int size() const noexcept { return n_; }
来源：http://hz.iojbl.cn/gtfjaxcmxt.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gtzkpjmolu.html

std::vector<int> w = std::move(v);
来源：http://hz.52xcode.cn/gtpxmrnvol.html

[S54] C++：异常处理
来源：http://hz.jlsjyb.cn/gthvibxgeu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gtwitnrcmc.html

[S55] C++：结构化绑定
来源：http://hz.xingfuxueyuan.xyz/gtpuopbwpg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtmwvkxsoz.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtxvrqslzw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xingfuxueyuan.xyz/gtcwvztcwh.html

[S57] C++：编译期常量
来源：http://hz.jinqigfzy.top/gtvnollich.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtnielqoll.html

[S58] C++：命名空间
来源：http://hz.xuanzx.com/gtscomtuvi.html

namespace ns { int f() { return 1; } }
来源：http://hz.yanxiufei.cn/gtuzcguxzo.html

[S59] C++：静态断言
来源：http://hz.shanyushiyangtech.top/gthskkbmtg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.quarkkingdee.top/gtzzchdgmx.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtcmjqaugz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtstraigsl.html

================================================================================
来源：http://hz.dashuyun.cn/gtxwucsups.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtrivoupnl.html

================================================================================
来源：http://hz.xziqi.cn/gtvciklufr.html

[T01] Kotlin：Hello World
来源：http://hz.chenzaomai.com/gtspbogyzb.html

println("Hello")
来源：http://hz.shuidangran.top/gtrwcirqjl.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtnsgxkgdc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtypfzbsjb.html

[T03] Kotlin：字符串模板
来源：http://hz.52xcode.cn/gthpgqmtwq.html

"值: $b"
来源：http://hz.sysykeji.top/gtwiethgjr.html

[T04] Kotlin：空安全
来源：http://hz.tianlin.xyz/gtejzgbisk.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtdmqxbywi.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtpcsinmnu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yonumen.top/gtxqyfxyaz.html

[T06] Kotlin：集合映射
来源：http://hz.guannengcc.top/gtjbhgellh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtnettpajv.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gttqicuvye.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuanzx.com/gtrzffevxq.html

[T08] Kotlin：数据类
来源：http://hz.xuanzx.com/gtelddjpcm.html

data class User(val name: String, val age: Int)
来源：http://hz.yj202588.top/gtvyjtpjoc.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258888.top/gthrjkgyja.html

fun String.exclaim() = this + "!"
来源：http://hz.feifeiyinyue.top/gtzzbqxifr.html

[T10] Kotlin：默认参数
来源：http://hz.ydjk.org.cn/gtzbzzlmxi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cucudq.cn/gtotsdupkf.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtibwdsunt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtteyeogkn.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtqqsqvluw.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtweuxnzxn.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtuvrlnwlj.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtmstdbdwd.html

[T14] Kotlin：循环
来源：http://hz.jyoumei.cn/gtcdhejrcn.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtahwbmhfr.html

[T15] Kotlin：接口
来源：http://hz.sysykeji.top/gtluyxxmbk.html

interface Shape { fun area(): Double }
来源：http://hz.jiagoushi.top/gtqwsytolf.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gtwkxvheev.html

print("Hello")
来源：http://hz.jianghu66.top/gtxlmxgouu.html

[T17] Swift：变量与常量
来源：http://hz.hysaishi.cn/gtmqqbckkb.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtarmudhth.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gtnlvcmfvu.html

"值: \(b)"
来源：http://hz.xziqi.cn/gtwfkmztfo.html

[T19] Swift：可选绑定
来源：http://hz.svipenyu.cn/gtxzfyswxb.html

if let n = opt { print(n) }
来源：http://hz.nanxinkj.top/gteectfrgt.html

[T20] Swift：数组操作
来源：http://hz.mhx1999.top/gtoecytsog.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xinyue.icu/gtxisihwlc.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gtiozmdnms.html

for x in a { print(x) }
来源：http://hz.meibo888.top/gtyptttwat.html

[T22] Swift：字典
来源：http://hz.svipenyu.cn/gtwncvrfiv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gtqrxqhvws.html

[T23] Swift：函数
来源：http://hz.yj202588.top/gtejaqboyv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sxryk.cn/gteobpfbml.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtajhyqeld.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtfglhmxma.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gtmlfntjxd.html

struct P { var x: Int }
来源：http://hz.sufxvd.cn/gtykwwewbx.html

[T26] Swift：类与重写
来源：http://hz.quarkkingdee.top/gtlojhdkuj.html

class A: Base { override func f() {} }
来源：http://hz.hysaishi.cn/gtcozanyvp.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtnjktkpfa.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtbvepwnmv.html

[T28] Swift：枚举
来源：http://hz.tian-w.cn/gtepqwmfmw.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gthtwkmsfh.html

[T29] Swift：guard 提前返回
来源：http://hz.ydjk.org.cn/gtmwwuudat.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtaemlgboe.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gtacioyufi.html

protocol Shape { func area() -> Double }
来源：http://hz.tanke756.top/gtgylhcyzv.html

[T31] Lua：Hello World
来源：http://hz.9152youxi.cn/gtpdejwfzu.html

print("Hello")
来源：http://hz.wangdashe.top/gtfauozjvi.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtbkfgvwrb.html

local a = 1
来源：http://hz.yonumen.top/gtkymotjye.html

[T33] Lua：表（数组）
来源：http://hz.jqgfzy.top/gtdqiiigir.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gtvtpwbmlj.html

[T34] Lua：遍历表
来源：http://hz.daria6918.cn/gtjfvaacpg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgfzy.top/gtrrbmofps.html

[T35] Lua：字典表
来源：http://hz.haohaochexian.top/gtoolgrdjy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gtjzkvsnna.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gtmwpmjizn.html

function add(a, b) return a + b end
来源：http://hz.tanke756.top/gtpckzsgky.html

[T37] Lua：字符串拼接
来源：http://hz.nanxinkj.top/gtlappsdmq.html

"a" .. "b"
来源：http://hz.52xcode.cn/gtwhmwtafl.html

[T38] Lua：条件
来源：http://hz.wangshuangyany.cn/gtugbkvfwn.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtshqcfmsm.html

[T39] Lua：模式匹配
来源：http://hz.52xcode.cn/gtavawjvzi.html

string.find(s, "%d+")
来源：http://hz.yueranfly.top/gtfhgayiqf.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gtixbtrdqa.html

setmetatable({}, { __index = base })
来源：http://hz.jinghuilouyu.cn/gtqqgbshlx.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gttftnsjsk.html

print "Hello\n";
来源：http://hz.mhx1999.top/gtsarsvdud.html

[T42] Perl：变量类型
来源：http://hz.shuidangran.top/gtwscssikf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtdnjzgkxl.html

[T43] Perl：字符串插值
来源：http://hz.xuanzx.com/gtnlnehrms.html

"值: $a"
来源：http://hz.zhaomingkeji.xyz/gterlwmvus.html

[T44] Perl：条件
来源：http://hz.sysykeji.top/gtgjkantio.html

if ($a > 0) { print "正"; }
来源：http://hz.daxiang520.top/gtkajrmrem.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtkmdbzyzm.html

for my $x (@arr) { print $x; }
来源：http://hz.nwbrower.top/gtcmvlbnye.html

[T46] Perl：哈希操作
来源：http://hz.daria6918.cn/gtnpzskhjv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zdqjudy.top/gtxzkstydt.html

[T47] Perl：正则捕获
来源：http://hz.jinyuanbaomall.cn/gtqvyadngd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.quarkkingdee.top/gthrmjqiph.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gtaojjwzms.html

$s =~ s/old/new/g;
来源：http://hz.zdqjudy.top/gtubcxxqnm.html


<!-- 参考信息 -->